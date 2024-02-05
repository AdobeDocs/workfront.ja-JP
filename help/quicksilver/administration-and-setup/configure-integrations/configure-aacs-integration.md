---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: '[!UICONTROL Experience Manager Assets as a Cloud Service] 統合の設定'
description: 作業内容を [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 84%

---

# [!UICONTROL Experience Manager Assets as a Cloud Service] 統合の設定

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>この機能は、 [!DNL Adobe Admin Console].

[!DNL Experience Manager Assets] のコンテンツと作業内容を連携できます。

* アセットとメタデータを [!DNL Adobe Workfront] から [!DNL Experience Manager Assets] にプッシュ
* [!DNL Experience Manager Assets] から [!DNL Workfront&#x200B;] のお使いのプロジェクトとタスクにアセットをリンク
* ユースケースのバージョン管理を容易化
* [!DNL Experience Manager Assets] にリンクされたフォルダーを作成
* アセットおよびフォルダーのメタデータをトラック
* [!DNL Workfront] および [!DNL Experience Manager Assets] の間でプロジェクトメタデータを同期

>[!NOTE]
>
>複数の [!DNL Experience Manager Assets] リポジトリを 1 つに [!UICONTROL Workfront] 環境、または複数 [!DNL Workfront] 環境を 1 つに [!DNL Experience Manager Assets] リポジトリを作成できます。 設定する統合ごとに、この記事の設定手順に従ってください。

## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] プラン</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] ライセンス</strong>
   </td>
   <td>現在： [!UICONTROL プラン ] <br>
   新規： [!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] ライセンス</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>製品</strong>
   </td>
   <td>[!DNL Experience Manager Assets as a Cloud Service] があり、製品にユーザーとして追加されている必要があります。
   </td>
  </tr>
  <tr>
   <td>アクセスレベル設定*
   </td>
   <td>[!DNL Workfront] 管理者であることが必要です。
   </td>
  </tr>
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 前提条件

開始する前に、

* 必要な機能は次のとおりです。 [!DNL Workfront] および [!DNL Adobe Experience Manager Assets] を [!DNL Adobe Admin Console]. 詳しくは、 [プラットフォームベースの管理上の違い ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 統合情報の設定

{{step-1-to-setup}}

1. 左のパネルで、「**[!UICONTROL ドキュメント]**」をクリックし、「**[!UICONTROL [!DNL Experience Manager]統合]**」を選択します。

   >[!NOTE]
   >
   >この設定領域は、お使いの [!DNL Workfront] 環境が、[!DNL Adobe Admin Console] に含まれる場合のみ表示されます。

1. 「**[!UICONTROL [!DNL Experience Manager] 統合を追加]**」を選択します。
1. 「**[!UICONTROL 名前]**」フィールドに、Workfront と Experience Manager Assets でこの統合を操作する際にユーザーに表示する名前を入力します。
1. 「**[!UICONTROL ナビゲーション URL]**」フィールドには、ナビゲーション URL がシステムによって自動的に入力されます。この読み取り専用 URL は、クイックアクセスの[!UICONTROL メインメニュー]からお使いの組織の [!DNL Experience Manager] にリンクするために使用されます。
1. **[!UICONTROL [!DNL Experience Manager]Assets リポジトリ]**&#x200B;ドロップダウンメニューからリポジトリを選択します。システムでは自動的にお使いのユーザープロファイルが割り当てられる組織 ID に関連する [!DNL Experience Manager] リポジトリが入力されます。
   ![experience manager リポジトリを選択](assets/setup-information.png)

1. 「**[!UICONTROL 保存]**」をクリック、または、この記事の[メタデータの設定（オプション）](#set-up-metadata-optional)の節へ移動してください。

   >[!NOTE]
   >
   >統合が複雑であるため、初期設定を保存した後はリポジトリを変更できません。

## メタデータを設定（オプション）

[!DNL Workfront] オブジェクトデータと [!DNL Experience Manager] Assets のメディアフィールドをマッピングできます。

>[!IMPORTANT]
>
>メタデータのマッピングは、[!DNL Workfront] から [!DNL Experience Manager] への一方向にのみ実行できます。[!DNL Experience Manager] から [!DNL Workfront] にリンクされたドキュメントのメタデータは、[!DNL Workfront] に転送できません。

### メタデータフィールドの設定

メタデータフィールドのマッピングを開始する前に、Workfront と Experience Manager Assets の両方でメタデータフィールドを設定する必要があります。

メタデータフィールドを設定するには、次の手順に従います。

1. [Adobe [!DNL Workfront] と [!DNL Experience Manager Assets] 間でのアセットメタデータマッピングの設定](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=ja)での説明に従って、[!DNL Experience Manager Assets] でメタデータスキーマを設定します。


1. Workfront でカスタムフォームフィールドを設定します。[!DNL Workfront] には、使用できる組み込みのカスタムフィールドが多数あります。ただし、[カスタムフォームの作成または編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)で説明されているように、独自のカスタムフィールドを作成することもできます。

+++ **サポートされている Workfront フィールドおよび Experience Manager Assets フィールドについて詳しくはこちらを展開**

**Experience Manager Assets タグ**

Workfront でサポートされている任意のフィールドを、Experience Manager Assets のタグにマッピングできます。それには、Experience Manager Assets のタグ値が Workfront と一致するようにする必要があります。

* タグと Workfront フィールド値は、つづりと形式が完全に一致する必要があります。
* Experience Manager Assets のタグに大文字が含まれているように見える場合でも、Experience Manager Assets タグにマッピングされる Workfront フィールドの値はすべて小文字にする必要があります。
* Workfront フィールドの値にスペースを含めることはできません。
* Workfront のフィールド値には、Experience Manager Assets タグのフォルダー構造も含める必要があります。
* 複数の 1 行テキストフィールドをタグにマッピングするには、メタデータマッピングの Workfront 側にタグ値のコンマ区切りリストを入力し、Experience Manager Assets 側に `xcm:keywords` を入力します。各フィールド値は、別個のタグにマッピングされます。計算フィールドを使用すると、複数の Workfront フィールドを組み合わせて、1 つのコンマ区切りテキストフィールドにすることができます。
* ドロップダウンフィールド、ラジオボタンフィールドまたはチェックボックスフィールドの値をマッピングするには、それぞれのフィールドで使用可能な値のコンマ区切りリストを入力します。


>[!INFO]
>
>**例**：ここのフォルダー構造に表示されるタグと一致させるために、Workfront のフィールド値は `landscapes:trees/spruce` になります。Workfront フィールド値の小文字に注意してください。
>
>タグをタグツリーの左端の項目にする場合は、タグの後にコロンを付ける必要があります。この例では、landscapes タグにマッピングするために、Workfront のフィールド値は `landscapes:` になります。
>
>![AEM のフォルダー構造](assets/aem-folder-structure-with-red-boxes.png)


Experience Manager Assets でタグを作成すると、タグは「メタデータ」セクションのタグドロップダウンに表示されます。フィールドをタグにリンクするには、メタデータマッピングエリアの Experience Manager Assets フィールドドロップダウンで `xcm:keywords` を選択します。

タグの作成および管理方法など、Experience Manager Assets のタグについて詳しくは、[タグの管理](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=ja)を参照してください。

**Experience Manager Assets のカスタムメタデータスキーマフィールド**

組み込みフィールドとカスタム Workfront フィールドの両方を、Experience Manager Assets のカスタムメタデータスキーマフィールドにマッピングできます。

Experience Manager Assets で作成したカスタムメタデータフィールドは、メタデータ設定エリアの独自のセクションに整理されます。

![「カスタムメタデータ」セクション](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront フィールド**

組み込みフィールドとカスタム Workfront フィールドの両方を、Experience Manager Assets にマッピングできます。以下のフィールド値は、Workfront と Experience Manager Assets の間で、大文字小文字の区別とつづりの両方が一致する必要があります。

* ドロップダウンフィールド
* 複数選択フィールド

>[!TIP]
>
> フィールド値が正確に一致するかどうかを確認するには、以下に移動します。
>
> * Workfront またはオブジェクトフィールドで、設定／カスタムフォーム
> * Experience Manager Assets で、アセット／メタデータスキーマ

+++

### アセットのメタデータのマッピング

アセットが初めて [!DNL Workfront] からプッシュされると、メタデータがマッピングされます。組み込みフィールドやカスタムフィールドを持つドキュメントは、アセットが [!DNL Experience Manager Assets] に初めて送信されたときに、指定のフィールドに自動的にマッピングされます。

アセットのメタデータをマッピングするには、次の手順に従います。

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. **[!UICONTROL [!DNL Workfront]フィールド]**&#x200B;列で、組み込みフィールドまたはカスタム Workfront フィールドを選択します。

   >[!NOTE]
   >
   >単一の [!DNL Workfront] フィールドを複数の [!UICONTROL Experience Manager Assets] フィールドにマッピングできます。複数の [!DNL Workfront] フィールドを単一の [!DNL Experience Manager Assets] フィールドにマッピングすることはできません。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. [!DNL Experience Manager Assets] フィールドで、事前入力されたカテゴリを検索するか、検索フィールドに 2 文字以上入力して、追加のカテゴリにアクセスします。
1. 必要に応じて、手順 2 および 3 を繰り返します。
   ![メタデータフィールド](assets/metadata-no-asset-toggle.png)
1. クリック [!UICONTROL 保存] または、 [ワークフローの設定](#set-up-workflows-optional) 」の節を参照してください。

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## ワークフローの設定（オプション）

ワークフローとは、Workfront を Adobe Experience Manager as a Cloud Service に接続する一連のアクションです。Workfront 管理者は、Workfront でワークフローを設定し、それらをプロジェクトテンプレートに割り当てることができます。ワークフローが割り当てられているプロジェクトテンプレートを使用してプロジェクトを作成すると、ワークフローで定義されたアクションがトリガーされます。

統合で設定したデフォルトのワークフロー値は、プロジェクトテンプレートレベルとプロジェクトレベルで上書きできます。

Adobe Experience Managerの統合では、次のワークフローを使用できます。

* [Adobe Experience Managerにリンクされたフォルダーの作成](#create-adobe-experience-manager-linked-folders)
* [Adobe Experience Manager Assetsに送信されたアセットの公開](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Adobe Experience Managerにリンクされたフォルダーの作成

1. 「**[!UICONTROL リンクされたフォルダーを作成]**」を有効にします。
1. フォルダーパスを選択して、この統合に関連付けるリンクされたすべてのフォルダーの場所を指定します。
   ![リンクされたフォルダーナビゲーション](assets/select-folder-aem-integration.png)
1. 「**[!UICONTROL ポートフォリオ名とプログラム名を追加]**」オプションを有効にすると、リンクされたフォルダー名の最後にポートフォリオ名とプログラム名が自動的に追加されます。
1. クリック **[!UICONTROL 保存]** または、 [Adobe Experience Manager Assetsに送信されたアセットの公開](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) 」の節を参照してください。

### Adobe Experience Manager Assetsに送信されたアセットの公開

1. オンに切り替え **[!UICONTROL アセットを自動的に公開]**.
1. Adobe Experience Manager Assets に送信するアセットを公開する場所の横にあるチェックボックスをオンにします。 どちらかまたは両方のオプションを有効にできます。
1. （条件付き） Brand Portalオプションを有効にしている場合、アセットを公開するBrand Portalを選択します。
1. 「**[!UICONTROL 保存]**」をクリックするか、[リンクされたフォルダーの設定（オプション）](#set-up-linked-folders-optional)の節を参照してください。

## リンクされたフォルダーを設定（オプション）

ユーザーが [!DNL Workfront] プロジェクト内で [!DNL Experience Manager] にリンクされたフォルダーを作成できるようにします。フォルダーがリンクされている場合、そのフォルダーに追加されたすべてのアセットが自動的に [!DNL Workfront] と [!DNL Experience Manager].の両方に表示されます。[!DNL Workfront] 内のリンクされたフォルダーにアセットを初めて追加する場合、そのアセットのメタデータは [!DNL Experience Manager Assets] にプッシュされます。

以下の手順では、リンクされたフォルダーを作成する場所を指定します。各統合では、リンクされたすべてのフォルダーに対して 1 つの場所のみを指定できます。

リンクされたフォルダーを設定するには、次の操作を実行します。

1. 「**[!UICONTROL リンクされたフォルダーを有効にする]**」をオンに切り替えます。
1. フォルダーパスを選択して、この統合に関連付けるリンクされたすべてのフォルダーの場所を指定します。

   >[!NOTE]
   >
   >ユーザーは、リンクされたフォルダーを作成するために指定したフォルダーに対して [!DNL Adobe Experience Manager Assets] での書き込みアクセス権が必要です。

1. 「**[!UICONTROL 保存]**」をクリックします。
