---
product-area: reports and dashboards
navigation-topic: data-connect
title: Data Connect におけるデータ更新の監視ビューの使用
description: Data Connectを使用すると、Workfront管理者は、最新の更新中にデータレイクの日付に加えられた最近の更新の詳細な記録にアクセスできます。
author: Courtney
feature: Reports and Dashboards
exl-id: 230d1a30-2af9-4d2c-9ec1-34c3d4c080d4
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 6%

---

# Data Connect におけるデータ更新の監視ビューの使用

データ更新の監視ビューには、最新の更新中にデータレイクの日付に対して行われた最近の更新が表示されます。 このビューのデータは、データ読み込みが正常に完了するたびに更新されます。

データ量が多く、集計が複雑であるため、監視データ更新ビューには、過去2週間以内に更新されたオブジェクトビューのみが表示されます。 このビューに特定のレコードタイプがない場合は、その時間枠内のアクティビティの欠如が原因である可能性があります。

>[!NOTE]
>
>このビューには、更新アクティビティ履歴を表示する日次の履歴またはイベントビューではなく、アプリケーションと更新アクティビティによって提供されるデータの詳細なコレクションが表示されます。 履歴リフレッシュ アクティビティの詳細を取得するには、<code>DL_LOAD_TIMESTAMPを利用します</code> date オブジェクト。

## データの監視によるビュー列の更新

監視データ更新ビューの列には、次の情報が含まれています。

<table>
    <tr>
        <td><b>列名</b></td>
        <td><b>タイプ</b></td>
        <td><b>説明</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      データレイクに送信されたWorkfront レコードに関連付けられているオブジェクトタイプ。 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>日付</td>
        <td>
   OBJ_TYPE列に表示されるオブジェクトタイプの最後の正常なデータ更新の日付。 </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 OBJ_TYPE列に表示されるオブジェクトタイプの最新のデータ更新の日時。  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       OBJ_TYPE列に表示されるオブジェクトタイプの2番目の最新のデータ更新の日時。 </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>数値</td>
        <td>
     オブジェクトタイプの最後のデータ更新から経過した時間（分単位）。 </td>
    </tr>
            <tr>
        <td>CREATED </td>
        <td>数値 </td>
        <td>オブジェクト タイプの前のデータ更新と最新のデータ更新の間にキャプチャされたCREATE レコード イベントの数。  </td>
    </tr>
                <tr>
        <td>更新済み</td>
        <td>数値 </td>
        <td>オブジェクト タイプの前のデータ更新と最新のデータ更新の間に取得されたUPDATE レコード イベントの数。</td>
    </tr>
                <tr>
        <td>削除済</td>
        <td>数値 </td>
        <td>オブジェクト型の前回と最新のデータ更新の間にキャプチャされたDELETE レコードイベントのカウント。 </td>
    </tr>
                <tr>
        <td>合計</td>
        <td>数値 </td>
        <td>オブジェクト タイプの前回と最新のデータ更新の間のイベントの合計数です。 
        <br> 
        <br><b>注意</b>：これは、CREATE、UPDATE、またはDELETE イベントの影響を受けるレコードの合計数と同じではありません。同じレコードが、更新の間隔で複数回作成および更新される可能性があるからです。  </td>
    </tr>
   </table>
