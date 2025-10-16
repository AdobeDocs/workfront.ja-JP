---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: カスタム費用タイプの作成
description: ' [!DNL Adobe Workfront]  管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 62%

---

# カスタム費用タイプを作成

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。

作成した費用タイプは、編集や削除することができます。ビルトインの [!DNL Workfront] 費用タイプは、削除したり編集したりすることができません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
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

[!DNL Workfront] の既定の費用タイプのうち、削除または編集できないものは次のとおりです。

* [!UICONTROL 広告宣伝費]
* [!UICONTROL コンサルティング]
* [!UICONTROL 接待交際費]
* [!UICONTROL 一般]
* [!UICONTROL 部材費]
* [!UICONTROL 交通費]

## カスタム費用タイプを作成

{{step-1-to-setup}}

1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. **[!UICONTROL 新規費用タイプ]** をクリックします。
1. **[!UICONTROL 新規費用タイプ]** ダイアログボックスで、次の情報を入力します。

   * **名前** – 費用の名前。
   * **説明** – 費用の説明。
   * **計算単位** - ドロップダウンリストから費用タイプの測定単位を選択します。 次の単位の測定を使用できます。

      * マイル
      * キロメートル
      * キログラム
      * ドル
      * 時間
      * 日
      * その他 - このオプションを選択すると、測定単位に名前を付け、測定単位を組織にとってなじみのあるものとして定義するよう求められます。

   * **料金** – 単位あたりの価格。 これは通貨書式のフィールドで、「計算単位 **フィールドで設定された各単位のコストを表** ます。 レートには、小数点以下 4 桁までの数値を含めることができます。例えば、1.0375 と入力します。

1. 「**[!UICONTROL 保存]**」をクリックします。

   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

## カスタム費用タイプの変更

{{step-1-to-setup}}

1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. 変更する費用タイプを選択し、**[!UICONTROL 編集]** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

   **[!UICONTROL 費用タイプを編集]** ダイアログボックスが表示されます。

1. 必要な変更を加え、「**[!UICONTROL 保存]**」をクリックします。

   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

費用の使用方法とプロジェクトのコストに与える影響に関して詳しくは、「[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)」の記事を参照してください。
