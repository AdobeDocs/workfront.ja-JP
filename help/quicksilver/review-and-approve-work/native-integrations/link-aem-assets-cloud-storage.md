---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Experience Manager Assetsのコンテンツとフォルダーを、Adobe クラウドストレージとリンクします
description: 組織でAdobe クラウドストレージを使用している場合は、Experience Manager Assetsのコンテンツとフォルダーを、ドキュメントをサポートする任意のAdobe Workfront オブジェクトにリンクできます。
author: Courtney
source-git-commit: 66635b2edc78833ec2d08cef382b39b89238b565
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 12%

---

# Experience Manager Assetsのコンテンツとフォルダーを、Adobe クラウドストレージとリンクします

Adobe クラウドストレージを使用している場合は、Experience Manager AssetsからWorkfrontにコンテンツとフォルダーをリンクできます。 リンクすると、Workfrontでコンテンツを表示および管理でき、Experience Manager Assetsでコンテンツに加えられた変更はWorkfrontに反映されます。

>[!IMPORTANT]
>
>組織がGenAI Rider契約への署名を拒否した場合でも、Content Advisorを使用してExperience Manager Assetsのアセットとフォルダーを選択できますが、AI 検索、スマートレコメンデーション、キャンペーンブリーフの分析など、AIを活用した機能にはアクセスできません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>コントリビューター以上</p> 
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">その他の製品</td> 
   <td>Experience Manager as a Cloud Serviceが必要であり、Admin Consoleのユーザーとして商品に追加する必要があります。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 権限</td> 
    <td>フォルダーへの書き込みアクセス権が必要です。</td> 
   </tr>
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示アクセス権またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

開始する前の確認事項。

* Workfront 管理者は、Experience Manager 統合を設定する必要があります。 詳しくは、[Frame.io 統合した Adobe Experience Manager の使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)を参照してください。

* スマート提案またはキャンペーンブリーフ機能を使用するには、GenAI ライダーに署名する必要があります。 詳しくは、[Adobe アプリケーションでContent Advisorを使用してAEM コンテンツにアクセスする](https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)を参照してください。

## Experience Manager Assetsからコンテンツをリンクする

コンテンツをリンクするには：

1. コンテンツをリンクするWorkfront オブジェクトに移動します。
1. 左側のパネルで「**ドキュメント**」セクションをクリックします。
1. ページの右側にある&#x200B;**新規**&#x200B;をクリックし、**AEM ファイル**&#x200B;をクリックして個々のアセットをリンクします。
   ![AEM ファイルをドキュメント領域に追加](assets/aem-files.png)

1. Content Advisorを使用すると、次のことが可能になります。

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>AI 検索を使用してアセットを検索します。</strong> AIを利用した検索により、クエリの背後にある意味や意図を理解し、複数の言語、タイプミス、類義語をサポートできます。</td>
         <td>詳しくは、「<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">よりスマートなアセット検出のためのAI 検索</a>」を参照してください。</td>
      </tr>
      <tr>
         <td><strong> コンテキストと意図に基づいてスマート提案を表示します。</strong> ホストのAdobeアプリケーションからコンテキストに応じたレコメンデーションを使用して、コンテンツのニーズに合ったアセットを見つけることができます。</td>
         <td>詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor"> コンテキストとインテントに基づくスマート提案</a>を参照してください。</td>
      </tr>
      <tr>
         <td><strong> キャンペーン概要をアップロードして、関連するアセットを見つけます。</strong> PDF、DOCX、TXTのキャンペーンブリーフドキュメントをアップロードして、Content Advisorが分析し、関連アセットを提案できるようにします。</td>
         <td>詳細については、<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor"> キャンペーン概要を参照して、関連するアセットを見つけてください</a>。</td>
      </tr>
      <tr>
         <td><strong>Dynamic Media アセットのレンディションを表示して選択します。</strong> 画像プリセット、スマート切り抜き、フォーマットタイプなど、チャネルに合わせて最適化されたレンディションを参照し、Dynamic Media修飾子を適用して調整をリアルタイムでプレビューします。</td>
         <td>詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">使用できるDynamic Media アセットのレンディション </a>を参照してください。</td>
      </tr>
      <tr>
         <td><strong> レンディションにDynamic Media修飾子を適用します。</strong> 修飾子を追加してアセットレンディションをリアルタイムで変換し、結果をプレビューしてから、ホストアプリケーションのレンディションを選択します。</td>
         <td>詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">使用できるDynamic Media アセットのレンディション </a>を参照してください。</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong> アセットのメタデータにアクセスします。</strong> Assetsのビューと一致するタイトル、説明、フォーマット、サイズ、その他のメタデータタブ（商品、キャンペーン、タグ）などのアセットのプロパティを確認できます。</td>
         <td>詳しくは、「<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Assets ビューと一致したアセットメタデータへのアクセス </a>」を参照してください。</td>
      </tr>
      <tr>
         <td><strong>定義済みフィルターを使用してアセットをフィルタリングします。</strong> ファイルタイプ、ファイル形式、アセットステータス、ファイルサイズ、画像の幅、画像の高さ、変更日、作成日などのフィルターを使用して、アセットの結果を調整します。</td>
         <td>詳しくは、「<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Assets ビューと一致するフィルターへのアクセス </a>」を参照してください。</td>
      </tr>
      <tr>
         <td><strong>検索を保存して再利用します。</strong> 検索語とフィルターオプションを指定して保存した検索を作成し、Experience Manager Assetsやその他のAdobe アプリケーションで再利用できます。</td>
         <td>詳細については、<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">最近の検索と保存された検索のアクセスと再利用</a>を参照してください。</td>
      </tr>
      <tr>
         <td><strong> コレクション間およびコレクション内のアセットを検索します。</strong> すべてのコレクションでアセットまたはコレクションを検索するか、特定のコレクションに検索を制限します。</td>
         <td>詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor"> コレクション間およびコレクション内のアセットの検索</a>を参照してください。</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >Content Advisorの「おすすめコンテンツ」では、次のデータを使用して、Workfrontで提案されたコンテンツを決定します。
   >
   >* Workfront オブジェクトの名前フィールドと説明フィールド
   >* 必須としてマークされたカスタムフォームフィールド
   >* 添付ドキュメントからのデータ

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## 考慮事項

* リンクされたAEM アセットでは、レビューと承認ワークフローはサポートされていません。
* メタデータフィールドは、WorkfrontからExperience Manager Assetsにアセットを送信するときに最初にマッピングされます。 Workfront 管理者がオブジェクトメタデータの同期を有効にしている場合、どちらかのアプリケーションで変更されたフィールドは最新の状態に保たれます。
