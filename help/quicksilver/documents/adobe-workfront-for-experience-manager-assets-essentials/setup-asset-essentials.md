---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 統合の設定
description: Experience Manager Assets Essentials で作業とコンテンツを結び付けます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 97%

---

# Experience Manager Assets Essentials 統合の設定

Experience Manager Assets Essentials で作業とコンテンツを結び付けます。

* Adobe Workfront から Experience Manager Assets Essentials にアセットおよびメタデータをプッシュ
* Experience Manager Assets Essentials からのアセットを Workfront のプロジェクトおよびタスクにリンク
* Experience Manager Assets Essentials へプッシュされたアセットのバージョン管理ワークフローを促進

>[!NOTE]
>
>複数の Experience Manager Assets リポジトリを 1 つの Workfront 環境に接続することも、複数の Workfront 環境を組織 ID をまたいで 1 つの Experience Manager Assets リポジトリに接続することもできます。設定する統合ごとに、この記事の設定手順に従ってください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table>
  <tr>
   <td>[!DNL Adobe Workfront] プラン*
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] ライセンス
   </td>
   <td><p>現在：[!UICONTROL Plan]</p>
   <p>新規：[!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] ライセンス
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>製品
   </td>
   <td>Experience Manager Assets Essentials が必要であり、Admin Console でユーザーとして製品に追加されている必要があります。
   </td>
  </tr>
  <tr>
   <td>アクセスレベル設定
   </td>
   <td>[!DNL Workfront] 管理者である必要があります。
   </td>
  </tr>
</table>

この表にある情報についての詳細は、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 統合を設定

{{step-1-to-setup}}

1. 左側のパネルで&#x200B;**ドキュメント** ![ドキュメントアイコン](assets/document-icon.png) を選択し、続いて「**Experience Manager の統合**」を選択します。
1. 「**Experience Manager の統合を追加**」を選択します。
1. 以下を指定します。

   <table>
   <tr>
      <td><strong>名前</strong>
      </td>
      <td>ドキュメント領域の「新規追加」ボタンに、ユーザーに表示する名前を入力します。
      </td>
   </tr>
   <tr>
      <td><strong>ナビゲーション URL</strong>
      </td>
      <td>ナビゲーション URL がシステムにより自動的に入力されます。この URL は、メインメニューから組織の Assets Essentials インスタンスにリンクし、すばやくアクセスするために使用されます。
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets リポジトリ</strong>
      </td>
      <td>
      組織 ID に関連付けられた Experience Manager リポジトリが、システムにより自動的に入力されます。
      </td>
   </tr>
   </table>

1. 「**保存**」をクリックするか、この記事の[メタデータを設定（オプション）](#set-up-metadata-optional)の節へ移動してください。


## メタデータを設定（オプション）

Workfront オブジェクトデータを、Experience Manager Assets のアセットメディアフィールドにマッピングします。メタデータは、アセットが最初に Workfront にプッシュされる際にマッピングされます。


### 前提条件

開始する前に、

* [Adobe Workfront と Experience Manager Assets 間のアセットメタデータマッピングの設定](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=ja)の説明に従って、Experience Manager Assets Essentials のメタデータスキーマを設定します。
* （オプション）Workfront でカスタムフォームフィールドを設定します。Workfront には、使用できる多くの組み込みのカスタムフィールドがあります。ただし、独自のカスタムフィールドを作成することもできます。詳しくは、[フォームデザイナーを使用したフォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## サポートされている Workfront および Experience Manager Assets のフィールド

### AEM キーワード

Workfront でサポートされている任意のフィールドを、Experience Manager Assets Essentials のキーワードにマッピングできます。

フィールドをキーワードにリンクするには、メタデータマッピング領域の Experience Manager Assets フィールドドロップダウンにある `xcm:keywords` を選択します。

複数の 1 行のテキストフィールドをキーワードにマッピングするには、メタデータマッピングの Workfront 側にキーワード値のコンマで区切られたリストを入力し、`xcm:keywords` を Experience Manager Assets 側に入力します。それぞれのフィールド値は、個別のキーワードにマッピングされます。計算フィールドを使用すると、複数の Workfront フィールドを組み合わせて、1 つのコンマ区切りテキストフィールドにすることができます。

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### アセット

アセットが Workfront から初めてプッシュされると、メタデータがマッピングされます。組み込みフィールドまたはカスタムフィールドを持つドキュメントは、アセットを Experience Manager Assets Essentials に初めて送信する際に、指定したフィールドに自動的にマッピングされます。

1. **Workfront のフィールド**&#x200B;列で、組み込みフィールドまたはカスタム Workfront フィールドを選択します。

   >[!NOTE]
   >
   >単一の Workfront フィールドを複数の Experience Manager Assets フィールドにマッピングできます。複数の Workfront フィールドを単一の Experience Manager Assets フィールドにマッピングすることはできません。

1. **Experience Manager** フィールドで、Experience Manager Assets フィールドを選択します。

   Workfront フィールドを Experience Manager Assets タグにマッピングするには、`xcm:keywords` を選択します。

1. 必要に応じて、手順 1 と 2 を繰り返します。
   ![メタデータを有効化](assets/metadata-assets-essentials.png)
1. 「**保存**」をクリックするか、この記事の[リンクされたフォルダーを設定（オプション）](#set-up-linked-folders-optional)の節を参照してください。


## リンクされたフォルダーを設定（オプション）

{{setup-linked-folder}}
