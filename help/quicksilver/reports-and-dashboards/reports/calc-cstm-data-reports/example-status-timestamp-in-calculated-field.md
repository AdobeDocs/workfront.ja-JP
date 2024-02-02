---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 「計算済みカスタムフィールドの例：カスタムフォームにステータスタイムスタンプを表示」
description: 次の計算フィールドには、オブジェクトのステータスが「処理中」（INP）とマークされた日付が表示されます。イシュー、タスクまたはプロジェクトに関する計算カスタムフィールドにも同じ情報を使用できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: ht
source-wordcount: '407'
ht-degree: 100%

---

# 計算済みカスタムフィールドの例：カスタムフォームにステータスタイムスタンプを表示する

次の計算フィールドには、オブジェクトのステータスが「処理中」（INP）とマークされた日付が表示されます。イシュー、タスクまたはプロジェクトに関する計算カスタムフィールドにも同じ情報を使用できます。

>[!NOTE]
>
>オブジェクトのステータスが INP に変わり、別のステータスに変わった後、INP に戻った場合、Adobe Workfront は最初に INP に変わった時点のタイムスタンプのみをキャプチャします。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront ライセンス*</p> </td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>レポート、ダッシュボードおよびカレンダーの作成へのアクセス権の編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>フォームが添付されたオブジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。<br>ダッシュボードの権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">レポート、ダッシュボードおよびカレンダーの共有</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

フィールドの編集履歴を表示する計算フィールドをカスタムフォームに追加するには、まずカスタムフォームを作成する必要があります。

## カスタムフォームへのステータスタイムスタンプの表示

1. フィールドを追加するカスタムフォームに移動します。
1. 「**計算済み**」をクリックして、計算済みカスタムフィールドをフォームに追加します。
1. *ステータスタイムスタンプカスタムフィールド*&#x200B;などのカスタムフィールドの&#x200B;**ラベル**&#x200B;を入力します。
1. 「**完了**」、「**保存して閉じる**」の順にクリックします。
1. カスタムフォームを再度開き、フォームで新しい&#x200B;**ステータスタイムスタンプカスタムフィールド**&#x200B;を選択します。
1. 「**計算**」ボックスに、カスタムフィールド用の次の計算をコピーして貼り付けます。

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >この計算は、すべてのオブジェクトとすべてのステータスで同じです。この計算でのオブジェクトのステータスのステータス名ではなく、常に 3 文字のキーを使用する必要があります。
   >
   >ステータスのキーについて詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   現在は、ステータスタイムスタンプカスタムフィールドに関するレポートを作成したり、他の計算、レポートまたはカスタムフィールドで使用したりできます。
