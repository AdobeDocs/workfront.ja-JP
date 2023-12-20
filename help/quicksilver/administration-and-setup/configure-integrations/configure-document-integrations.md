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
source-git-commit: ae063189eebb17a3341aabb978ee0f0e03d1e299
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 1%

---

# ドキュメント統合の設定

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

As an [!DNL Adobe Workfront] 管理者は、ドキュメント統合を設定して、 [!UICONTROL Workfront]. また、 [!UICONTROL Workfront] そのため、ドキュメントは、ドキュメントサービスアプリケーションにのみ保存され、には保存されません。 [!UICONTROL Workfront] それ自体。 詳しくは、 [ドキュメントの更新とリンク元 [!UICONTROL Workfront] 外部クラウドプロバイダーに](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>次の間のオープン通信を許可する： [!DNL Workfront Proof] そして [!DNL Workfront] サーバーの場合は、特定の IP アドレスをサーバーに追加する必要がある場合があ許可リストに加えるります。 詳しくは、 [ファイアウォールの設定を許可リストに加える行う](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

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
   <td><p>新規： [!UICONTROL Standard]</p>
       <p>または</p>
       <p>現在： [!UICONTROL プラン ]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## サポートされる統合

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

ドキュメント管理用に次の統合を設定できます。

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  配達確認のリンク元 [!DNL Workfront Proof] では、最初に [!DNL Workfront Proof] 以内で使用可能 [!DNL Workfront]. 現在のプランの場合、 [!UICONTROL Pro] [!DNL Workfront] この機能を使用するには、プラン以降が必要です。 新しいプランでは、この機能はすべてのプランで使用できます。 利用可能な様々なプランについて詳しくは、 [Workfront Plans](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  との統合について詳しくは、 [!DNL SharePoint]を参照してください。 [を設定します。 [!DNL SharePoint] 統合](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* サードパーティのクラウドドキュメントプロバイダー：

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
  >外部クラウドプロバイダーからリンクされたドキュメントの配達確認や承認を、に直接アップロードされたドキュメントの配達確認や承認と同じ方法でおこなうことができます。 [!DNL Workfront].

* 他のドキュメントプロバイダー（カスタムドキュメント統合を通じて）。

  現在のプランの場合、 [!UICONTROL Pro] [!DNL Workfront] この機能を使用するには、プラン以降が必要です。 新しいプランでは、この機能はすべてのプランで使用できます。 利用可能な様々なプランについて詳しくは、 [Workfront Plans](https://www.workfront.com/plans).

さらに、 [!DNL Workfront] ネイティブの Digital Asset Management(DAM) システムやサードパーティの DAM 統合を使用したドキュメントエクスペリエンス。 ユーザーがサービスを自分のユーザーにリンクするには、管理者がこれらの機能を有効にする必要があります [!DNL Workfront] アカウント。 Workfront DAM について詳しくは、 [を使用したドキュメントの管理 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## ドキュメントを管理するための統合の設定

{{step-1-to-setup}}

1. 左側のパネルで、 **[!UICONTROL ドキュメント]** > **[!UICONTROL クラウドプロバイダー].**

1. （オプション）ドキュメントをドキュメントサービスのアプリケーションに保存し、に保存しない場合 [!DNL Workfront]を選択します。 **[!UICONTROL ユーザーがにドキュメントを保存できないようにする [!DNL Workfront]].**

1. 有効にする統合を選択します。
1. 「**[!UICONTROL 保存]**」をクリックします。

との統合を設定している場合 [!DNL Workfront DAM]を有効にすると、 [!DNL Workfront] メタデータをドキュメントに含めるには メタデータのマッピングについて詳しくは、 [メタデータマッピングの設定](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## カスタムドキュメント統合の設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

カスタムドキュメントの統合により、 [!DNL Workfront] ファイルをリンクするユーザー [!DNL Workfront] システムがと連携するように設定されている場合、ほぼすべてのシステムから [!DNL Workfront].

カスタム統合をユーザーが使用できるようにするには、まず統合を構築する必要があります。 と共に使用する統合の作成方法に関する情報 [!DNL Workfront]を参照してください。 [Document Webhook API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

カスタムドキュメントの統合を構築した後、サイト上のユーザーが使用できるようにします。

{{step-1-to-setup}}

1. 左側のパネルで、 **[!UICONTROL ドキュメント]** > **[!UICONTROL カスタム統合]**.

1. クリック **[!UICONTROL カスタム統合の追加]**.
1. 統合を設定するには、次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>カスタム統合の名前。 Workfront内で統合を使用すると、ユーザーに表示される名前です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>API 呼び出しのベース HTTP またはセキュア HTTP URL。 以下に例を挙げます。 <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 認証タイプ ]</td> 
      <td> <p>カスタム統合に対して認証済みの API 呼び出しをおこなう際に使用する認証方法。</p> 
       <ul> 
        <li>次を選択した場合： <strong>[!UICONTROL OAuth]</strong>、手順 5 に進みます。</li> 
        <li>次を選択した場合： <strong>[!UICONTROL Api キー ]</strong>で、手順 6 に進みます。</li> 
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
      <td role="rowheader">[!UICONTROL 認証 URL]</td> 
      <td>ユーザー認証に使用する完全な URL。 [!DNL Workfront] OAuth プロビジョニングプロセスの一環として、ユーザーをこのアドレスに移動します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL トークンエンドポイント URL]</td> 
      <td>OAuth トークンの取得に使用される完全な API の URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID]</td> 
      <td>この統合の OAut クライアント ID です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td> 
      <td>この統合の OAut クライアント秘密鍵。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL リクエストパラメーター ]</td> 
      <td> <p>すべての API 呼び出しのクエリ文字列に追加するオプションの値を入力します。 例えば、 access_type=offline とします。</p> <p>複数のリクエストパラメーターを追加するには、 <strong>+リクエストパラメーターの追加</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >The [!DNL Workfront] の下部に表示されるリダイレクト URI [!UICONTROL カスタム統合] page は、この統合を外部のドキュメントプロバイダーに登録するために使用される URI をリストします。

1. （条件付き）選択した場合、 **[!UICONTROL ApiKey]** 認証 **[!UICONTROL 認証タイプ]**、カスタムドキュメントプロバイダーによって発行された API キーを入力します。

   [!DNL Workfront] はこの API キーを使用して、ドキュメントプロバイダーに対する認証済みの API 呼び出しをおこないます。

1. クリック **[!UICONTROL 保存]** をクリックして統合を作成します。

## ドキュメント統合の使用

ユーザーが [!DNL Workfront DAM]を参照してください。 [を使用したドキュメントの管理 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

ユーザーによる校正機能の使い方について詳しくは、 [配達確認の作成](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

設定後にサードパーティのドキュメント統合をユーザーが使用する方法について詳しくは、 [外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 設定 [!DNL Workfront] メタデータの送信先 [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

からドキュメントを送信する際 [!DNL Workfront] から [!DNL Workfront DAM]を使用すると、そのドキュメントに関連する情報を送信することもできます。 ドキュメントに関する情報のマッピング先 [!DNL Workfront DAM] メタデータとして。

情報は、次から一方向にのみマッピングされます： [!DNL Workfront] から [!DNL Workfront DAM] そして、ドキュメントが [!DNL Workfront DAM]. 今後Workfrontフィールドに変更を加えても、 [!DNL Workfront DAM] ドキュメントが既にアップロードされた後。\
同じ [!DNL Workfront] ～の種々の分野に属する [!DNL Workfront DAM] フィールドに値を入力する必要がありますが、同じ値を使用することはできません [!DNL Workfront DAM] 複数のフィールド [!DNL Workfront] フィールド。

複数の [!DNL Workfront] 1 つに書き出すフィールド [!DNL Workfront DAM] フィールドに値を入力する場合は、まず [!DNL Workfront] をクリックして、オブジェクトの個々のカスタムフィールドをすべて表示します。 次に、計算指標 [!DNL Workfront] 1 つのフィールド [!DNL Workfront DAM] フィールドに入力します。\
計算カスタムフィールドの詳細については、 [計算データをカスタムフォームに追加する](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

マッピングは、任意のユーザーがからアップロードしたすべてのドキュメントに影響します。 [!DNL Workfront] から [!UICONTROL Workfront] DAM.

As a [!DNL Workfront] 管理者、有効にする必要があります [!DNL Workfront DAM] Workfrontで、メタデータマッピングプロセスのフィールドをマッピングする前に行ってください。

を設定するには、以下を実行します。 [!DNL Workfront] メタデータの送信先 [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. クリック **[!UICONTROL ドキュメント]** > **[!UICONTROL メタデータマッピング]**.

1. Adobe Analytics の **[!UICONTROL マッピングのソースフィールドを選択]** フィールドに、マッピング先のWorkfrontフィールドの名前を入力します [!DNL Workfront DAM]をクリックし、リストに表示されたら選択します。
1. Adobe Analytics の **[!UICONTROL マッピングのターゲットフィールドを選択]**&#x200B;を選択し、 [!DNL Workfront DAM] 選択した [!DNL Workfront] フィールドに入力します。

   >[!NOTE]
   >
   > に送信されたすべてのドキュメント [!DNL Workfront DAM] 権限を持つユーザーのメタデータを [!DNL Workfront] ここにマッピングされたフィールド（アップロード時） [!DNL Workfront DAM].

1. クリック **[!UICONTROL マッピングを追加]**.

1. さらに追加を続行 [!UICONTROL Workfront] フィールドと対応する [!DNL Workfront DAM] フィールド。

### マッピングされたフィールドを削除

{{step-1-to-setup}}

1. 展開 **[!UICONTROL ドキュメント]**&#x200B;を選択し、次に **[!UICONTROL メタデータマッピング]**.

1. フィールドのリストで、メタデータマッピングから削除するフィールドを選択します。
1. クリック **[!UICONTROL 削除]**.

   フィールドはメタデータマッピングから削除され、フィールドに含まれる情報は [!DNL Workfront DAM] アップロードされたドキュメントと共に。
