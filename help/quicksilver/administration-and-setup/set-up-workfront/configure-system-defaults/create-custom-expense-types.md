---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: カスタム経費タイプを作成
description: As a [!DNL Adobe Workfront] 管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。 費用は、タスクまたはプロジェクトに関連付けることができる非労務費です。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# カスタム経費タイプを作成

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

As a [!DNL Adobe Workfront] 管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。 費用は、タスクまたはプロジェクトに関連付けることができる非労務費です。

作成した費用タイプは、編集または削除できます。 組み込みの [!DNL Workfront] 費用タイプ。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## デフォルトの費用タイプ

に含まれる費用タイプ [!DNL Workfront] デフォルトでは、次の項目を含むを削除または編集することはできません。

* [!UICONTROL 広告宣伝費]
* [!UICONTROL コンサルティング]
* [!UICONTROL 接待交際費]
* [!UICONTROL 一般]
* [!UICONTROL 部材費]
* [!UICONTROL 交通費]

## カスタム経費タイプを作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront].
1. クリック **[!UICONTROL 費用タイプ]**.
1. クリック **[!UICONTROL 新しい費用タイプ]**.
1. 内 **[!UICONTROL 新しい費用タイプ]** 表示されるボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>費用の名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>費用の説明を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 計算単位 ]</td> 
      <td> <p>費用タイプの測定単位をドロップダウンリストから選択します。</p> <p>以下の測定単位を使用できます。</p> 
       <ul> 
        <li>マイル</li> 
        <li>キロメートル</li> 
        <li>キログラム</li> 
        <li>ドル</li> 
        <li>ドル</li> 
        <li>日</li> 
        <li>その他 — このオプションを選択すると、測定単位に名前を付け、測定単位を組織にとってなじみのあるものとして定義するよう求められます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">レート</td> 
      <td> <p>単位あたりの価格を指定します。 これは通貨形式のフィールドで、 <strong>[!UICONTROL 計算単位 ]</strong> フィールドに入力します。 </p> <p>レートには、小数点以下 4 桁までの数値を含めることができます。 例： 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 費用タイプを作成]**.\
   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

## カスタム費用タイプの変更

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront].
1. クリック **[!UICONTROL 費用タイプ]**.
1. 変更する費用タイプを選択し、「 **[!UICONTROL 編集]**.

   この **[!UICONTROL 費用タイプの編集]** ダイアログボックスが表示されます。

1. 必要な変更を加え、「 **[!UICONTROL 変更を保存]**.\
   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

費用の使用方法とプロジェクトのコストに与える影響の詳細については、「 [プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md).
