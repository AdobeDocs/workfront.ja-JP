---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Experience Manager AssetsまたはAssets Essentialsのマッピングされたメタデータの表示
description: マッピングされたメタデータのリアルタイム表示は、ドキュメントのドキュメントの詳細と概要パネルで確認できます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Experience Manager AssetsまたはAssets Essentialsのマッピングされたメタデータの表示

マッピングされたメタデータのリアルタイム表示は、ドキュメントのドキュメントの詳細と概要パネルで確認できます。 アセットをWorkfrontからExperience Manager AssetsまたはAssets Essentialsに送信する際に、メタデータフィールドが最初にマッピングされます。 Workfront管理者がオブジェクトメタデータの同期を有効にしている場合、どちらかのアプリケーションで変更されたフィールドは最新の状態に保たれます。

## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>Adobe Workfront plan*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfrontライセンス*</strong>
   </td>
   <td>リクエスト以上
   </td>
  </tr>
  <tr>
   <td><strong>製品</strong>
   </td>
   <td>Experience Manager AssetsまたはAssets Essentialsがあり、Admin Consoleでユーザーとして製品に追加される必要があります。
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定*</strong>
   </td>
   <td>ドキュメントへのアクセスを編集
<p>
<strong>注意： </strong>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <strong>カスタムアクセスレベルの作成または変更</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>オブジェクト権限</strong>
   </td>
   <td>アクセス権以上の表示
<p>
追加のアクセス権のリクエストについて詳しくは、 <strong>オブジェクトへのアクセスのリクエスト </strong>.
   </td>
  </tr>
</table>


*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。


## 前提条件

始める前に

* Workfront管理者は、統合を設定する必要があります。 詳しくは、 [Experience Manager Assets統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## ドキュメントの詳細

ドキュメントの詳細でメタデータパネルを開くには：

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「 」を選択します。 **ドキュメント**.
1. 必要なドキュメントの上にマウスポインターを置いて、「 **ドキュメントの詳細**.
1. 検索と展開 **メタデータ** 」セクションに入力します。
   >[!NOTE]
   >
   >このセクションのフィールドは編集できません。 これらは表示専用です。

![ドキュメントの詳細パネル](assets/metadata-panel-doc-details.png)


## ドキュメントの概要

Summary パネルでメタデータパネルを開くには：

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「 」を選択します。 **ドキュメント**.
1. 必要なドキュメントを見つけます。
1. 次をクリック： **概要アイコン** ![概要アイコン](assets/summary-panel-icon.png)をクリックし、次に **メタデータ** 」セクションに入力します。
   >[!NOTE]
   >
   >このセクションのフィールドは編集できません。 これらは表示専用です。

![文書の概要](assets/metadata-panel-summary.png)
