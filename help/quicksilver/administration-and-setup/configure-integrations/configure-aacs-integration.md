---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager Assets の統合
description: 作業内容は、次のAdobe Experience Manager Assets 統合と連携できます。
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 0%

---

# の設定 [!UICONTROL Experience Manager Assetsas a Cloud Service] 統合

作業内容を [!DNL Experience Manager Assets]&#x200B;:

* からのアセットとメタデータのプッシュ [!DNL Adobe Workfront] から [!DNL Experience Manager Assets]&#x200B;
* からのアセットのリンク [!DNL Experience Manager Assets] を [!DNL Workfront&#x200B;]
* バージョン管理の使用例の容易化
* リンク先のフォルダーを作成 [!DNL Experience Manager Assets]
* アセットおよびフォルダーのメタデータの追跡
* 次の間でプロジェクトメタデータを同期 [!DNL Workfront] および [!DNL Experience Manager Assets]


## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 計画*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] ライセンス*</strong>
   </td>
   <td>[!UICONTROL プラン ]
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
   <td>必ず [!DNL Experience Manager Assets as a Cloud Service]をクリックし、製品にユーザーとして追加される必要があります。
   </td>
  </tr>
  <tr>
   <td>アクセスレベル設定*
   </td>
   <td>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <strong>ユーザーに完全な管理アクセス権を付与する</strong>.
   </td>
  </tr>
</table>


*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。


## 前提条件

始める前に

* 必ず [!DNL Workfront] および [!DNL Adobe Experience Manager Assets] を [!DNL Adobe Admin Consol]e.詳しくは、 [プラットフォームベースの管理上の違い ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 統合情報の設定

1. 次をクリック： **[!UICONTROL メインメニュー]** Adobe Workfrontの右上隅にあるアイコンをクリックし、 **[!UICONTROL 設定]** .
1. 選択 **[!UICONTROL ドキュメント]** 左のパネルで、「 **[!UICONTROL [!DNL Experience Manager]統合]**.
   >[!NOTE]
   >
   >この設定領域は、 [!DNL Workfront] 環境が [!DNL Adobe Admin Console].

1. 選択 **[!UICONTROL 追加 [!DNL Experience Manager] 統合]**.
1. 内 **[!UICONTROL 名前]** 「 」フィールドに、WorkfrontとExperience Manager Assetsでこの統合を操作する際に表示する名前を入力します。
1. 内 **[!UICONTROL ナビゲーション URL]** 」フィールドに値が入力されると、ナビゲーション URL が自動的に入力されます。 この読み取り専用 URL は、組織の [!DNL Experience Manager] インスタンスを [!UICONTROL メインメニュー] を使用してすばやくアクセスできます。
1. 次からリポジトリを選択： **[!UICONTROL [!DNL Experience Manager]Assets リポジトリ]** ドロップダウンメニュー。 自動的に [!DNL Experience Manager] リポジトリを作成します。
   ![experience manager リポジトリを選択](assets/setup-information.png)

1. クリック **[!UICONTROL 保存]** または、 [メタデータの設定（オプション）](#set-up-metadata-optional) 」の節を参照してください。

   >[!NOTE]
   >
   >統合が複雑なので、初期設定を保存した後はリポジトリを変更できません。

## メタデータの設定（オプション）

マッピング可能 [!DNL Workfront] オブジェクトデータを [!DNL Experience Manager] アセット。

>[!IMPORTANT]
>
>メタデータは、次の 1 つの方向にのみマッピングできます。から [!DNL Workfront] から [!DNL Experience Manager]. リンク先のドキュメントのメタデータ [!DNL Workfront] から [!DNL Experience Manager] に転送できません [!DNL Workfront].



### メタデータフィールドの設定

1. でのメタデータスキーマの設定 [!DNL Experience Manager Assets] で説明されているように [Adobe間でのアセットメタデータマッピングの設定 [!DNL Workfront] および [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Workfrontでカスタムフォームフィールドを設定します。 [!DNL Workfront] には、使用できる多くの組み込みカスタムフィールドがあります。 ただし、独自のカスタムフィールドを作成することもできます。 [カスタムフォームの作成または編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Assets

アセットがからプッシュされると、メタデータがマッピングされます。 [!DNL Workfront] 初めて 組み込みフィールドまたはカスタムフィールドを持つドキュメントは、アセットの初回送信時に、指定したフィールドに自動的にマッピングされます [!DNL Experience Manager Assets].

>[!NOTE]
>
>この統合は、次のカスタムメタデータをサポートしていません： [!DNL Adobe Experience Manager].

アセットのメタデータをマッピングするには：

1. 選択 **[!UICONTROL Assets]** を metadata テーブルの上に配置します。
1. 内 **[!UICONTROL [!DNL Workfront]フィールド]** 列で、組み込みフィールドまたはカスタムWorkfrontフィールドを選択します。

   >[!NOTE]
   >
   >1 つの [!DNL Workfront] 複数のフィールド [!UICONTROL Experience Manager Assets] フィールド。 複数の [!DNL Workfront] 単一の [!DNL Experience Manager Assets] フィールドに入力します。

1. 内 [!DNL Experience Manager Assets] 」フィールドで、事前入力されたカテゴリを検索するか、検索フィールドに 2 文字以上入力して、追加のカテゴリにアクセスします。
1. 必要に応じて、手順 2 と 3 を繰り返します。
   ![メタデータフィールド](assets/asset-metadata.png)
1. クリック [!UICONTROL 保存] または、 [フォルダー](#folders) 」の節を参照してください。

### フォルダー

ユーザーがプロジェクト上にリンクフォルダーを作成すると、関連するプロジェクト、ポートフォリオおよびプログラムデータが、 [!DNL Experience Manager Assets].

>[!NOTE]
>
>この統合は、次のカスタムメタデータをサポートしていません： [!DNL Adobe Experience Manager].

フォルダーのメタデータをマッピングするには：

1. 選択 **[!UICONTROL フォルダー]** を metadata テーブルの上に配置します。
1. 内 **[!UICONTROL [!DNL Workfront]フィールド]** 列で、組み込みフィールドまたはカスタムWorkfrontフィールドを選択します。

   >[!NOTE]
   >
   >1 つのWorkfrontフィールドを複数のExperience Manager Assetsフィールドにマッピングできます。 複数の [!DNL Workfront] 単一の [!DNL Experience Manager Assets] フィールドに入力します。

1. 内 **[!DNL Experience Manager Assets]** 」フィールドで、事前入力されたカテゴリを検索するか、検索フィールドに 2 文字以上入力して、追加のカテゴリにアクセスします。
1. 必要に応じて、手順 2 と 3 を繰り返します。
   ![フォルダーメタデータ](assets/folder-metadata.png)
1. クリック **[!UICONTROL 保存]** または、 [プロジェクトメタデータの同期](#project-metadata-sync) 」の節を参照してください。


### オブジェクトメタデータの同期

An [!DNL Experience Manager] マッピング先のフィールド [!DNL Workfront] ポートフォリオ、プログラム、プロジェクト、タスク、タスク、問題、およびドキュメントの各フィールドは、フィールドが [!DNL Workfront].

>[!IMPORTANT]
>
>ユーザーはで書き込みアクセス権が必要です [!DNL Experience Manager] ：メタデータの更新時に同期するために、オブジェクト内に存在するアセットの場合。

1. を有効にします。 **[!UICONTROL オブジェクトのメタデータを同期]** フィールドに入力します。
1. 「保存」をクリックするか、 [リンクされたフォルダーの設定（オプション）](#set-up-linked-folders-optional) 」の節を参照してください。

## リンクされたフォルダーの設定（オプション）

ユーザーが [!DNL Experience Manager] が [!DNL Workfront] プロジェクト。 フォルダーをリンクすると、そのフォルダーに追加されたすべてのアセットが自動的に [!DNL Workfront] および [!DNL Experience Manager]. アセットが [!DNL Workfront] アセットのメタデータが初めてににプッシュされます。 [!DNL Experience Manager Assets].

次の手順では、リンクされたフォルダーを作成する場所を指定します。 各統合では、リンクされたすべてのフォルダーに対して 1 つの場所のみを指定できます。

リンクされたフォルダーを設定するには：

1. 切り替え **[!UICONTROL リンクされたフォルダを有効にする]** オン。
1. フォルダーパスを選択して、この統合に関連付けるリンクされたすべてのフォルダーを指定します。

   >[!NOTE]
   >
   >ユーザーはで書き込みアクセス権が必要です [!DNL Adobe Experience Manager Assets] を指定し、リンクされたフォルダーを作成します。

1. 「**[!UICONTROL 保存]**」をクリックします。
