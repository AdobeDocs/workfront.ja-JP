---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce の概要
description: ' [!DNL Adobe Workfront] for Salesforce をインストールすることで、Salesforce ユーザーが Salesforce を終了せずに [!DNL Workfront] リクエストを送信したり、プロジェクトを自動的に作成したりできます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 97d755c71eb1bdfa8a031fa387741318f9a7f261
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 76%

---

# [!DNL Adobe Workfront for Salesforce] の概要

<!-- Audited: 5/2025 -->

[!DNL Adobe Workfront for Salesforce] をインストールして、[!DNL Salesforce] ユーザーが [!DNL Salesforce] を終了せずに [!DNL Workfront] リクエストを送信したり、プロジェクトを自動的に作成したりできます。

[!DNL Workfront] 管理者は、[!DNL Workfront for Salesforce] をダウンロードして設定できます。その後、他のすべての [!DNL Salesforce] ユーザーと共有できます。

[!DNL Workfront for Salesforce] のインストールについて詳しくは、[インストール： [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) を参照してください。

[!DNL Salesforce] にすべてのユーザー向けの [!DNL Workfront] セクションを設定する方法について詳しくは、[ [!DNL Salesforce] ユーザー向けの [!DNL Adobe Workfront] セクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

>[!NOTE]
>
>この機能を使用するには、[!UICONTROL Pro] [!DNL Workfront] プランが必要です。利用可能な様々なプランについて詳しくは、[[!DNL Workfront] プラン](https://business.adobe.com/products/workfront/pricing.html)を参照してください。

## アクセス要件

この記事で説明されている機能を使用するには、次のアクセス権が必要です。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：標準<p>
   <p>または</p>
   <p>現在：プラン</p>


</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront for Salesforce]

[!DNL Workfront for Salesforce] の使用時には以下を行えます。

* [!DNL Salesforce] のオポチュニティまたはアカウント内で新しい [!DNL Workfront] リクエストを手動で作成する。

  詳しくは、[ オブジェクトからの送信  [!DNL Adobe Workfront]  リクエスト  [!DNL Salesforce]  を参照してください ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)。

* [!DNL Salesforce] で特定の条件が満たされたときに、[!DNL Workfront] でプロジェクトの作成を自動的にトリガーする。[!DNL Salesforce] からプロセスを作成するためのトリガーを [!DNL Salesforce] システム管理者が設定する必要があります。

  [!DNL Salesforce] からの [!DNL Workfront] プロジェクトの作成について詳しくは、[ [!DNL Salesforce] オブジェクトからの [!DNL Adobe Workfront] プロジェクトの作成](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)を参照してください。

[!DNL Workfront] for [!DNL Salesforce] を使用する際は以下を考慮します。

* アドビでは、[!DNL Salesforce Classic] および [!DNL Lightning Experience] のどちらのフレームワークもサポートしています。
* アイテムは [!DNL Salesforce] から [!DNL Workfront] までのみ作成できます。
* [!DNL Workfront] の項目に関する情報を [!DNL Salesforce] に表示することができます。この情報はカスタマイズできません。

  [!DNL Salesforce] に表示できる [!DNL Workfront] フィールドのリストについては、[ [!DNL Salesforce] オブジェクトからの [!DNL Adobe Workfront] リクエストの送信](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)と[ [!DNL Salesforce] オブジェクトからの [!DNL Adobe Workfront] プロジェクトの作成](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md)を参照してください。

* Workfront で「[!UICONTROL Salesforce に移動]」リンクをクリックすることで、[!DNL Salesforce] にリンクしている項目に直接アクセスできます。

  [!DNL Workfront] の [!DNL Salesforce] の項目に関する情報は表示できませんが、WorkfrontにはSalesforceの項目に移動するリンクがあり、そこで確認できます。

  [!UICONTROL Salesforceに移動 &#x200B;] リンクが次の領域に表示されます。

   * プロジェクトまたはイシューの [!UICONTROL &#x200B; 詳細 &#x200B;] セクション。
   * プロジェクトまたはイシューのヘッダー。

     プロジェクトまたはイシューのヘッダーに「[!UICONTROL Salesforce に移動]」リンクを表示するには、システム管理者またはグループ管理者がレイアウトテンプレートに「[!UICONTROL 統合]」フィールドを追加する必要があります。
   * リストのツールバーで [!UICONTROL &#x200B; 概要を開く &#x200B;]![ 概要パネルアイコン ](assets/summary-panel-icon.png) をクリックした後、リストでイシューを選択する際のイシューの [!DNL Summary] パネル。

     >[!NOTE]
     >
     >「[!UICONTROL Salesforce に移動]」リンクは、プロジェクトまたはイシューを表示できるすべての [!DNL Workfront] ユーザーに表示されます。イシューが記録された [!DNL Salesforce] オポチュニティまたはアカウントに移動するには、[!DNL Salesforce] アカウントが必要です。

* 一方のアプリケーション内のある項目のフィールドを更新しても、もう一方のアプリケーション内のリンクされた項目に関する情報は更新されません。
