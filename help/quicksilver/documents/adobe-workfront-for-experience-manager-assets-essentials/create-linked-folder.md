---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Experience Manager AssetsまたはフォルダーにリンクしたAssets Essentialsーの作成
description: Workfrontでは、Experience Manager AssetsやフォルダーにリンクしたAssets Essentialsーを作成できます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 1744e6f2b78c64ba2fa4856d9c6a0611404e4458
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Experience Manager AssetsまたはフォルダーにリンクしたAssets Essentialsーの作成

Workfrontでは、Experience Manager AssetsやフォルダーにリンクしたAssets Essentialsーを作成できます。 フォルダーはリンクされているので、フォルダーに追加されたアセットは自動的にWorkfrontと Experience Manager の両方に表示されます。 リンクされたフォルダー内にある場合、手動でアセットを送信する必要はありません。


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
   <td>計画
   </td>
  </tr>
  <tr>
   <td><strong>製品</strong>
   </td>
   <td>Experience Manager Assetsがas a Cloud Service的またはAssets Essentialsで、ユーザーとして製品に追加されている必要があります。
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager権限</strong>
   </td>
   <td>Experience Manager 統合の保存先フォルダーへの書き込みアクセス権が必要です。
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定</strong>
   </td>
   <td>統合を設定するには、Workfront管理者である必要があります。 設定が完了すると、プランライセンスを持つユーザーは、個々のプロジェクトにリンクされたフォルダを設定できます。
   </td>
  </tr>
</table>


*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。


## 前提条件

始める前に

* Workfront管理者は、統合を設定する必要があります。 詳しくは、 [Experience Manager Assets as a Cloud Service統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## リンクされたフォルダーの作成

リンクされたフォルダーは、Workfront管理者が統合の設定時に指定した場所に作成されます。 各統合では、リンクされたフォルダーに対して 1 つのフォルダーの場所のみを指定できます。

リンクされたフォルダの名前は、Portfolio、プログラム、プロジェクトに関連付けられたフォルダに基づいて自動的に作成され、変更できません。 プロジェクトがPortfolioまたはプログラムに関連付けられていない場合、リンクされたフォルダにはプロジェクト名と作成日が表示されます。

リンクされたフォルダーを作成するには：



1. フォルダーを追加するプロジェクトに移動します。
1. 選択 **新規追加**&#x200B;次に、管理者が設定した Adobe Experience Manager 統合に移動します。

   >[!NOTE]
   >
   >Workfrontの管理者は、この統合に対して任意の名前を選択できるので、Experience Manager AssetsやAssets Essentialsについては特に言及しない場合があります。

1. 選択 **リンクされたフォルダーを作成**. 統合が設定された際に指定された場所に基づいて、Experience Manager内にフォルダーが自動的に作成されます。
   ![リンクされたフォルダーを作成](assets/linked-folder.png)
