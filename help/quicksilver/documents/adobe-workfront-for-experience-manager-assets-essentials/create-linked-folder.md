---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Experience Manager Assets または Assets Essentials にリンクされたフォルダーの作成
description: Experience Manager Assets または Assets Essentials にリンクされたフォルダーを Workfront 内で作成できます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 1744e6f2b78c64ba2fa4856d9c6a0611404e4458
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 92%

---

# Experience Manager Assets または Assets Essentials にリンクされたフォルダーの作成

Experience Manager Assets または Assets Essentials にリンクされたフォルダーを Workfront 内で作成できます。フォルダーはリンクされているので、フォルダーに追加されたアセットはすべて、Workfront と Experience Manger の両方に自動的に表示されます。リンクされたフォルダー内にアセットがある場合は、アセットを手動で送信する必要はありません。


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
   <td><strong>製品</strong>
   </td>
   <td>Experience Manager Assets as a Cloud Service または Assets Essentials が必要であり、製品にユーザーとして追加されている必要があります。
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager 権限</strong>
   </td>
   <td>Experience Manger 統合の宛先フォルダーへの書き込みアクセス権が必要です。
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定</strong>
   </td>
   <td>統合を設定するには、Workfront管理者である必要があります。 設定が完了すると、プランライセンスを持つユーザーは、個々のプロジェクトにリンクされたフォルダを設定できます。
   </td>
  </tr>
</table>


*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。


## 前提条件

開始する前に、

* Workfront 管理者は、Experience Manager 統合を設定する必要があります。詳しくは、[Experience Manager Assets as a Cloud Service 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。


## リンクされたフォルダーの作成

リンクされたフォルダーは、Workfront 管理者が統合を設定する際に指定した場所に作成されます。統合ごとに、リンクされたフォルダーの場所を 1 つだけ設定できます。

リンクされたフォルダーの名前は、関連付けられているポートフォリオ、プログラムおよびプロジェクトに基づいて自動的に作成され、変更することはできません。プロジェクトがポートフォリオまたはプログラムに関連付けられていない場合、リンクされたフォルダーにはプロジェクト名と作成日が表示されます。

リンクされたフォルダーを作成するには、次の手順に従います。



1. フォルダーを配置するプロジェクトに移動します。
1. 「**新規追加**」を選択したあと、管理者が設定した Experience Manager 統合に移動します。

   >[!NOTE]
   >
   >Workfront 管理者は、この統合に任意の名前を選択できるので、Experience Manager Assets や Assets Essentials に具体的に言及しないことがあります。

1. 「**リンクされたフォルダーを作成**」を選択します。統合の設定時に指定した場所に基づいて、Experience Manager にフォルダーが自動的に作成されます。
   ![リンクされたフォルダーを作成](assets/linked-folder.png)
