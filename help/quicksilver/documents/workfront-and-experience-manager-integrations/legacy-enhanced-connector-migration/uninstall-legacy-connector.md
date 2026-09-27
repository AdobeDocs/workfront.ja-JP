---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のコネクターのアンインストール
description: テキスト
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
TQID: 'https://experienceleague.adobe.com/vA8FflK8mA9a002-Mf8WKzECsEhOaIlvnd0kG958ySE'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 100%
---
# Adobe Experience Manager レガシーコネクターでの Workfront のアンインストール

Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合に、Workfront と Adobe Experience Manager レガシーコネクターをアンインストールする必要があります。

## Workfront から登録解除

1. Adobe Experience Manager を開きます。
1. Experience Manager で、**ツール**／**クラウドサービス**／**Workfront 統合の設定**&#x200B;に移動します。
1. 設定（デフォルトでは global-workfront）を選択し、「**プロパティ**」をクリックします。

   ![Workfront から登録解除](assets/unsubscribe-from-workfront.png)

1. ドキュメント、コメントおよびメタデータの同期を無効にします。 ラベルは「無効」の日付にする必要があります。
これにより、Workfront のサブスクリプションが削除され、Day CQ Link Externalizer で定義されたのと同じURLを使用して新しいサブスクリプションを作成できます。

## Workfront 統合設定の削除

サブスクリプションを削除した後は、Workfront 統合設定を削除しても安全です。

1. 設定を開き、「**削除**」を選択します。

   ![設定を削除](assets/delete-wf-configuration.png)

## マッピングを削除

次に、Workfront プロパティマッピングを削除する必要があります。

1. Experience Manager で、**ツール**／**アセット**／**Workfront プロパティマッピング**&#x200B;に移動します。

1. すべてのマッピングを選択し、「**削除**」をクリックします。

## ユーザー権限

Workfront から AEM Dam にアクセスするすべてのユーザーに、`/content/dam` への読み取り権限が付与されました。 ユーザーがその権限を必要としなくなった場合は、そのユーザーに与えられている権限を削除できます。

コネクターは、システムユーザーの WorkFront サービスを使用して動作します。 これは、コネクターをアンインストールする際にアンインストールされます。

>[!NOTE]
>
>コネクターバージョン2.0.3を使用し、グループを追加した場合`workfront-aem-connector-group`、**ツール**／**セキュリティ**／**グループ**&#x200B;に移動して削除する必要もあります。

## Day CQ Link Externalizer

Day CQ Link Externalizer が必要ない場合は、`/system/console/configMgr`に移動し「Day CQ Link Externalizer」を探すことで、これを`localhost:4502`に戻すことができます。

>[!NOTE]
>
>Adobe Experience Manager as a Cloud Service を使用している場合は、プロジェクトを調べ、_com.day.cq.commons.impl.ExternalizerImpl.xml_&#x200B;ファイルを&#x200B;_ui/apps/src/main/content/jcr_ root/apps/mysite/config_内で見つけることでこれを変更できます。

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## コネクターパッケージのアンインストール

コネクターパッケージをアンインストールするために必要な手順は、使用している Adobe Experience Manager のバージョンによって異なります。

### Adobe Experience Manager オンプレミス

オンプレミスで Adobe Experience Manager を使用している場合は、_crx/packmgr/index.jsp_&#x200B;に移動し、`workfront-aem-connector.all-<version>.zip` を探し、**その他**／**アンインストール**&#x200B;をクリックします。

Workfront で作成されたすべてのファイルが削除されていることを確認するために、`/conf` を確認してください。

### Adobe Experience Manager as a Cloud Service

Adobe Experience Manager as a Cloud Service の場合は、プロジェクトの pom.files からコネクターの依存関係を削除できます。

## ファイアウォールと Dispatcher

通信が不要になった場合は、忘れずにホワイトリストに登録されている Workfront URL を削除してください。 また、コネクターは、Dispatcher に設定されたヘッダー apiKey とユーザー名を使用します。 これらは削除することもできます。
