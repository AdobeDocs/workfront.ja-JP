---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce の概要
description: 次をインストールできます。 [!DNL Adobe Workfront] Salesforce ユーザーが送信を許可するための [!DNL Workfront] 要求を行い、Salesforce から離れることなくプロジェクトを自動的に作成します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] 概要

A [!UICONTROL Pro] [!DNL Workfront] この機能を使用するにはプランが必要です。 利用可能な様々なプランについて詳しくは、 [[!DNL Workfront] プラン。](https://www.workfront.com/plans)

次をインストールできます。 [!DNL Adobe Workfront for Salesforce] を許可する [!DNL Salesforce] 送信するユーザー [!DNL Workfront] を要求し、を終了せずに自動的にプロジェクトを作成する [!DNL Salesforce].

As a [!DNL Workfront] 管理者は、ダウンロードして設定できます [!DNL Workfront for Salesforce]. その後、他のすべてのものと共有できます [!DNL Salesforce] ユーザー。

インストールの詳細 [!DNL Workfront for Salesforce]を参照してください。 [インストール [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
詳しくは、 [!DNL Workfront] セクション [!DNL Salesforce] すべてのユーザーについては、 [の設定 [!DNL Adobe Workfront] セクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## アクセス要件

この記事で説明する機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## [!DNL Workfront for Salesforce]

次の操作は、 [!DNL Workfront for Salesforce]:

* 手動で新規を作成 [!DNL Workfront] からのリクエスト [!DNL Salesforce] を Opportunity または Account 内に追加する必要があります。

   作成に関する詳細 [!DNL Workfront] からのリクエスト [!DNL Salesforce]を参照してください。 [送信 [!DNL Adobe Workfront] からのリクエスト [!DNL Salesforce] オブジェクト](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* でプロジェクトの作成を自動的にトリガー [!DNL Workfront] 特定の条件が [!DNL Salesforce]. お使いの [!DNL Salesforce] システム管理者は、次からプロジェクトを作成するトリガーを設定する必要があります [!DNL Salesforce].

   作成に関する詳細 [!DNL Workfront] プロジェクトから [!DNL Salesforce]を参照してください。 [作成 [!DNL Adobe Workfront] プロジェクトから [!DNL Salesforce] オブジェクト](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

を使用する際は、次の点に注意してください。 [!DNL Workfront] 対象 [!DNL Salesforce]:

* 当社は、 [!DNL Salesforce Classic] および [!DNL Lightning Experience] フレームワーク
* 項目の作成元は次の場所のみです： [!DNL Salesforce] に [!DNL Workfront].
* 次の項目に関する情報を表示できます。 [!DNL Workfront] 項目 [!DNL Salesforce].

   この情報はカスタマイズできません。

   のリスト [!DNL Workfront] 次から表示できるフィールド [!DNL Salesforce]を参照してください。  [送信 [!DNL Adobe Workfront] からのリクエスト [!DNL Salesforce] オブジェクト](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  および [作成 [!DNL Adobe Workfront] プロジェクトから [!DNL Salesforce] オブジェクト](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* 次にリンクされた項目に直接アクセスできます： [!DNL Salesforce] クリックして **[!UICONTROL Salesforce に移動]** Workfrontからのリンク

   次に関する情報は表示できません： [!DNL Salesforce] 項目 [!DNL Workfront]が表示されるが、 [!UICONTROL Salesforce] 項目： [!DNL Workfront] レビューイン [!DNL Salesforce].

   [!UICONTROL この **Salesforce に移動**] リンクは次の領域に表示されます。

   * この [!UICONTROL 詳細] プロジェクトまたは問題のセクション
   * プロジェクトまたはイシューのヘッダー。

      システム管理者またはグループ管理者が [!UICONTROL 統合] フィールドをレイアウトテンプレートに追加して、 [!UICONTROL Salesforce に移動] プロジェクトまたはイシューのヘッダー内のリンク。
   * この [!DNL Summary] リストで問題を選択する際に、「 [!UICONTROL 概要を開く] ![](assets/summary-panel-icon.png) 」をクリックします。

      >[!NOTE]
      >
      >この [!UICONTROL Salesforce に移動] リンクはすべてのに対して表示されます [!DNL Workfront] プロジェクトまたはイシューを表示できるユーザー。 次をお持ちの場合は、 [!DNL Salesforce] 次にアクセスできるアカウント [!DNL Salesforce] 問題が記録された商談またはアカウント。

* 1 つのアプリケーション内の 1 つのアイテムのフィールドを更新しても、他のアプリケーション内のリンクされたアイテムに関する情報は更新されません。
