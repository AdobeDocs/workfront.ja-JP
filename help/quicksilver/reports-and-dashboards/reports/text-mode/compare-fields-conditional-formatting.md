---
product-area: reporting
navigation-topic: text-mode-reporting
title: 条件付き書式でのフィールドの比較
description: 条件付き書式を使用すると、ビュー内の 2 つの異なるフィールドを比較し、特定の条件が満たされた場合にそれらをハイライト表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 条件付き書式でのフィールドの比較

条件付き書式を使用すると、ビュー内の 2 つの異なるフィールドを比較し、特定の条件が満たされた場合にそれらをハイライト表示できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートのビューを編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理して、レポートの表示を編集します</p> <p>ビューに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 例：実績開始日と計画開始日の比較

たとえば、タスクの実績開始日が計画開始日より後の場合、条件付き書式を使用して「計画開始日」列をハイライト表示できます。

条件付き書式を使用して、タスクの計画開始日と実績開始日を比較する手順は、次のとおりです。

1. タスクビューまたはレポートに移動します。
1. （条件付き）レポートを操作する場合、**列（表示）** 」タブで、条件付き書式を設定する列のヘッダーをクリックして選択します。\
   例えば、 **実際の開始日** 列に条件付き書式を追加する場合は、「計画開始日」フィールドと「実際の開始日」フィールドを比較します。

1. クリック **詳細オプション**」、「 **この列のルール**.

1. ビルダーにある既存の値を使用した比較条件を入力し、条件付き書式を指定します。\
   たとえば、実績開始日が計画開始日より後（またはそれ以上）のタスクを強調表示します。 「次より大きい」修飾子を選択し、日付フィールドで実際の日付を選択します。\
     ![](assets/cond-format-1-350x84.png)

1. （オプション）「 」を選択します。 **行全体に適用** 行全体に書式を適用する場合。
1. クリック **ルールを追加**&#x200B;を、 **完了**.

1. を選択します。 **実際の開始日** 列、「 **テキストモードに切り替え**.

1. **クリックしてテキストを編集** 次に、次のテキスト行を追加します。

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   この例では、次のようになります。 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Workfrontのネイティブフィールドを比較する場合は、フィールド名にキャメルケース構文を使用します。 カスタムフィールドを比較する場合は、 **DE：実際のフィールド名** を選択します。\
   >例えば、 **実際の開始日** というラベルの付いたカスタムフィールド **配信日**&#x200B;テキストモードコードに次の文を追加します。
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. 次を確認します。 `righttext` コード行が `rightmethod` コードの行。

   ![](assets/cond-format-2-350x171.png)

1. 「**保存**」をクリックします。
1. クリック **保存して閉じる**.

   この列では、条件に一致するフィールドが強調表示されます。
