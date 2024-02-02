---
navigation-topic: notifications
title: サンドボックスプレビュー環境からのメール配信を有効にする
description: プレビューサンドボックス環境からメール通知を受け取る場合は、プレビューにログインしている間に、ユーザー設定でこの機能を有効にする必要があります。
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: ht
source-wordcount: '517'
ht-degree: 100%

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

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>自身の設定を変更する場合は[!UICONTROL Request]以上の権限</p> <p>他のユーザー用の設定を編集する場合は[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>[!UICONTROL System Administrator] アクセスレベル。</p> <p> このアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> </li> 
     <li> <p>アクセスレベルの [!UICONTROL Users] 設定で、[!UICONTROL Edit] が選択されている必要があります。また、[!UICONTROL Users]設定の場合は、[!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> で、[!UICONTROL Create]オプションと 2 つの[!UICONTROL User Admin]オプションのうち少なくとも 1 つを有効にする必要があります。 </p> <p>[!UICONTROL User Admin (Group Users)] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>アクセスレベルの[!UICONTROL Users]設定について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
    </ul> <p>メモ：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## プレビューサンドボックス環境からのメールの配信を有効にする

1. プレビューサンドボックス環境にログインします。
1. [!DNL Adobe Workfront] の右上隅のプロフィール画像をクリックします。次に、「**[!UICONTROL その他]**」メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

   または

   [!DNL Workfront] でユーザーを検索して、名前をクリックします。次に、「**[!UICONTROL その他]**」メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

   または

   複数のユーザーの場合、Workfront の右上隅で、**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**[!UICONTROL ユーザー]** ![](assets/users-icon-in-main-menu.png) をクリックします。次に、複数のユーザーを選択して、「**[!UICONTROL 編集]**」をクリックします。

1. 「**[!UICONTROL 環境設定]**」をクリックします。
1. **[!UICONTROL このテスト環境から E メールを受信する]**&#x200B;を選択します。

   >[!NOTE]
   >
   >実稼動環境では、このオプションは使用できません。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
