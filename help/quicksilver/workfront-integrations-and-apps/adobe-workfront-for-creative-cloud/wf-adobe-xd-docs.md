---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: XD アートボードをドキュメントとして Workfront にアップロード
description: アートボードをドキュメントとしてアップロードすると、素早くレビューや承認を行ったり、単に Adobe Workfront に保存することができます。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: ht
source-wordcount: '577'
ht-degree: 100%

---


# [!DNL XD] アートボードをドキュメントとして [!DNL Workfront] にアップロード

アートボードをドキュメントとしてアップロードすると、素早くレビューや承認を行ったり、単に [!DNL Adobe Workfront] に保存したりすることができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">製品</td> 
   <td>[!DNL Workfront] ライセンスに加えて [!DNL Adobe Creative Cloud] ライセンスが必要です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!UICONTROL Documents]の編集権限</p> <p>まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントをアップロードするオブジェクトに対する [!UICONTROL View] アクセス権以上。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

* XD アートボードをドキュメントとして Workfront にアップロードする前に、[!DNL Adobe Workfront for XD] プラグインをインストールする必要があります。

手順については、[インストール [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md)を参照してください。

## 新しいドキュメントを追加

1. 右上隅にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL ワークリスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. ドキュメントをアップロードする作業アイテムに移動します。
1. ナビゲーションバーの&#x200B;**[!UICONTROL ドキュメント]**&#x200B;アイコン ![](assets/documents.png) をクリックします。

1. プラグインの下部近くにある「**[!UICONTROL 新規ファイル]**」をクリックします。
1. アップロードするアートボードを選択します。

   >[!TIP]
   >
   >複数のアートボードを選択するには、目的のアートボード上でマウスをクリックしてドラッグします。
1. （オプション）**[!UICONTROL アップデート]**&#x200B;エリアにコメントを入力します。
1. ドロップダウンメニューから「**[!UICONTROL アセットタイプ]**」を選択します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Export Format]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>アートボードは、PNG として [!DNL Workfront] にある作業アイテムの「[!UICONTROL Documents]」タブにアップロードされます。 </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>アートボードは、PNG として [!DNL Workfront] にある作業アイテムの「[!UICONTROL Documents]」タブにアップロードされます。 <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>アートボードは、SVG として [!DNL Workfront] にある作業アイテムの「[!UICONTROL Documents]」タブにアップロードされます。 </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>選択したアートボードを<strong>単一 PDF ファイル</strong>または<strong>複数の PDF ファイル</strong>としてアップロードするかどうかを選択します。アートボードは、PDF として [!DNL Workfront] にある作業項目の「[!UICONTROL Documents]」タブにアップロードされます。</td>
     </tr>
    </tbody>
   </table>


1. 「**[!UICONTROL アップロード]**」をクリックします。\
   ドキュメントが、プラグインとデスクトップアプリの[!UICONTROL ドキュメント]エリアに表示されます。

## 新しいバージョンを追加

1. 右上隅にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL ワークリスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. ドキュメントをアップロードする作業アイテムに移動します。
1. ナビゲーションバーの&#x200B;**[!UICONTROL ドキュメント]**&#x200B;アイコン ![](assets/documents.png) をクリックします。

1. 新しいバージョンを追加するドキュメントをクリックします。
1. プラグインの下部近くにある「**[!UICONTROL 新しいバージョン]**」をクリックします。
1. アップロードするアートボードを選択します。

   >[!NOTE]
   >
   >新しいバージョンの SVG、PNG、JPG をアップロードする場合は、1 つのアートボードのみをアップロードできます。

1. （オプション）**[!UICONTROL アップデート]**&#x200B;エリアにコメントを入力します。

1. ドロップダウンメニューから「**[!UICONTROL アセットタイプ]**」を選択します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">書き出し形式</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>アートボードは、[!DNL Workfront] の作業アイテムの「[!UICONTROL Documents]」タブに PNG としてアップロードします。 </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>アートボードは、[!DNL Workfront] の作業アイテムの 「[!UICONTROL Documents]」タブに JPG としてアップロードします。 <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>アートボードは、[!DNL Workfront] の作業アイテムの「[!UICONTROL Documents]」タブに SVG としてアップロードします。 </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>アートボードは、[!DNL Workfront] の作業アイテムの「[!UICONTROL Documents]」タブに PDF としてアップロードします。</p>
      <p><strong>メモ</strong>：新しいドキュメントバージョン用にアップロードできるアートボードは 1 つだけです。</p>
      </td>
     </tr>
    </tbody>
   </table>

1. 「**[!UICONTROL アップロード]**」をクリックします。\
   ドキュメントが、プラグインおよびデスクトップアプリケーションの[!UICONTROL ドキュメント]エリアに表示されます。
