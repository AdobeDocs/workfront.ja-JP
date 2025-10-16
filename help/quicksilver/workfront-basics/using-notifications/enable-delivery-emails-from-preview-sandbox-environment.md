---
navigation-topic: notifications
title: サンドボックスプレビュー環境からのメール配信を有効にする
description: プレビューサンドボックス環境からメール通知を受け取る場合は、プレビューにログインしている間に、ユーザー設定でこの機能を有効にする必要があります。
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 85%

---

# サンドボックスプレビュー環境からのメール配信を有効にする

[!UICONTROL Adobe Workfront] は、プレビューサンドボックス環境とカスタム更新サンドボックス環境の両方からのすべてのメール通信を無効にします。プレビューサンドボックス環境について詳しくは、[Adobe Workfront プレビューサンドボックス環境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。カスタム更新サンドボックス環境について詳しくは、[Adobe Workfront カスタム更新サンドボックス環境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)を参照してください。

プレビューサンドボックス環境から次のメール通知を受け取る場合は、プレビューにログインしている間に、ユーザー設定でこの機能を有効にする必要があります。

* イベント通知によってトリガーされるメール通知
* リマインダー通知
* 遅延または早期のリマインダー通知の自動送信
* 招待メール

これは、自分自身に対して、または自分が編集アクセス権を持っている任意のユーザーに行うことができます。ユーザーの編集に必要なアクセスについて詳しくは、[ユーザーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

>[!NOTE]
>
>モバイルアプリのレポート配信とプッシュ通知は、プレビューサンドボックス環境では常に無効です。ユーザーと [!DNL Workfront] 管理者のどちらも、プレビューサンドボックス環境にアクセスした場合、モバイルアプリのレポート配信やプッシュ通知を有効にすることはできません。
>
>レポートの配信について詳しくは、[レポート配信の概要](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td> 
   <p>独自の設定を変更する投稿者以上</p> <p>他のユーザー用に設定を編集するための「標準」</p> 
   または
   <p> 独自の設定の変更をリクエストまたはそれ以上</p> <p>他のユーザー用に設定を編集する</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>[!UICONTROL System Administrator] アクセスレベル。</p> </li> 
     <li> <p>アクセスレベルの [!UICONTROL Users] 設定で、[!UICONTROL Edit] が選択されている必要があります。また、[!UICONTROL Users]設定の場合は、[!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> で、[!UICONTROL Create]オプションと 2 つの[!UICONTROL User Admin]オプションのうち少なくとも 1 つを有効にする必要があります。 </li> 
     <li>[!UICONTROL User Admin (Group Users)] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プレビューサンドボックス環境からのメールの配信を有効にする

1. プレビューサンドボックス環境にログインします。
1. [!DNL Adobe Workfront] の右上隅のプロフィール画像をクリックします。次に、「**[!UICONTROL その他]**」メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

   または

   [!DNL Workfront] でユーザーを検索して、名前をクリックします。次に、「**[!UICONTROL その他]**」メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

   または

   複数のユーザーの場合：Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ユーザー]**![ ユーザーアイコン ](assets/users-icon-in-main-menu.png) をクリックします。  次に、複数のユーザーを選択して、「**[!UICONTROL 編集]**」をクリックします。

1. 「**[!UICONTROL 環境設定]**」をクリックします。
1. **[!UICONTROL このテスト環境から E メールを受信する]**&#x200B;を選択します。

   >[!NOTE]
   >
   >本番環境では、このオプションは使用できません。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
