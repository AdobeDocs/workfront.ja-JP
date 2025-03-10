---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: チーム別アクティビティ クエリ
description: Analytics クエリの強化機能
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 6f07e52b-b813-4b3a-9333-0c9300e051ca
source-git-commit: bd39c5794c55e27a876da185e67bf8c654a003b2
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 3%

---

# チーム別アクティビティ クエリ

この記事のクエリを使用して、Enhanced Analytics と同様のデータビジュアライゼーションを作成できます。

>[!IMPORTANT]
>
>クエリは、Enhanced Analytics で表示される結果と同様の結果を生成しますが、完全には一致しない場合があります。


## 前提条件

開始する前に、

1. Business Intelligence（BI）ツールとの接続を確立します。
   1. [Snowflakeのリーダーアカウントまたは接続を作成する](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Workfront Data Connect への接続の確立](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

接続を確立したら、この記事のクエリを使用してデータを抽出および視覚化できます。

## ホームチームのユーザーのログインイベント 

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(ul.lastlogindate) 
```

### ホームチームのユーザーのログインイベント：ドリルダウン

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(ul.lastlogindate)
```

## チーム ユーザーのログインイベント

```
Teams' users' login events 
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM teammembers_current tmc 
    inner join teams_current tc on tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    inner join userlogins ul on tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(ul.lastlogindate)
```

### チームのユーザーのログインイベント：ドリルダウン

```
WITH userlogins as ( 
    SELECT userid, lastlogindate 
    FROM ( 
        SELECT userid, lastlogindate, lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid  ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate), count(*) 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN userlogins ul ON tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate)
```



## ホームチームのユーザーのタスクステータス変更イベント 

```
WITH task_status_changes as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    ) 
    WHERE status != previous_status 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid,  TO_DATE(tsc.begin_effective_timestamp)
```

### ホームチームのユーザーのタスクステータス変更イベント：ドリルダウン

```
WITH task_status_changes as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    ) 
    WHERE status != previous_status 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tsc.begin_effective_timestamp)
```

## チームのユーザーのタスクステータス変更イベント

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
) 

SELECT tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp), count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp) 
```

### チームのユーザーのタスクステータス変更イベント：ドリルダウン

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
WHERE status != previous_status  
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    inner join teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    inner join assignments_current ac ON tmc.userid = ac.assignedtoid  
    inner join task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tsc.begin_effective_timestamp) 
```

## ホームチームのユーザーのタスク完了イベント

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(tasks_done.task_completion_date)
```

### ホームチームのユーザーのタスク完了イベント：ドリルダウン

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        ) 
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tasks_done.task_completion_date) 
```

## チームのユーザーのタスク完了イベント

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(tasks_done.task_completion_date) 
```

### チームのユーザーのタスク完了イベント：ドリルダウン

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT taskid, actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tasks_done.task_completion_date) 
```
