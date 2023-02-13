---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '''計算済みカスタムフィールドの例：カスタムフォームにステータスタイムスタンプを表示する'
description: 次の計算フィールドには、オブジェクトのステータスが「処理中」(INP) とマークされた日付が表示されます。 イシュー、タスク、プロジェクトに関する計算カスタムフィールドにも同じ情報を使用できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 計算済みカスタムフィールドの例：カスタムフォームでのステータスタイムスタンプの表示

次の計算フィールドには、オブジェクトのステータスが「処理中」(INP) とマークされた日付が表示されます。 イシュー、タスク、プロジェクトに関する計算カスタムフィールドにも同じ情報を使用できます。

>[!NOTE]
>
>オブジェクトのステータスが INP に変わり、別のステータスに変わった後、INP に戻った場合、Adobe Workfrontは最初に INP に変わった時点のタイムスタンプのみを取り込みます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>レポート、ダッシュボード、カレンダーの作成へのアクセス権の編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>フォームが添付されているオブジェクトに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.<br>ダッシュボードの権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">レポート、ダッシュボード、カレンダーの共有 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

フィールドの編集履歴を表示する計算フィールドをカスタムフォームに追加するには、まずカスタムフォームを作成する必要があります。

## カスタムフォームにステータスタイムスタンプを表示する

1. フィールドを追加するカスタムフォームに移動します。
1. クリック **計算済み** をクリックして、計算済みカスタムフィールドをフォームに追加します。
1. タイプ a **ラベル** カスタムフィールドの場合： *ステータスタイムスタンプカスタムフィールド*.
1. クリック **完了**&#x200B;を選択し、「 **保存して閉じる**.
1. カスタムフォームを再度開き、新しい **ステータスタイムスタンプカスタムフィールド** をフォームに追加します。
1. 内 **計算** ボックスに、カスタムフィールド用の次の計算をコピーして貼り付けます。

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >この計算は、すべてのオブジェクトとすべてのステータスで同じです。 この計算でのオブジェクトのステータスのステータス名ではなく、常に 3 文字のキーを使用する必要があります。
   >
   >ステータスのキーについて詳しくは、 [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. クリック **保存して閉じる**.

   現在は、ステータスタイムスタンプカスタムフィールドに関するレポートを作成したり、他の計算、レポート、カスタムフィールドで使用したりできます。
