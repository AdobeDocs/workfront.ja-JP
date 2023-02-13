---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: XDアートボードをドキュメントとしてWorkfrontにアップロード
description: アートボードをドキュメントとしてアップロードして、すばやいレビューや承認を得たり、Adobe Workfrontに保存するだけで済みます。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# アップロード [!DNL XD] ～への書類としてのアートボード [!DNL Workfront]

アートボードをドキュメントとしてアップロードして、すばやいレビューや承認を得ることも、単ににに保存することもできます。 [!DNL Adobe Workfront].

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
   <td>次が必要です： [!DNL Adobe Creative Cloud] に加えてライセンス [!DNL Workfront] ライセンス。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!UICONTROL ドキュメント ] へのアクセスの編集</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>[!UICONTROL 表示 ] ドキュメントをアップロードするオブジェクトに対する [!UICONTROL 表示 ] アクセス権以上。</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

* 次をインストールする必要があります： [!DNL Adobe Workfront for XD] プラグインを使用して、XD art boards をドキュメントとしてWorkfrontにアップロードする必要があります。

手順については、 [インストール [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 新しいドキュメントを追加

1. 次をクリック： **[!UICONTROL メニュー]** アイコンをクリックし、「 **[!UICONTROL 作業用リスト]**. メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. ドキュメントをアップロードする作業項目に移動します。
1. 次をクリック： **[!UICONTROL 文書]** アイコン ![](assets/documents.png) をクリックします。

1. クリック **[!UICONTROL 新規ファイル]** プラグインの下部付近にある。
1. アップロードするアートボードを選択します。

   >[!TIP]
   >
   >複数のアートボードを選択するには、目的のアートボード上でマウスをクリックしてドラッグします。
1. （オプション） **[!UICONTROL 更新]** 領域
1. を選択します。 **[!UICONTROL アセットタイプ]** ドロップダウンメニューから、次の操作を実行します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL 書き出し形式 ]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>アートボードは、PNG として作業項目の「[!UICONTROL ドキュメント ]」タブにアップロードされます。 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>アートボードは、JPGとして [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>アートボードは、SVGとして [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>選択したアートボードを <strong>単一PDFファイル</strong> または <strong>複数のPDFファイル</strong>. アートボードは、作業項目の [!UICONTROL ドキュメント ] タブにPDFとしてアップロードします ( [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. クリック **[!UICONTROL アップロード]**.\
   ドキュメントが [!UICONTROL ドキュメント] 領域がプラグインおよびデスクトップアプリケーションに表示される問題を修正しました。

## 新しいバージョンを追加

1. 次をクリック： **[!UICONTROL メニュー]** アイコンをクリックし、「 **[!UICONTROL 作業用リスト]**. メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. ドキュメントをアップロードする作業項目に移動します。
1. 次をクリック： **[!UICONTROL 文書]** アイコン ![](assets/documents.png)をクリックします。

1. 新しいバージョンを追加するドキュメントをクリックします。
1. クリック **[!UICONTROL 新しいバージョン]** プラグインの下部付近にある。
1. アップロードするアートボードを選択します。

   >[!NOTE]
   >
   >新しいバージョンのSVG、PNG、JPGをアップロードする場合は、1 つのアートボードのみをアップロードできます。

1. （オプション） **[!UICONTROL 更新]** 領域

1. を選択します。 **[!UICONTROL アセットタイプ]** ドロップダウンメニューから、次の操作を実行します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">書き出し形式</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>アートボードは、PNG 形式で作業項目の「[!UICONTROL ドキュメント ]」タブにアップロードします。 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>アートボードは、作業項目の [!UICONTROL ドキュメント ] タブにJPGとしてアップロードします ( [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>アートボードは、作業項目の「[!UICONTROL ドキュメント ]」タブにSVGとしてアップロードします ( [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>アートボードは、PDFとして [!DNL Workfront].</p>
      <p><strong>注意</strong>:新しいドキュメントバージョン用にアップロードできるアートボードは 1 つだけです。</p>
      </td>
     </tr>
    </tbody>
   </table>

1. クリック **[!UICONTROL アップロード]**.\
   ドキュメントが [!UICONTROL ドキュメント] 領域がプラグインおよびデスクトップアプリケーションに表示される問題を修正しました。
