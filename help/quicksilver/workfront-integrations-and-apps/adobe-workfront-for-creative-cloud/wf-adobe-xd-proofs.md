---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: XDアートボードを配達確認としてWorkfrontにアップロード
description: アートボードを配達確認としてAdobe Workfrontに直接アップロードし、詳細なレビューと承認を受けることができます。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 4a7fb18674b399b138fd981907f3a9da8e0bb30e
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# アップロード [!DNL XD] 配達確認としてのアートボード [!DNL Workfront]

アートボードを配達確認としてに直接アップロードできます。 [!DNL Adobe Workfront] 徹底的なレビューと承認を行う

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>現在のプラン：[!UICONTROL Pro] 以降</p> <p>または</p> <p>レガシープラン：[!UICONTROL Premium]</p> <p>様々なプランでのアクセス権の校正について詳しくは、を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>現在のプラン：[!UICONTROL Work] または [!UICONTROL Proof]</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>次が必要です： [!DNL Adobe Creative Cloud] に加えてライセンス [!DNL Workfront] ライセンス。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>[!UICONTROL Manager] 以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>[!UICONTROL ドキュメント ] へのアクセスの編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、役割、または配達確認権限プロファイルを確認するには、 [!DNL Workfront] または [!DNL Workfront Proof] 管理者。

## 前提条件

* 次をインストールする必要があります： [!DNL Adobe Workfront for XD] プラグインを使用して、配達確認をアップロードできるようにする [!DNL Adobe XD].

   手順については、 [インストール [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 静的配達確認のアップロード

1. 次をクリック： **[!UICONTROL メニュー]** アイコンをクリックし、「 **[!UICONTROL 作業用リスト]**. メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. 静的配達確認をアップロードする作業項目に移動します。
1. 次をクリック： **[!UICONTROL 文書]** アイコン ![](assets/documents.png) をクリックします。

1. クリック **[!UICONTROL 新規ファイル]** プラグインの下部付近にある。
1. アップロードするアートボードを選択します。

   >[!TIP]
   >
   >複数のアートボードを選択するには、目的のアートボード上でマウスをクリックしてドラッグします。

1. 有効にする **[!UICONTROL 配達確認の作成]**.

1. 配達確認に名前を付けます。

1. 目的の配達確認の承認の種類を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 基本 ]: </td> 
      <td> <p>基本的な承認プロセスはアドホックであり、必要に応じて様々なレビュー担当者を含めることができます。 </p> 
       <ul> 
        <li> <p>（オプション） <strong>承認者</strong> をクリックします。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自動 ]</td> 
      <td> <p>自動承認プロセスは、管理者が事前に作成し、特定のレビュー担当者とステージが含まれています。 詳しくは、 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動ワークフローの概要</a>.</p> 
       <ul> 
        <li> <p>ドロップダウンメニューから「 [!UICONTROL ワークフローテンプレート ] 」を選択します。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション） **[!UICONTROL 更新]** 領域

   ![](assets/proof-approvals-xd-350x396.png)

1. 書き出し形式を **[!UICONTROL アセットタイプ]** ドロップダウンメニュー。


1. （オプション）アセットタイプとして「PDF」を選択し、複数のアートボードを選択した場合は、アートボードを **[!UICONTROL 単一PDFファイル]s** または **M[!UICONTROL 複数のPDFファイル]**.

1. （オプション）PDFに名前を付けます。

   ![](assets/pdf-options.png)

1. クリック **[!UICONTROL アップロード]**.\
   ドキュメントが [!UICONTROL ドキュメント] 領域がプラグインおよびデスクトップアプリケーションに表示される問題を修正しました。

## インタラクティブな配達確認のアップロード {#upload-an-interactive-proof}

アートボードに対して、 [!DNL Workfront for Adobe] プラグイン。 これは 2 段階のプロセスです。 まず、インタラクティブリンクを作成してから、配達確認を作業項目にアップロードする必要があります。

### アートボード用のインタラクティブリンクの作成  {#create-an-interactive-link-for-your-art-board}

1. アートボードを開き、「 **[!UICONTROL 共有]** をクリックします。
1. リンク設定を指定します。

   1. リンクに名前を付けます。
   1. 表示設定を選択します。
   1. 内 **[!UICONTROL リンクアクセス]** セクション **[!UICONTROL このリンクを知っているすべてのユーザー]** が選択されている。

      インタラクティブな配達確認を生成するには、このタイプのアクセスを有効にする必要があります。

   1. クリック **[!UICONTROL リンクを作成]**.

