---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: カスタム費用タイプの作成
description: ' [!DNL Adobe Workfront]  管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。 費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
TQID: https://experienceleague.adobe.com/lf8hEp6JYtT4mZPP5f6e5M-gX4juYH-hRZF8kGonN3E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 383
ht-degree: 65%

---

# カスタム費用タイプを作成

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。 費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。

作成した費用タイプは、編集や削除することができます。 ビルトインの [!DNL Workfront] 費用タイプは、削除したり編集したりすることができません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 既定の費用タイプ

削除または編集できない[!DNL Workfront]の既定の費用タイプには、次のものが含まれます。

* [!UICONTROL 広告宣伝費]
* [!UICONTROL コンサルティング]
* [!UICONTROL 接待交際費]
* [!UICONTROL 一般]
* [!UICONTROL 部材費]
* [!UICONTROL 交通費]

## カスタム費用タイプを作成

{{step-1-to-setup}}

1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. **[!UICONTROL 新しい費用タイプ]**&#x200B;をクリックします。
1. **[!UICONTROL 新しい費用タイプ]** ダイアログボックスで、次の情報を入力します。

   * **名前** – 費用の名前。
   * **説明** – 費用の説明。
   * **計算単位** - ドロップダウンリストから、費用タイプの測定単位を選択します。 次の測定単位を使用できます。

      * マイル
      * キロメートル
      * キログラム
      * ドル
      * 時間
      * 日
      * その他 - このオプションを選択すると、測定単位に名前を付け、測定単位を組織にとってなじみのあるものとして定義するよう求められます。

   * **レート** – 単位あたりの価格。 これは通貨形式のフィールドで、**計算単位** フィールドに設定された各単位のコストを表します。 レートには、小数点以下 4 桁までの数値を含めることができます。 例：1.0375

1. 「**[!UICONTROL 保存]**」をクリックします。

   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

## カスタム費用タイプの変更

{{step-1-to-setup}}

1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. 変更する費用タイプを選択し、**[!UICONTROL 編集]** アイコン ![編集アイコン ](assets/edit-icon.png)をクリックします。

   「**[!UICONTROL 費用タイプを編集]**」ダイアログボックスが表示されます。

1. 必要な変更を行い、**[!UICONTROL 保存]**&#x200B;をクリックします。

   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

費用の使用方法とプロジェクトのコストに与える影響に関して詳しくは、「[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)」の記事を参照してください。
