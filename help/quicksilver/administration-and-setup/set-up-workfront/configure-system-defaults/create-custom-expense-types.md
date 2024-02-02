---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: カスタム費用タイプを作成
description: ' [!DNL Adobe Workfront]  管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: ht
source-wordcount: '438'
ht-degree: 100%

---

# カスタム費用タイプを作成

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。

作成した費用タイプは、編集や削除することができます。組み込みの [!DNL Workfront] 費用タイプは、削除したり編集したりすることができません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## デフォルトの費用タイプ

デフォルトで [!DNL Workfront] に含まれる費用タイプは、次の項目を含み、削除したり編集したりすることができません。

* [!UICONTROL 広告宣伝費]
* [!UICONTROL コンサルティング]
* [!UICONTROL 接待交際費]
* [!UICONTROL 一般]
* [!UICONTROL 部材費]
* [!UICONTROL 交通費]

## カスタム費用タイプを作成

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。
1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. 「**[!UICONTROL 新規費用タイプ]**」をクリックします。
1. 表示される「**[!UICONTROL 新規費用タイプ]**」ボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>費用の名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>費用の説明を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>費用タイプの測定単位をドロップダウンリストから選択します。</p> <p>以下の測定単位が使用できます。</p> 
       <ul> 
        <li>マイル</li> 
        <li>キロメートル</li> 
        <li>キログラム</li> 
        <li>ドル</li> 
        <li>ドル</li> 
        <li>日</li> 
        <li>その他 - このオプションを選択すると、測定単位に名前を付け、測定単位を組織にとってなじみのあるものとして定義するよう求められます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">レート</td> 
      <td> <p>単位あたりの価格を指定します。これは通貨形式のフィールドで、<strong>[!UICONTROL Calculated Unit]</strong>フィールドで確立された各ユニットのコストを表します。 </p> <p>レートには、小数点以下 4 桁までの数値を含めることができます。例えば、1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 費用タイプの作成]**」をクリックします。\
   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

## カスタム費用タイプを変更

1. [!DNL Adobe Workfront] の右上隅にある **[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。
1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. 変更する費用タイプを選択してから、「**[!UICONTROL 編集]**」をクリックします。

   **[!UICONTROL 費用タイプの編集]**&#x200B;ダイアログボックスが表示されます。

1. 必要な変更を加え、「**[!UICONTROL 変更を保存]**」をクリックします。\
   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

費用の使用方法とプロジェクトのコストに与える影響に関して詳しくは、「[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)」の記事を参照してください。
