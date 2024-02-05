---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront] プレビューサンドボックス環境'
description: プレビューサンドボックスは、ライブ環境のレプリカとして機能するテスト環境です。Workfront によって毎週末に更新されます。金曜日にライブ環境に追加されたデータは、次の月曜日までにプレビューサンドボックスに表示されます。すべてのサポートパッケージが、このサンドボックスにアクセスできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 96%

---

# [!DNL Adobe Workfront] プレビューサンドボックス環境

<!-- Audited: 12/2023 -->

[!DNL Workfront] には、[!DNL Workfront] 実稼動環境のレプリカである次の 2 つのテスト環境があります。

* プレビューサンドボックス

  プレビューサンドボックスは、ライブ環境のレプリカとして機能するテスト環境で、[!DNL Workfront] によって毎週末に更新されます。金曜日にライブ環境に追加されたデータは、次の月曜日までにプレビューサンドボックスに表示されます。

  すべてのサポートパッケージは、プレビューサンドボックスにアクセスできます。

* カスタム更新サンドボックス

  カスタム更新サンドボックスは、個別のテスト環境で、ユーザーが手動で更新します。カスタム更新サンドボックスを取得するには、追加の費用がかかります。この環境について詳しくは、[ [!DNL Adobe Workfront] カスタム更新サンドボックス環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard]サポートパッケージ</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus]、[!UICONTROL Preferred]および[!UICONTROL Enterprise]サポートパッケージ</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>プレビューサンドボックス</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>カスタム更新サンドボックス</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## プレビューサンドボックス

プレビューサンドボックスは、組織のユーザーが実稼動環境に影響を与えることなく、実稼動環境のデータを安全にテストし、操作できる環境の役割を果たします。

プレビューサンドボックスには、実際の実稼動データが含まれていますが、毎週末に更新されるので、データは実稼動環境より最大 1 週間遅れている可能性があります。最後の更新時間以降に作成された項目は、次の更新が行われるまで、プレビューサンドボックス環境にあります。

データは、実稼動環境からプレビュー環境に一方向に流れます（逆方向には流れません）。プレビュー環境の更新は、[!DNL Workfront] によって常に毎週末に予定されています。

また、プレビューサンドボックスでは、[!DNL Workfront] で新しい機能を安全な環境にデプロイしてから、実稼動環境にデプロイする準備が整います。プレビューサンドボックスにアクセスすることで、新機能をテストし、その機能についてのフィードバックを [!DNL Workfront] に返すことができます。このため、データは週に 1 回更新されるものの、プレビューサンドボックスのコードは実稼動コードよりも常に進んでいます。

プレビュー環境は、トレーニングの実行、新機能のテストおよび設定機能の決定に最適です。

>[!NOTE]
>
>プレビューサンドボックスにアクセスすると、画面の上部に青いバナーが表示されます。この環境で作業している間は、このバナーを削除できません。
>
>アクセスしている環境の名前（プレビュー）とコードのリリースバージョンがバナーに表示されます。そのリリースについては、「**[!UICONTROL XXの新機能]**」をクリックしてください。
>
>![](assets/preview-banner-nwe-350x161.png)

## プレビューサンドボックスへのアクセス

デフォルトでは、[!DNL Workfront] 管理者は[!UICONTROL プレビュー]サンドボックス環境にアクセスできます。この節の説明どおりに[!UICONTROL プレビュー]サンドボックス環境にアクセスできない場合は、[!DNL Workfront] 管理者またはアドビのサカスタマーサポートチームにお問い合わせください。


### [!DNL Workfront] インターフェイスからプレビューサンドボックスにアクセス {#accessing-the-preview-sandbox-from-the-workfront-interface}

[!DNL Workfront] 管理者は、[!DNL Workfront] インターフェイスを使用してプレビューサンドボックスにアクセスできます。

プレビューサンドボックスにアクセスするには、次の手順に従います。

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、**[!UICONTROL 設定]**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。

1. **[!UICONTROL システム]**／**[!UICONTROL 環境設定]**&#x200B;をクリックします。

1. 「**[!UICONTROL テスト環境]**」セクションで「**[!UICONTROL サンドボックス プレビュー]**」をクリックします。

1. プレビュー資格情報を使用してログインします。

   プレビューの更新後に実稼動環境で変更した場合を除き、これらは実稼動環境の資格情報と同じにする必要があります。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。

### URL を使用してプレビューサンドボックスにアクセス {#accessing-the-preview-sandbox-using-a-url}

