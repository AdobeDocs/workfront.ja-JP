---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: を設定します。 [!UICONTROL Experience Manager Assetsas a Cloud Service] 統合
description: 作業内容を [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---

# を設定します。 [!UICONTROL Experience Manager Assetsas a Cloud Service] 統合

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>この機能は、 [!DNL Adobe Admin Console].

作業内容を [!DNL Experience Manager Assets]&#x200B;:

* からのアセットとメタデータのプッシュ [!DNL Adobe Workfront] から [!DNL Experience Manager Assets]&#x200B;
* 次のアセットをリンク： [!DNL Experience Manager Assets] を [!DNL Workfront&#x200B;]
* バージョン管理の使用例の容易化
* リンク先のフォルダーを作成 [!DNL Experience Manager Assets]
* アセットおよびフォルダーのメタデータの追跡
* 次の間でプロジェクトメタデータを同期 [!DNL Workfront] および [!DNL Experience Manager Assets]

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
   <td>必要な機能は次のとおりです。 [!DNL Experience Manager Assets as a Cloud Service]をクリックし、製品にユーザーとして追加される必要があります。
   </td>
  </tr>
  <tr>
   <td>アクセスレベル設定*
   </td>
   <td>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。
   </td>
  </tr>
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 前提条件

始める前に

* 必要な機能は次のとおりです。 [!DNL Workfront] および [!DNL Adobe Experience Manager Assets] を [!DNL Adobe Admin Console]. 詳しくは、 [プラットフォームベースの管理上の違い ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 統合情報の設定

{{step-1-to-setup}}

1. 選択 **[!UICONTROL ドキュメント]** 左のパネルで、「 **[!UICONTROL [!DNL Experience Manager]統合]**.

   >[!NOTE]
   >
   >この設定領域は、 [!DNL Workfront] 環境は、 [!DNL Adobe Admin Console].

1. 選択 **[!UICONTROL 追加 [!DNL Experience Manager] 統合]**.
1. Adobe Analytics の **[!UICONTROL 名前]** 「 」フィールドに、WorkfrontとExperience Manager Assetsでこの統合を操作する際に表示する名前を入力します。
1. Adobe Analytics の **[!UICONTROL ナビゲーション URL]** 」フィールドに値が入力されると、ナビゲーション URL が自動的に入力されます。 この読み取り専用 URL は、組織の [!DNL Experience Manager] インスタンスを [!UICONTROL メインメニュー] を使用してすばやくアクセスできます。
1. 次の場所からリポジトリを選択： **[!UICONTROL [!DNL Experience Manager]Assets リポジトリ]** ドロップダウンメニュー。 自動的に次の項目が設定されます。 [!DNL Experience Manager] ユーザープロファイルを割り当てる組織 ID に関連付けられたリポジトリ。
   ![experience manager リポジトリを選択](assets/setup-information.png)

1. クリック **[!UICONTROL 保存]** または、 [メタデータの設定（オプション）](#set-up-metadata-optional) 」の節を参照してください。

   >[!NOTE]
   >
   >統合が複雑なので、初期設定を保存した後はリポジトリを変更できません。

## メタデータの設定（オプション）

マッピング可能 [!DNL Workfront] のアセットメディアフィールドに対するオブジェクトデータ [!DNL Experience Manager] アセット。

>[!IMPORTANT]
>
>メタデータのマッピングは、次の 1 つの方向にのみ実行できます。 [!DNL Workfront] から [!DNL Experience Manager]. リンク先のドキュメントのメタデータ [!DNL Workfront] から [!DNL Experience Manager] に転送できません [!DNL Workfront].

### メタデータフィールドの設定

メタデータフィールドのマッピングを開始する前に、WorkfrontとExperience Manager Assetsの両方でメタデータフィールドを設定する必要があります。

メタデータフィールドを設定するには：

1. でのメタデータスキーマの設定 [!DNL Experience Manager Assets] で説明されているように [Adobe間でのアセットメタデータマッピングの設定 [!DNL Workfront] および [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Workfrontでカスタムフォームフィールドを設定します。 [!DNL Workfront] には、使用できる多くの組み込みカスタムフィールドがあります。 ただし、独自のカスタムフィールドを作成することもできます。 [カスタムフォームの作成または編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **サポートされているWorkfrontおよびExperience Manager Assetsフィールドの詳細を見るには、ここを展開してください。**

**Experience Manager Assets Tags**

Workfrontでサポートされている任意のフィールドを、Experience Manager Assetsのタグにマッピングできます。 これをおこなうには、Experience Manager Assetsのタグ値がWorkfrontと一致するようにする必要があります。

* タグとWorkfrontのフィールド値は、スペルと形式が完全に一致する必要があります。
* Workfrontのタグが大文字である場合でも、experience manager の assets タグにマッピングされるExperience Manager Assetsフィールド値は、すべて小文字にする必要があります。
* Workfrontフィールドの値にスペースを含めることはできません。
* Workfrontのフィールド値には、Experience Manager Assetsタグのフォルダー構造も含める必要があります。
* 複数の 1 行のテキストフィールドをタグにマッピングするには、メタデータマッピングのWorkfront側にタグ値のコンマ区切りリストを入力し、 `xcm:keywords` Experience Manager Assets側の 各フィールド値は、別々のタグにマッピングされます。 計算フィールドを使用すると、複数のWorkfrontフィールドを組み合わせて、コンマで区切られた単一のテキストフィールドにすることができます。
* ドロップダウンフィールド、ラジオボタンフィールドまたはチェックボックスフィールドの値をマッピングするには、そのフィールドで使用可能な値のコンマ区切りリストを入力します。


>[!INFO]
>
>**例**：ここでフォルダー構造に表示されるタグと照合するには、Workfrontのフィールド値は次のようになります。 `landscapes:trees/spruce`. 「 Workfront 」フィールドの値には小文字が含まれています。
>
>タグツリー内の一番左の項目をタグにする場合は、その後にコロンを付ける必要があります。 この例では、景観タグにマッピングするために、Workfrontのフィールド値は次のようになります。 `landscapes:`.
>
>![AEMのフォルダー構造](assets/aem-folder-structure-with-red-boxes.png)


Experience Manager Assetsでタグを作成すると、それらは「メタデータ」セクションの「タグ」ドロップダウンに表示されます。 フィールドをタグにリンクするには、「 `xcm:keywords` ( メタデータマッピング領域の「 Experience Manager Assetsフィールド」ドロップダウン )。

タグの作成および管理方法など、Experience Manager Assetsでのタグについて詳しくは、 [タグの管理](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Experience Manager Assetsのカスタムメタデータスキーマフィールド**

組み込みフィールドとカスタムWorkfrontフィールドの両方を、Experience Manager Assetsのカスタムメタデータスキーマフィールドにマッピングできます。

Experience Manager Assetsで作成したカスタムメタデータフィールドは、メタデータ設定領域の独自のセクションに整理されます。

![カスタムメタデータセクション](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfrontフィールド**

組み込みフィールドとカスタムWorkfrontフィールドの両方をExperience Manager Assetsにマッピングできます。 以下のフィールド値は、大文字と小文字の両方で、WorkfrontとExperience Manager Assetsのスペルが一致する必要があります。

* ドロップダウンフィールド
* 複数選択フィールド

>[!TIP]
>
> フィールドの値が正確に一致するかどうかを確認するには、次に進みます。
>
> * Workfrontの場合は設定/カスタムForms、オブジェクトの場合はフィールド
> * Experience Manager Assetsのアセット/メタデータスキーマ

+++

### アセットのメタデータのマッピング

アセットがからプッシュされると、メタデータがマッピングされます。 [!DNL Workfront] 初めて。 組み込みフィールドまたはカスタムフィールドを持つドキュメントは、アセットの初回送信時に、指定したフィールドに自動的にマッピングされます [!DNL Experience Manager Assets].

アセットのメタデータをマッピングするには：

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Adobe Analytics の **[!UICONTROL [!DNL Workfront]フィールド]** 列で、組み込みフィールドまたはカスタムWorkfrontフィールドを選択します。

   >[!NOTE]
   >
   >1 つの [!DNL Workfront] 複数のフィールド [!UICONTROL Experience Manager Assets] フィールド。 複数の [!DNL Workfront] フィールドを単一の [!DNL Experience Manager Assets] フィールドに入力します。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Adobe Analytics の [!DNL Experience Manager Assets] 」フィールドで、事前入力されたカテゴリを検索するか、検索フィールドに 2 文字以上入力して、追加のカテゴリにアクセスします。
1. 必要に応じて、手順 2 と 3 を繰り返します。
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

ワークフローとは、WorkfrontをAdobe Experience Manager as a Cloud Serviceに接続する一連のアクションです。 Workfront管理者は、Workfrontでワークフローを設定し、それらをプロジェクトテンプレートに割り当てることができます。 ワークフローが割り当てられているプロジェクトテンプレートを使用してプロジェクトを作成すると、ワークフローで定義されたアクションがトリガーされます。

統合で設定したデフォルトのワークフロー値は、プロジェクトテンプレートレベルとプロジェクトレベルで上書きできます。

Adobe Experience Managerの統合では、次のワークフローを使用できます。

* [Adobe Experience Managerにリンクされたフォルダーの作成](#create-adobe-experience-manager-linked-folders)
* [Adobe Experience Manager Assetsに送信されたアセットの公開](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Adobe Experience Managerにリンクされたフォルダーの作成

1. 切り替え **[!UICONTROL リンクされたフォルダーを作成]** オン。
1. フォルダーパスを選択して、この統合に関連付けるリンクされたすべてのフォルダーの場所を指定します。
   ![リンクされたフォルダーナビゲーション](assets/select-folder-aem-integration.png)
1. を有効にします。 **[!UICONTROL Portfolio名とプログラム名を追加]** リンクされたPortfolioの名前の最後にフォルダ名とプログラム名を自動的に含めるオプション。
1. クリック **[!UICONTROL 保存]** または、 [Adobe Experience Manager Assetsに送信されたアセットの公開](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) 」の節を参照してください。

### Adobe Experience Manager Assetsに送信されたアセットの公開

1. オンに切り替え **[!UICONTROL アセットを自動的に公開]**.
1. Adobe Experience Manager Assets に送信するアセットを公開する場所の横にあるチェックボックスをオンにします。 どちらかまたは両方のオプションを有効にできます。
1. （条件付き） Brand Portalオプションを有効にしている場合、アセットを公開するBrand Portalを選択します。
1. クリック **[!UICONTROL 保存]** または、 [リンクされたフォルダーの設定（オプション）](#set-up-linked-folders-optional) 」の節を参照してください。

## リンクされたフォルダーの設定（オプション）

ユーザーが [!DNL Experience Manager] その間 [!DNL Workfront] プロジェクト。 フォルダーをリンクすると、そのフォルダーに追加されたすべてのアセットが自動的に [!DNL Workfront] および [!DNL Experience Manager]. アセットが [!DNL Workfront] アセットのメタデータが初めてににプッシュされます。 [!DNL Experience Manager Assets].

次の手順では、リンクされたフォルダーを作成する場所を指定します。 各統合では、リンクされたすべてのフォルダーに対して 1 つの場所のみを指定できます。

リンクされたフォルダーを設定するには：

1. 切り替え **[!UICONTROL リンクされたフォルダを有効にする]** オン。
1. フォルダーパスを選択して、この統合に関連付けるリンクされたすべてのフォルダーの場所を指定します。

   >[!NOTE]
   >
   >ユーザーはで書き込みアクセス権が必要です [!DNL Adobe Experience Manager Assets] を指定し、リンクされたフォルダーを作成します。

1. 「**[!UICONTROL 保存]**」をクリックします。
