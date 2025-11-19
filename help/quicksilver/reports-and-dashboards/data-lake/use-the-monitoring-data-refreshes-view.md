---
product-area: reports and dashboards
navigation-topic: data-connect
title: Data Connect のデータ更新の監視ビューの使用
description: Data Connect を使用すると、Workfront管理者は、最新の更新中に Data Lake の日付に対して行われた最新の更新の詳細なレコードにアクセスできます。
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# Data Connect のデータ更新の監視ビューの使用

データ更新の監視ビューには、最新の更新中にデータレイクの日付に対して行われた最新の更新が表示されます。 このビューのデータは、データ読み込みが正常に完了するたびに更新されます。

データ量が多く、集計は複雑であるため、データ更新の監視ビューには、過去 2 週間以内に更新されたオブジェクト・ビューのみが表示されます。 このビューに特定のレコードタイプがない場合は、その期間内のアクティビティの欠如が原因である可能性があります。

>[!NOTE]
>
>このビューには、リフレッシュ・アクティビティ履歴を表示する日次履歴またはイベント・ビューとは対照的に、アプリケーションおよびリフレッシュ・アクティビティによって提供されるデータの詳細なコレクションが表示されます。 リフレッシュ・アクティビティの履歴の詳細を取得するには、<code>DL_LOAD_TIMESTAMP を使用します</code> date オブジェクト。

## データ更新ビュー列の監視

[Monitoring Data Refreshed] ビューの列には、次の情報が表示されます。

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
      データレイクに送信されるWorkfront レコードに関連付けられたオブジェクトタイプ。 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>日付</td>
        <td>
   OBJ_TYPE 列に表示されるオブジェクト・タイプのデータが前回正常にリフレッシュされた日付。 </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 OBJ_TYPE 列に表示されるオブジェクト・タイプの最新データ更新の日時。  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       OBJ_TYPE 列に表示されるオブジェクト・タイプの 2 回目の最新データ更新の日時。 </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>数値</td>
        <td>
     オブジェクトタイプの最後のデータ更新以降の経過時間（分）。 </td>
    </tr>
            <tr>
        <td>作成日時 </td>
        <td>数値 </td>
        <td>オブジェクトタイプの前回と最新のデータ更新の間に取得されたレコードの作成イベントの数。  </td>
    </tr>
                <tr>
        <td>更新日</td>
        <td>数値 </td>
        <td>オブジェクトタイプの前回と最新のデータ更新の間に取得された UPDATE レコードイベントの数。</td>
    </tr>
                <tr>
        <td>削除済み</td>
        <td>数値 </td>
        <td>オブジェクトタイプの前回と最新のデータ更新の間にキャプチャされたDELETE レコードイベントの数。 </td>
    </tr>
                <tr>
        <td>合計</td>
        <td>数値 </td>
        <td>オブジェクトタイプの前回と最新のデータ更新の間のイベント総数のカウント。 
        <br> 
        <br><b> メモ </b>：同じレコードが更新間に複数回作成および更新されるので、これは、CREATE、UPDATE またはDELETE イベントの影響を受けるレコードの合計数とは異なります。  </td>
    </tr>
   </table>

