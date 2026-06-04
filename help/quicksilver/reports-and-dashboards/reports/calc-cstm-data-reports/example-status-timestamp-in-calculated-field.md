---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算済みカスタムフィールドの例：カスタムフォームにステータスタイムスタンプを表示する
description: 次の計算フィールドには、オブジェクトステータスが進行中（INP）としてマークされた日付が表示されます。 イシュー、タスクまたはプロジェクトに関する計算カスタムフィールドにも同じ情報を使用できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OsYpPu9dAsSEQE6BBkvGovNR5E6I7k0BC2n48R7psLg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 343
ht-degree: 86%

---

# 計算済みカスタムフィールドの例：カスタムフォームにステータスタイムスタンプを表示する

次の計算フィールドには、オブジェクトステータスが進行中（INP）としてマークされた日付が表示されます。 イシュー、タスクまたはプロジェクトに関する計算カスタムフィールドにも同じ情報を使用できます。

>[!NOTE]
>
>オブジェクトのステータスが INP に変わり、別のステータスに変わった後、INP に戻った場合、Adobe Workfront は最初に INP に変わった時点のタイムスタンプのみをキャプチャします。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront パッケージ</p> </td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront プラン</p> </td> 
   <td>
      <p>標準</p>
      <p>プラン</p></td>
  </tr> 
  <tr> 
   <td><p>アクセスレベル設定</p></td> 
   <td> <p>レポート、ダッシュボードおよびカレンダーの作成へのアクセス権の編集</p> </td> 
  </tr> 
  <tr> 
   <td> <p>オブジェクト権限</p> </td> 
   <td> <p>フォームが添付されたオブジェクトに対する権限の管理</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

フィールドの編集履歴を表示する計算フィールドをカスタムフォームに追加するには、まずカスタムフォームを作成する必要があります。

## カスタムフォームへのステータスタイムスタンプの表示

1. フィールドを追加するカスタムフォームに移動します。
1. 「**計算済み**」をクリックして、計算済みカスタムフィールドをフォームに追加します。
1. カスタムフィールドに&#x200B;**Label**&#x200B;を入力します。 例えば、「ステータスタイムスタンプカスタムフィールド」のように指定します。
1. 「**保存して閉じる**」をクリックします。
1. カスタムフォームを再度開き、フォームで新しい&#x200B;**ステータスタイムスタンプカスタムフィールド**&#x200B;を選択します。
1. 「**計算**」ボックスに、カスタムフィールド用の次の計算をコピーして貼り付けます。

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >この計算は、すべてのオブジェクトとすべてのステータスで同じです。 この計算でのオブジェクトのステータスのステータス名ではなく、常に 3 文字のキーを使用する必要があります。
   >
   >ステータスのキーについて詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   現在は、ステータスタイムスタンプカスタムフィールドに関するレポートを作成したり、他の計算、レポートまたはカスタムフィールドで使用したりできます。
