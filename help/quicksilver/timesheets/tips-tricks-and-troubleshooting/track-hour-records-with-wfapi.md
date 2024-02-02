---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Adobe Workfront API を使用して時間レコードをトラック
description: 組織で Adobe Workfront を使用して勤務時間を入力しており、そのデータの記録システムとして別のツールを使用している場合は、Workfront API を使用して 2 つのシステム間でデータを同期できます。
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: ht
source-wordcount: '386'
ht-degree: 100%

---

# Adobe Workfront API を使用して時間レコードをトラック

組織で Adobe Workfront を使用して勤務時間を入力しており、そのデータの記録システムとして別のツールを使用している場合は、Workfront API を使用して 2 つのシステム間でデータを同期できます。

時間エントリが削除されるとレコード全体が削除され、データセット全体を取得して以前のデータセットと比較する必要があるので、単純に時間レコードを追跡する手法は現実的ではありません。幸いにも、すべての時間トランザクションは Workfront ジャーナルエントリに記録されます。

システム内の現在の時間の初期セットをすべて取得した後で、ジャーナルエントリを通じてあらゆる変更を追跡できます。
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>以下で、含まれるフィールドについて説明します。

* **changeType：**&#x200B;オブジェクトに加えられる変更のタイプ：

   * **A：**&#x200B;追加

   * **E：**&#x200B;編集

   * **D：**&#x200B;削除

* **aux2：**&#x200B;時間レコードの対象となるユーザーの名前。

* **newNumberVal：**&#x200B;時間レコードの新しい値（changeType が D の場合は null になります）。

* **oldNumberVa：**&#x200B;時間レコードの前の値。

* **subObjCode：**&#x200B;変更するレコードのタイプ（常に HOUR にする必要があります）。

* **subObjID**&#x200B;時間レコードの ID。

この情報を使用すると、変更、編集または削除された時間レコードを確認できます。その後、必要に応じて subObjID を使用して、時間レコードから詳細情報を取得できます。
