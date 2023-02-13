---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のコネクタのアンインストール
description: テキスト
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Adobe Experience ManagerレガシーコネクタでのWorkfrontのアンインストール

WorkfrontとAdobe Experience Manager Assetsas a Cloud Serviceを接続する最新のネイティブ統合に、WorkfrontとAdobe Experience Managerレガシーコネクタをアンインストールする必要があります。

## Workfrontを購読解除

1. Adobe Experience Manager を開きます。
1. Experience Managerで、に移動します。 **ツール** > **Cloud Services** > **Workfront統合の設定**.
1. 設定（デフォルトは global-workfront）を選択し、 **プロパティ**.
   ![Workfront から購読解除](assets/unsubscribe-from-workfront.png)
1. ドキュメント、コメントおよびメタデータの同期を無効にします。 ラベルは「無効」の日付にする必要があります。
これにより、Workfrontのサブスクリプションが削除され、 Day CQ Link Externalizer で定義されたのと同じ URL を使用して新しいサブスクリプションを作成できます。

## Workfront統合設定の削除

サブスクリプションを削除した後、Workfront Integration Configuration を削除しても安全になりました。

1. 設定を開き、「 」を選択します。 **削除**.
   ![設定を削除](assets/delete-wf-configuration.png)

## マッピングを削除

次に、Workfront Property Mapping を削除する必要があります。

1. Experience Managerで、に移動します。 **ツール** > **Assets** > **Workfront Property Mapping**.

1. すべてのマッピングを選択し、 **削除**.

## ユーザー権限

WorkfrontからAEM Dam にアクセスするすべてのユーザーに、への読み取り権限が付与されました。 `/content/dam`. ユーザーがその権限を必要としなくなった場合は、そのユーザーに与えられている権限を削除できます。

コネクタは、システムユーザーの WorkFront サービスを使用して動作します。 これは、コネクタをアンインストールする際にアンインストールされます。

>[!NOTE]
>
>Connecter バージョン 2.0.3 を使用し、グループを追加した場合 `workfront-aem-connector-group`を削除する場合は、 **ツール** > **セキュリティ** > **グループ**.

## Day CQ Link Externalizer

Day CQ Link Externalizer が必要ない場合は、これをに戻すことができます。 `localhost:4502` ～に行くことで `/system/console/configMgr` 「Day CQ Link Externalizer」を探しています。

>[!NOTE]
>
>Adobe Experience Manager as a Cloud Serviceを使用している場合は、プロジェクトを調べ、ファイルを見つけることで、これを変更できます _com.day.cq.commons.impl.ExternalizerImpl.xml_ inside _ui/apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## コネクタパッケージのアンインストール

コネクタパッケージをアンインストールするために必要な手順は、使用しているAdobe Experience Managerのバージョンによって異なります。

### Adobe Experience Managerオンプレミス

オンプレミスでAdobe Experience Managerを使用している場合は、に移動します。 _crx/packmgr/index.jsp_&#x200B;を探し、 `workfront-aem-connector.all-<version>.zip`をクリックし、 **詳細** その後 **アンインストール**.

以下を確認してください。 `/conf` Workfrontで作成されたすべてのファイルが削除されていることを確認します。

### Adobe Experience Manager as a Cloud Service

Adobe Experience Manager as a Cloud Serviceの場合は、プロジェクトの pom.files からコネクタの依存関係を削除できます。

## ファイアウォールと Dispatcher

通信が不要になった場合は、忘れずにホワイトリストに登録されているWorkfront URL を削除してください。 また、コネクタは、Dispatcher に設定されたヘッダー apiKey とユーザー名を使用します。 これらは削除することもできます。
