---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 統合の設定
description: Experience Manager Assets Essentials のコンテンツと作業内容を接続します。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: a729c134ce3d9c565fac18fea80ea7c49471182b
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 96%

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

以下が必要です。

<table>
  <tr>
   <td><strong>Adobe Workfront プラン*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront ライセンス*</strong>
   </td>
   <td>プラン
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager ライセンス</strong>
   </td>
   <td>標準
   </td>
  </tr>
  <tr>
   <td><strong>製品</strong>
   </td>
   <td>Experience Manager Assets Essentials が必要であり、Admin Console でユーザーとして製品に追加されている必要があります。
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定</strong>
   </td>
   <td>Workfront 管理者である必要があります。Workfront 管理者については、<strong>ユーザーへの完全な管理アクセス権の付与</strong>を参照してください。
   </td>
  </tr>
</table>


*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。


## 統合を設定

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコンをクリックし、「**設定**」をクリックします。
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
* （オプション）Workfront でカスタムフォームフィールドを設定します。Workfront には、使用できる多くの組み込みのカスタムフィールドがあります。ただし、独自のカスタムフィールドを作成することもできます。詳しくは、[カスタムフォームの作成または編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

## サポートされるWorkfrontおよびExperience Manager Assetsのフィールド

### AEMキーワード

Workfront でサポートされている任意のフィールドを、Experience Manager Assets Essentials のキーワードにマッピングできます。

フィールドをキーワードにリンクするには、メタデータマッピング領域の Experience Manager Assets フィールドドロップダウンにある `xcm:keywords` を選択します。

複数の 1 行のテキストフィールドをキーワードにマッピングするには、メタデータマッピングの Workfront 側にキーワード値のコンマで区切られたリストを入力し、`xcm:keywords` を Experience Manager Assets 側に入力します。それぞれのフィールド値は、個別のキーワードにマッピングされます。計算フィールドを使用すると、複数の Workfront フィールドを組み合わせて、1 つのコンマ区切りテキストフィールドにすることができます。

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


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