1. 戻る **[!UICONTROL デザイン]** をクリックします。 次に進みます。 [インタラクティブな配達確認のアップロード](#upload-an-interactive-proof) 」の節を参照してください。

   >[!NOTE]
   >
   >画面の左下隅にあるプラグインパネルを再度開く必要が生じる場合があります。

### インタラクティブな配達確認のアップロード

1. 次をクリック： **[!UICONTROL メニュー]** アイコンをクリックし、「 **[!UICONTROL 作業用リスト]**. メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. インタラクティブ配達確認をアップロードする作業項目に移動します。
1. 次をクリック： **[!UICONTROL 文書]** アイコン ![](assets/documents.png) をクリックします。

1. クリック **[!UICONTROL 新規ファイル]** プラグインの下部付近にある。
1. 有効にする **[!UICONTROL 配達確認の作成]**.

1. 目的の配達確認の承認の種類を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 基本 ]: </td> 
      <td> <p>基本的な承認プロセスはアドホックであり、必要に応じて様々なレビュー担当者を含めることができます。 </p> 
       <ul> 
        <li> <p>（オプション） <strong>承認者</strong> をクリックします。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自動 ]</td> 
      <td> <p>自動承認プロセスは、管理者が事前に作成し、特定のレビュー担当者とステージが含まれています。 詳しくは、 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動ワークフローの概要</a>.</p> 
       <ul> 
        <li> <p>ドロップダウンメニューから「 [!UICONTROL ワークフローテンプレート ] 」を選択します。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション） **[!UICONTROL 更新]** 領域

   ![](assets/proof-approvals-xd-350x396.png)

1. 内 **[!UICONTROL アセットタイプ]** ドロップダウンメニューから、先ほど作成したリンクを **共有リンク** タブをクリックします。 詳しくは、 [アートボード用のインタラクティブリンクの作成](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. クリック **[!UICONTROL アップロード]**.

   ドキュメントが [!UICONTROL ドキュメント] 領域がプラグインおよびデスクトップアプリケーションに表示される問題を修正しました。

   >[!IMPORTANT]
   >
   >ユーザーは、 [!UICONTROL デスクトップ校正ビューア] インタラクティブな配達確認を確認および承認するには 詳しくは、 [のインストール [!UICONTROL デスクトップ校正ビューア]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## 新しい配達確認バージョンをアップロード

新しいバージョンの配達確認をアップロードできます。 このプラグインでは以前のバージョンで設定された校正ワークフローが記憶されますが、必要に応じて変更できます。

1. 次をクリック： **[!UICONTROL メニュー]** アイコンをクリックし、「 **[!UICONTROL 作業用リスト]**. メニューを使用して親オブジェクトに移動することもできます。

   ![](assets/menu-350x440.png)

1. ドキュメントのアップロード先の作業項目に移動します。
1. 次をクリック： **[!UICONTROL 文書]** アイコン ![](assets/documents.png)をクリックします。

1. クリック **[!UICONTROL 新しいバージョン]** プラグインの下部付近にある。
1. 有効にする **[!UICONTROL 配達確認の作成]**.
1. アップロードするアートボードを選択します。

   >[!NOTE]
   >
   >新しいバージョンの.svg、.png または.jpg をアップロードする場合は、1 つのアートボードのみをアップロードできます。

1. 目的の配達確認の承認の種類を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 基本 ]: </td> 
      <td> <p>基本的な承認プロセスはアドホックであり、必要に応じて様々なレビュー担当者を含めることができます。 </p> 
       <ul> 
        <li> <p>（オプション） <strong>承認者</strong> をクリックします。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自動 ]</td> 
      <td> <p>自動承認プロセスは、管理者が事前に作成し、特定のレビュー担当者とステージが含まれています。 詳しくは、 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動ワークフローの概要</a>.</p> 
       <ul> 
        <li> <p>ドロップダウンメニューから「 [!UICONTROL ワークフローテンプレート ] 」を選択します。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 書き出し形式を **[!UICONTROL アセットタイプ]** ドロップダウンメニュー。

   ![](assets/create-a-proof-xd-350x202.png)

1. （オプション） **[!UICONTROL 更新]** 領域

   ![](assets/proof-approvals-xd-350x396.png)

1. （オプション）アセットタイプとして「PDF」を選択し、複数のアートボードを選択した場合は、アートボードを **[!UICONTROL 単一PDFファイル]s** または **M[!UICONTROL 複数のPDFファイル]**.

1. （オプション）PDFに名前を付けます。

   ![](assets/pdf-options.png)

1. クリック **[!UICONTROL アップロード]**.\
   ドキュメントが [!UICONTROL ドキュメント] 領域がプラグインおよびデスクトップアプリケーションに表示される問題を修正しました。
