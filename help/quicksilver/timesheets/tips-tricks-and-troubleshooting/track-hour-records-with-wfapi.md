---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Adobe Workfront API を使用した時間レコードの追跡
description: 組織でAdobe Workfrontを使用して勤務時間を入力しているが、別のツールをそのデータの記録システムとして使用している場合、Workfront API を使用して 2 つのシステム間でデータを同期できます。
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Adobe Workfront API を使用した時間レコードの追跡

組織でAdobe Workfrontを使用して勤務時間を入力しているが、別のツールをそのデータの記録システムとして使用している場合、Workfront API を使用して 2 つのシステム間でデータを同期できます。

hour エントリが削除された場合、レコード全体が削除され、データセット全体を取り込んで古いデータセットと比較する必要があるので、hour レコードは単に追跡できません。 幸いにも、すべての時間トランザクションはWorkfrontジャーナルエントリに記録されます。

システム内の現在の時間の初期セットを取得した後、ジャーナルエントリを通じて、すべての変更を追跡できます。
<pre>GET/attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data":[<br>{<br>"ID":"5785406d008d93dd35665f14d90d4929",<br>"objCode":「JRNLE」<br>"changeType":「A」<br>"aux2":「ブラッド・リトラー」<br>"newNumberVal":1,<br>"oldNumberVal":null,<br>"subObjCode":"HOUR",<br>"subObjID":"5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID":"57854124008da2b9f372c01f8b9054bf",<br>"objCode":「JRNLE」<br>"changeType":「D」<br>"aux2":「ブラッド・リトラー」<br>"newNumberVal":null,<br>"oldNumberVal":1,<br>"subObjCode":"HOUR",<br>"subObjID":"5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID":"5785416f008db05ecee934663a968366",<br>"objCode":「JRNLE」<br>"changeType":「A」<br>"aux2":「ブラッド・リトラー」<br>"newNumberVal":1,<br>"oldNumberVal":null,<br>"subObjCode":"HOUR",<br>"subObjID":"5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID":"57854176008db22fe974b7c67feea6b2",<br>"objCode":「JRNLE」<br>"changeType":「E」<br>"aux2":「ブラッド・リトラー」<br>"newNumberVal":2,<br>"oldNumberVal":1,<br>"subObjCode":"HOUR",<br>"subObjID":"5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>次に、含まれるフィールドの説明を示します。

* **changeType:** オブジェクトに対して行われる変更のタイプ。

   * **回答：** 追加

   * **E:** 編集

   * **D:** 削除

* **aux2:** 時間レコードの対象となるユーザーの名前。

* **newNumberVal:** 時間レコードの新しい値（changeType が D の場合は null になります）。

* **oldNumberVal:** 時間レコードの以前の値。

* **subObjCode:** 変更するレコードのタイプ（常に HOUR にする必要があります）。

* **subObjID:** Hour レコードの ID。

この情報を使用して、変更、編集または削除された時間レコードを確認できます。 その後、必要に応じて subObjID を使用して、時間レコードからさらに多くの情報を取得できます。
