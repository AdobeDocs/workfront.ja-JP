---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 俊敏なストーリーを移動
description: アジャイルストーリーは、別のイテレーション（スクラムチームの場合）またはバックログ（かんばんチームとスクラムチームの場合）に移動できます。
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 俊敏なストーリーを移動

アジャイルストーリーは、別のイテレーション（スクラムチームの場合）またはバックログ（かんばんチームとスクラムチームの場合）に移動できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>[!UICONTROL ストーリーへのアクセスを管理 ]</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## イテレーションまたはかんばんボードからバックログにストーリーを移動

1. バックログに移動するストーリーが含まれる反復またはかんばんボードに移動します。
1. ページ上部にある繰り返し処理の見出しをクリックします。
1. の **[!UICONTROL ストーリー]** 「 」タブで、移動するストーリーを選択します。
1. クリック **[!UICONTROL 詳細]** > **[!UICONTROL 移動先]**.

   この **[!UICONTROL ストーリーを移動]** ダイアログボックスが表示されます。

   ![ストーリーを移動ダイアログ](assets/iteration-story-move.png)

1. 選択 *team_name*&#39;s バックログ。\
   上記の例では、チーム名はで&#x200B;す。 **マーケティング。**

1. クリック **[!UICONTROL ストーリーを移動]**.

## ストーリーを別の反復に移動

Scrum チームの別の反復にストーリーを移動できます。

>[!NOTE]
>
>この **[!UICONTROL 移動先]** このオプションは、イテレーションの親ストーリーには使用できません。 サブタスクは別の反復にのみ移動できます。

1. 移動するストーリーを含む繰り返しに移動します。
1. ページ上部にある繰り返し処理の見出しをクリックします。
1. の **[!UICONTROL ストーリー]** 「 」タブで、移動するストーリーを選択します。
1. クリック **[!UICONTROL 詳細]** > **[!UICONTROL 移動先]**.

   この **[!UICONTROL ストーリーを移動]** ダイアログボックスが表示されます。

   ![ストーリーを移動ダイアログ](assets/iteration-story-move.png)

1. 選択 **[!UICONTROL 別の反復]**&#x200B;を選択し、ドロップダウンメニューで、ストーリーを移動する反復を選択します。

   >[!NOTE]
   >
   >作業項目 [!UICONTROL 計画開始日] および [!UICONTROL 計画完了日] が [!UICONTROL チームの編集] ページ。 詳しくは、 [[!UICONTROL 設定] 作業項目を反復に追加する際に日付を適用する方法](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 記事内 [スクラムの設定](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. クリック **[!UICONTROL ストーリーを移動]**.