URL を使用してプレビューサンドボックスにアクセスできます。

#### クラスター 1、2、3、5 のアカウントのプレビューサンドボックスへのアクセス {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

レビューサンドボックスの URL は `https://companyname.preview.workfront.com/` です。

>[!NOTE]
>
>プレビューサンドボックス用の古い URL にブックマークをリンクしていた場合は、この変更をメモしてブックマークの URL を更新してください。

URL を使用してプレビューサンドボックスにログインするには：

1. `https://companyname.preview.workfront.com/` に移動します。

   EMEA のお客様で、お客様のアカウントがクラスター 4 にある場合は、以下の「クラスター 4（EMEA アカウント）のアカウントのプレビューサンドボックスへのアクセス」の節を参照してください。

1. プレビューの資格情報を使用してログインします。

   >[!TIP]
   >
   >プレビューの更新後に実稼動環境で変更していない限り、プレビューの資格情報は実稼動環境の資格情報と同じにする必要があります。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。


#### クラスター 4 のアカウント（EMEA アカウント）のプレビューサンドボックスへのアクセス {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

URL を使用してプレビューサンドボックスにログインするには：

1. `https://companyname.preview.workfront.com/` に移動します。

   また、プレビューサンドボックスには、[https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login) からアクセスすることもできます。

1. プレビューの資格情報を使用してログインします。

   プレビューの更新後に実稼動環境で変更していない限り、プレビューの資格情報は実稼動環境の資格情報と同じにする必要があります。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。

## プレビューサンドボックスからのメールを受信

Workfront では、プレビューサンドボックス環境からのすべてのメール通信が無効になります。プレビューサンドボックス環境からメール通知を受け取る場合は、ユーザー設定でこの機能を有効にする必要があります。プレビューサンドボックス環境でメール通知を有効にする方法について詳しくは、[プレビューサンドボックス環境からのメールの配信の有効化](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)を参照してください。

>[!NOTE]
>
>モバイルアプリのレポート配信とプッシュ通知は、プレビューサンドボックス環境では常に無効です。ユーザーも [!DNL Workfront] 管理者も、プレビューサンドボックス環境にアクセスする際に、モバイルアプリのレポート配信やプッシュ通知を有効にすることはできません。
>
>実稼動環境でのレポート配信について詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。


## シングルサインオン(SSO)

SSO を使用している場合はカスタマーサポートチームと協力のうえ、SSO 資格情報を使用して[!UICONTROL プレビュー]サンドボックスにログインできるように正しく設定してください。初回ログインに失敗した場合は、通常のサポート担当者または [!DNL Workfront] 管理者にお問い合わせください。

シングルサインオンの詳細については、[Adobe Workfront でのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)を参照してください。

## プレビューサンドボックスでのシングルサインオンの設定

>[!IMPORTANT]
>
>このページで説明する手順は、[!DNL Adobe Admin Console] にまだオンボーディングされていない組織にのみ適用されます。組織が [!DNL Adobe Admin Console] にオンボーディングされている場合、アクションは必要ありません。
>
>組織が [!DNL Adobe Admin Console] にオンボーディングされているかどうかによって手順が異なります。それら手順のリストについては、[プラットフォームベースの管理上の違い（[!UICONTROL Adobe Workfront] / [!UICONTROL Adobe Business Platform]）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。


プレビューサンドボックスでシングルサインオンを使用する場合は、実稼動環境とは別にその設定を行う必要があります。プレビューサンドボックスの SSO 設定は、実稼動環境の SSO 設定とは独立しています。

プレビューサンドボックスが（週末ごとに）更新されると、SSO 情報は実稼動環境からコピーされず、プレビューサンドボックス設定が上書きされます。

プレビューサンドボックスでシングルサインオンを設定する手順は、実稼動環境での手順と同様です。

[!DNL Workfront] でのシングルサインオンの設定について詳しくは、[Adobe Workfront でのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)を参照してください。

## プレビュー環境のパフォーマンスと可用性

パフォーマンスや負荷のテストを目的としていない [!DNL Workfront] プレビュー環境では、組織の既存のワークフローとの機能性が検証されます。

[!DNL Workfront] プレビュー環境は、常に使用可能であることを目的としています。

通常の営業時間中の [!DNL Workfront] プレビュー環境の停止への対応は、実稼働環境の問題（存在する場合）の解決に続く最優先事項となります。

週末（土曜日と日曜日）に [!DNL Workfront] プレビュー環境が停止した場合は、月曜日の営業時間までに復旧できるよう対処されます。
