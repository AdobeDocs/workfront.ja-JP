---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Adobe Workfront プラグインを使用して作業項目の情報を表示
description: プロジェクト、タスク、イシュー、ドキュメントに関する情報は、Adobe Creative Cloud アプリケーションから確認できます。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: a53a716f-4faf-4ea7-a4fc-ad8d87634267
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 80%

---

# [!DNL Adobe Workfront] プラグインを使用した作業アイテム情報の表示

プロジェクト、タスク、イシュー、ドキュメントに関する情報は、次の [!DNL Adobe Creative Cloud] アプリケーションから確認できます。

{{cc-app-list}}

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <!--<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">製品</td> 
   <td>[!DNL Workfront] ライセンスに加えて [!DNL Adobe Creative Cloud] ライセンスが必要です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、タスク、イシューへの [!UICONTROL View] アクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示するオブジェクトへの表示アクセス権。 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

+++

## 前提条件

{{cc-install-prereq}}

## 詳細とカスタムフォームデータの表示

1. 右上隅にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL 作業リスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![&#x200B; 作業リストに戻る &#x200B;](assets/go-back-to-work-list-350x314.png)

1. 表示する作業アイテムを選択します。

   >[!TIP]
   >
   >**[!UICONTROL メニュー]**&#x200B;アイコンを使用して、作業アイテムの親オブジェクトに移動します。

1. ナビゲーションバーの **[!UICONTROL 詳細]** アイコン ![&#x200B; 詳細 &#x200B;](assets/details.png) をクリックして、以下を表示します。

   * [!UICONTROL 説明]
   * [!UICONTROL 予定完了日]
   * [!UICONTROL ステータス]
   * [!UICONTROL 割り当て先]
   * [!UICONTROL プロジェクト所有者]（プロジェクトのみ）
   * カスタムフォームデータ

## ドキュメントの詳細の表示

1. 右上隅にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL 作業リスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![&#x200B; 作業リストに戻る &#x200B;](assets/go-back-to-work-list-350x314.png)

1. 表示する作業アイテムを選択します。

   >[!TIP]
   >
   >**[!UICONTROL メニュー]**&#x200B;アイコンを使用して、作業アイテムの親オブジェクトに移動します。

1. ナビゲーションバーの **[!UICONTROL ドキュメント]** アイコン ![&#x200B; ドキュメントアイコン &#x200B;](assets/documents.png) をクリックし、ドキュメントをダブルクリックして表示します。

   * [!UICONTROL 説明]
   * [!UICONTROL ファイルタイプ]
   * [!UICONTROL プルーフのステータス]（プルーフに対してのみ使用可能）
   * [!UICONTROL バージョン]
   * [!UICONTROL サイズ]
   * カスタムフォームデータ

## プルーフの詳細の表示

1. 右上隅にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL 作業リスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![&#x200B; 作業リストに戻る &#x200B;](assets/go-back-to-work-list-350x314.png)

1. 表示する作業アイテムを選択します。

   >[!TIP]
   >
   >**[!UICONTROL メニュー]**&#x200B;アイコンを使用して、作業アイテムの親オブジェクトに移動します。

1. ナビゲーションバーの **[!UICONTROL ドキュメント]** アイコン ![&#x200B; ドキュメントアイコン &#x200B;](assets/documents.png) をクリックし、プルーフをダブルクリックします。

1. サムネイルの右上隅にある矢印アイコンをクリックして、[!DNL Workfront] でプルーフの詳細を開きます。

![Workfront でプルーフの詳細ページを開きます。](assets/go-to-proof-details.png)

## プルーフのステータスの表示

1. 右上にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL 作業リスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![&#x200B; 作業リストに戻る &#x200B;](assets/go-back-to-work-list-350x314.png)

1. 表示する作業アイテムを選択します。

   >[!TIP]
   >
   >**[!UICONTROL メニュー]**&#x200B;アイコンを使用して、作業アイテムの親オブジェクトに移動します。

1. ナビゲーションバーの **[!UICONTROL ドキュメント]** アイコン ![&#x200B; ドキュメントアイコン &#x200B;](assets/documents.png) をクリックし、プルーフをダブルクリックします。

1. 下部までスクロールして、プルーフの現在のステータスを表示します。送信済み、開封済み、コメント、決定（SOCD）の詳細については、 [ドキュメントの詳細の概要](/help/quicksilver/documents/managing-documents/document-details-overview.md)を参照してください。

![&#x200B; プルーフステータス &#x200B;](assets/proof-status.png)

## サブタスクとイシューの表示

1. 右上にある&#x200B;**[!UICONTROL メニュー]**&#x200B;アイコンをクリックし、「**[!UICONTROL 作業リスト]**」を選択します。メニューを使用して親オブジェクトに移動することもできます。

   ![&#x200B; 作業リストに戻る &#x200B;](assets/go-back-to-work-list-350x314.png)

1. 表示する作業アイテムを選択します。

   >[!TIP]
   >
   >**[!UICONTROL メニュー]**&#x200B;アイコンを使用して、作業アイテムの親オブジェクトに移動します。

1. **[!UICONTROL イシュー]** アイコン ![&#x200B; イシューアイコン &#x200B;](assets/issues.png) または **サブタスク** アイコン ![&#x200B; サブタスクアイコン &#x200B;](assets/subtasks.png) をクリックします。

1. タスクまたは問題を選択し、ナビゲーションバーの **[!UICONTROL 詳細]** アイコン ![&#x200B; 詳細 &#x200B;](assets/details.png) をクリックして、以下を表示します。

   * [!UICONTROL 予定完了日]
   * [!UICONTROL ステータス]
   * [!UICONTROL 割り当て先]
   * カスタムフォームデータ
