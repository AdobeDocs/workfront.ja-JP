---
title: ドキュメント統合の設定
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Adobe Workfrontの管理者は、Workfrontでドキュメントを管理するためのドキュメント統合を設定できます。
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 84%

---

# ドキュメント統合の設定

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

[!DNL Adobe Workfront] 管理者は、ドキュメント統合を設定して、[!UICONTROL Workfront] でドキュメントを管理できます。また、[!UICONTROL Workfront] は、ドキュメントがドキュメントサービスアプリケーションにのみ保存され、[!UICONTROL Workfront] には保存されないように設定することもできます。詳しくは、[外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)の[[!UICONTROL Workfront] のドキュメントを外部クラウドプロバイダーに更新しリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider)を参照してください。

>[!NOTE]
>
>[!DNL Workfront Proof] と [!DNL Workfront] サーバーの間のオープン通信を許可するには、特定の IP アドレスを許可リストに追加することが必要になる場合があります。詳しくは、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

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
   <td><p>新規： [!UICONTROL Standard]</p>
       <p>または</p>
       <p>現在： [!UICONTROL プラン ]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## サポートされている統合

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

ドキュメント管理用に次の統合を設定できます。

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  [!DNL Workfront Proof] からプルーフをリンクすると、最初に [!DNL Workfront Proof] 内で作成されたプルーフを、[!DNL Workfront] 内で使用可能にすることができます。現在のプランの場合、 [!UICONTROL Pro] [!DNL Workfront] この機能を使用するには、プラン以降が必要です。 新しいプランでは、この機能はすべてのプランで使用できます。 利用可能な様々なプランについて詳しくは、[Workfront プラン](https://www.workfront.com/plans)を参照してください。

* [!DNL Microsoft SharePoint]

  [!DNL SharePoint] との統合について詳しくは、[ [!DNL SharePoint]  統合を設定](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md)を参照してください。

* サードパーティクラウドドキュメントプロバイダー：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

     <!--Quip-->
  >[!TIP]
  >
  >[!DNL Workfront] に直接アップロードされたドキュメントのプルーフおよび承認と同じ方法で、外部クラウドプロバイダーからリンクされたドキュメントのプルーフや承認を行うことができます。

* その他のドキュメントプロバイダー（カスタムドキュメント統合を通じて）。

  現在のプランの場合、 [!UICONTROL Pro] [!DNL Workfront] この機能を使用するには、プラン以降が必要です。 新しいプランでは、この機能はすべてのプランで使用できます。 利用可能な様々なプランについて詳しくは、[Workfront プラン](https://www.workfront.com/plans)を参照してください。

さらに、[!DNL Workfront] ドキュメントのエクスペリエンスを、ネイティブのデジタルアセット管理（DAM）システムまたはサードパーティの DAM 統合で強化することもできます。ユーザーがサービスを自分の [!DNL Workfront] アカウントにリンクするために、管理者がこれらの機能を有効にする必要があります。Workfront DAM について詳しくは、[ [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md) を使用したドキュメントの管理を参照してください。

## ドキュメントを管理するための統合の設定

{{step-1-to-setup}}

1. 左側のパネルで「**[!UICONTROL ドキュメント]**」をクリックし、「**[!UICONTROL クラウドプロバイダー]」を選択します。**

1. （オプション）ドキュメントを [!DNL Workfront] ではなくドキュメントサービスアプリケーションに保存するには、「**[!UICONTROL ユーザーに [!DNL Workfront]] でドキュメントを保存させない**」を選択します。

1. 有効にする統合を選択します。
1. 「**[!UICONTROL 保存]**」をクリックします。

[!DNL Workfront DAM] との統合を設定している場合は、ドキュメントにメタデータを含めることができるように [!DNL Workfront] を設定できます。メタデータのマッピングについて詳しくは、[メタデータマッピングの設定](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md)を参照してください。

## カスタムドキュメント統合の設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

カスタムドキュメント統合により、[!DNL Workfront] ユーザーは、[!DNL Workfront] に対応するようになっているシステムであれば、ほぼどのシステムからでも [!DNL Workfront] にファイルをリンクすることができます。

カスタム統合をユーザーが使用できるようにするには、まず統合を作成する必要があります。[!DNL Workfront] で使用する統合の作成方法について詳しくは、[ドキュメント web フック API](../../wf-api/doc-wbhks-api/docu-webhook-api.md) を参照してください。

カスタムドキュメント統合は、作成後、サイト上のユーザーが使用できるようにすることができます。

{{step-1-to-setup}}

1. 左側のパネルで、 **[!UICONTROL ドキュメント]** > **[!UICONTROL カスタム統合]**.

1. 「**[!UICONTROL カスタム統合を追加]**」をクリックします。
1. 統合を設定するには、次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>カスタム統合の名前。Workfront 内で統合を使用する際に、ユーザーに表示される名前です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>API 呼び出し用のベース HTTP またはセキュア HTTP URL。例： <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>カスタム統合に対して認証済みの API 呼び出しを行う際に使用する認証方法。</p> 
       <ul> 
        <li><strong>[!UICONTROL OAuth]</strong> を選択した場合は、手順 5 に進みます。</li> 
        <li><strong>[!UICONTROL ApiKey]</strong> を選択した場合は、手順 6 に進みます。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）選択した場合、 **[!UICONTROL OAuth]** 認証 **[!UICONTROL 認証タイプ]**、次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>ユーザー認証に使用する完全な URL。[!DNL Workfront] は、OAuth プロビジョニングプロセスの一環として、ユーザーをこのアドレスに移動します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>OAuth トークンの取得に使用される完全な API の URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>この統合用の OAut クライアント ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>この統合用の OAut クライアントシークレット。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Parameters]</td> 
      <td> <p>すべての API 呼び出しのクエリ文字列に追加するオプションの値を入力します。 例えば、access_type=offline など。</p> <p>複数のリクエストパラメーターを追加するには、「<strong>+ リクエストパラメーターを追加</strong>」をクリックします。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >[!UICONTROL カスタム統合]ページの下部に表示される [!DNL Workfront] リダイレクト URIに、この統合を外部のドキュメントプロバイダーに登録するのに使用される URI が表示されます。

1. （条件付き）選択した場合、 **[!UICONTROL ApiKey]** 認証 **[!UICONTROL 認証タイプ]**、カスタムドキュメントプロバイダーによって発行された API キーを入力します。

   [!DNL Workfront] はこの API キーを使用して、ドキュメントプロバイダーに対する認証済みの API 呼び出しを行います。

1. 「**[!UICONTROL 保存]**」をクリックして統合を作成します。

## ドキュメント統合を使用

[!DNL Workfront DAM] の使用法については、[ [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md)を使用したドキュメントの管理を参照してください。

プルーフの使用法については、[プルーフを作成](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md)を参照してください。

サードパーティのドキュメント統合の設定後にその統合を使用する方法については、[外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

### [!UICONTROL [!DNL Workfront] DAM] にメタデータを送信するように [!DNL Workfront] を設定 {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

[!DNL Workfront] から [!DNL Workfront DAM] にドキュメントを送信する場合、そのドキュメントに関連する情報も送信することができます。ドキュメントに関する情報は、[!DNL Workfront DAM] にメタデータとしてマッピングされます。

情報は、[!DNL Workfront] から [!DNL Workfront DAM] への一方向でのみマッピングされ、ドキュメントが [!DNL Workfront DAM] にアップロードされたときにのみ転送されます。ドキュメントが既にアップロードされている場合は、その後 Workfront フィールドに変更を加えても、[!DNL Workfront DAM] のメタフィールドは更新されません。\
様々な [!DNL Workfront DAM] フィールドに同じ [!DNL Workfront] フィールドをマッピングできますが、複数の [!DNL Workfront] フィールドに同じ [!DNL Workfront DAM] フィールドを使用することはできません。

1 つの [!DNL Workfront DAM] フィールドに書き出すように複数の [!DNL Workfront] フィールドを設定する必要がある場合は、まず [!DNL Workfront] に計算カスタムフィールドを作成して、オブジェクトの個々のカスタムフィールドをすべて表示します。次に、1 つの [!DNL Workfront DAM] フィールドに計算 [!DNL Workfront] フィールドをマッピングします。\
計算カスタムフィールドについて詳しくは、[カスタムフォームに計算データを追加](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)を参照してください。

マッピングは、任意のユーザーが [!DNL Workfront] から [!UICONTROL Workfront] DAM にアップロードしたすべてのドキュメントに影響します。

As a [!DNL Workfront] 管理者、有効にする必要があります [!DNL Workfront DAM] Workfrontで、メタデータマッピングプロセスのフィールドをマッピングする前に行ってください。

メタデータを [!DNL Workfront DAM] に送信するように [!DNL Workfront] を設定するには、次の手順を実行します。

{{step-1-to-setup}}

1. **[!UICONTROL ドキュメント]**／**[!UICONTROL メタデータ マッピング]**&#x200B;をクリックします。

1. 「**[!UICONTROL マッピングのソース フィールドを選択]**」フィールドで、[!DNL Workfront DAM] にマッピングする Workfront フィールドの名前を途中まで入力し、名前がリストに表示されたらそれを選択します。
1. 「**[!UICONTROL マッピングのターゲット フィールドを選択]**」で、選択した [!DNL Workfront] フィールドの情報を入力する [!DNL Workfront DAM] フィールドを選択します。

   >[!NOTE]
   >
   > 権限を持つユーザーによって [!DNL Workfront DAM] に送信されるすべてのドキュメントで、[!DNL Workfront DAM] へのアップロード時にここでマッピングされた [!DNL Workfront] フィールドでメタデータが更新されます。

1. 「**[!UICONTROL マッピングを追加]**」をクリックします。

1. [!UICONTROL Workfront] フィールドと対応する [!DNL Workfront DAM] フィールドの追加をさらに続けます。

### マッピングされたフィールドを削除

{{step-1-to-setup}}

1. 「**[!UICONTROL ドキュメント]**」を展開し、「**[!UICONTROL メタデータ マッピング]**」をクリックします。

1. フィールドのリストで、メタデータマッピングから削除するフィールドを選択します。
1. 「**[!UICONTROL 削除]**」をクリックします。

   フィールドがメタデータマッピングから削除され、フィールドに含まれていた情報は、アップロードされたドキュメントと共には [!DNL Workfront DAM] に転送されません。
