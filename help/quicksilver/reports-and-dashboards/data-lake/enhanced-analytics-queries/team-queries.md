---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: チーム別アクティビティクエリ
description: 拡張分析クエリ
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 6f07e52b-b813-4b3a-9333-0c9300e051ca
TQID: https://experienceleague.adobe.com/q4x3b0G-hwtFUAkNyRp1oWnAi09Kh8qFO77U8aDEl98
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 172
ht-degree: 18%

---

# チーム別アクティビティクエリ

この記事のクエリを使用して、Enhanced Analyticsのクエリと同様のデータビジュアライゼーションを作成できます。

>[!IMPORTANT]
>
>クエリは、拡張分析で表示されるクエリと同様の結果を生成しますが、正確に一致しない場合があります。


## 前提条件

開始する前に、

1. Business Intelligence（BI）ツールとの連携を構築する：
   1. [Snowflake のリーダーアカウントまたは接続の作成](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Workfront Data Connect への接続の確立](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

接続を確立したら、この記事のクエリを使用してデータを抽出および視覚化できます。

## Home Teamsのユーザーのログインイベント 

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

### Home Teamsのユーザーのログインイベント：ドリルダウン

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

## チームのユーザーログインイベント

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
    tmc.teamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM teammembers_current tmc 
    inner join teams_current tc on tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    inner join userlogins ul on tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(ul.lastlogindate)
```

### チームのユーザーのログインイベント：ドリルダウンする

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

### チームのユーザーのタスク完了イベント：ドリルダウンする

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
