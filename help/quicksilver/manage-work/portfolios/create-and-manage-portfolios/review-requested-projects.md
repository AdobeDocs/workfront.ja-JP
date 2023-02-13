---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: リクエストされたプロジェクトを確認
description: プロジェクトリクエストは、ステータスが「 [!UICONTROL リクエスト] Adobe Workfront この記事では、プロジェクトの要求を確認する方法について説明します。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# リクエストされたプロジェクトを確認

複数のプロジェクト要求がレビュー用に送信された場合、プロジェクト管理オフィスまたはポートフォリオ委員会は会議を開き、送信された要求をレビューし、プロジェクト要求の承認を決定できます。 プロジェクトリクエストは、ステータスが「 [!UICONTROL リクエスト] in [!DNL Adobe Workfront].

次のいずれかの操作を行って、プロジェクトのレビューリクエストを送信できます。

* プロジェクトのステータスを次に変更 **[!UICONTROL リクエスト]**.
* 次を完了： [!UICONTROL ビジネス事例] 承認を得るために送信します。\
   プロジェクトのビジネスケースの完了について詳しくは、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

次の領域で、リクエストされたプロジェクトを確認できます： [!DNL Adobe Workfront]:

* プロジェクトレポート内
* ポートフォリオ内

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!UICONTROL 表示 ]Portfolioへのアクセス以上</p> <p>プロジェクトへの [!UICONTROL 編集 ] アクセス</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオの [!UICONTROL 表示 ] 権限以上</p> <p>プロジェクトに対する [!UICONTROL 管理 ] 権限でステータスを更新する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## プロジェクトレポートでのリクエストされたプロジェクトのレビュー

プロジェクトのレポートを作成して、どのプロジェクトのステータスが「 [!UICONTROL リクエスト].

プロジェクトレポートの作成によるプロジェクトリクエストの承認の詳細については、 [[!UICONTROL プロジェクトレポートの作成によるビジネス事例の承認]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) セクション [ビジネスケースの承認](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## ポートフォリオ内でリクエストされたプロジェクトを確認する

1. リクエストされたプロジェクトを確認するポートフォリオに移動します。
1. クリック&#x200B;**[!UICONTROL プロジェクト]** 左パネル内
1. 次の **[!UICONTROL フィルター]** ドロップダウンメニューで、「 **[!UICONTROL リクエスト]**.

   ステータスが「 」のプロジェクトのみ **[!UICONTROL リクエスト]** がリストに表示されます。

   >[!TIP]
   >
   > ステータスが **[!UICONTROL リクエスト]**&#x200B;の場合、このリストに表示するには、選択したPortfolioにプロジェクトを関連付ける必要があります。

1. リスト内のプロジェクトの名前をクリックして開きます。
1. クリック **[!UICONTROL プロジェクトの詳細]** をクリックします。
1. 次のいずれかの操作を行います。

   * クリック **[!UICONTROL ビジネス事例]**&#x200B;を選択し、「 **[!UICONTROL 承認]** または **[!UICONTROL 拒否]** 内 [!UICONTROL ビジネス事例の概要] ビジネス事例を承認または却下する領域

      ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

      プロジェクトのステータスが **[!UICONTROL 承認済み]** （ビジネスケースが承認された場合）

      プロジェクトのステータスが **[!UICONTROL 却下]** （ビジネス・ケースが却下された場合）

      >[!NOTE]
      ビジネスケースの承認を送信したユーザーに、プロジェクトリクエストが承認されたか却下されたかに関わらず、警告する通知はありません。 

      または

   * プロジェクトのステータスを **[!UICONTROL ステータス]** ドロップダウンメニュー。

      ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
