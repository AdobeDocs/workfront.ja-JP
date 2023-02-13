---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: この [!DNL Adobe Workfront] カスタム更新サンドボックス環境
description: カスタム更新サンドボックスは、実稼動環境のデータをテストし、使用する環境です。 また、トレーニングの実行やセットアップ機能の決定にも最適です。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# この [!DNL Adobe Workfront] カスタム更新サンドボックス環境

カスタム更新サンドボックスは、実稼動環境のデータをテストし、使用する環境です。 また、トレーニングの実行やセットアップ機能の決定にも最適です。

>[!NOTE]
>
>これは、プレビューサンドボックス（お客様のをレプリケートするテスト環境）とは異なります [!DNL Workfront] 実稼動環境。
>
>* 実稼動環境で使用できるようになる前に、プレビューサンドボックスに新しい機能が導入されています。
>* カスタム更新サンドボックスには、実稼動環境で使用できるようになる前に、新しい機能は導入されません。
>
>  また、プレビューサンドボックスには必要ないカスタム更新サンドボックスを取得するための追加費用も発生します。
>
>  プレビューサンドボックスについて詳しくは、 [この [!DNL Adobe Workfront] サンドボックス環境をプレビュー](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 計画</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] ライセンス</p> </td> 
   <td> <p>[!UICONTROL プラン ] </p> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">サポートパッケージ</td> 
   <td> <p>[!UICONTROL Plus]、[!UICONTROL Preferred]、または [!UICONTROL Enterprise]</p> <p>標準サポートパッケージは、カスタム更新サンドボックスにアクセスできませんが、プレビューサンドボックスにアクセスできます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタム更新サンドボックスの更新

カスタム更新サンドボックスには、実際の実稼動データが含まれ、更新するようにスケジュールするまで更新されません。 更新のスケジュールは、いつでも、週に 1 回の頻度で設定できます。

>[!NOTE]
>
>* 現在の日付の更新をスケジュールすることはできません。 例えば、今日が 6 月 1 日の場合、更新をスケジュールできる最も早い日は 6 月 2 日です。
>* カスタム更新サンドボックスには、実稼動環境と同じ製品機能が常に含まれます。 ただし、カスタム更新サンドボックスを更新すると、ログイン画面の背景色に対するブランディングのみが保持されます。 ログイン画面とナビゲーションバーのロゴがにリセットされる [!DNL Workfront] デフォルトと、更新前に変更したブランディング画像は表示されません。
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 実稼動環境からカスタム更新サンドボックスにアクセスする {#access-the-custom-refresh-sandbox-from-your-production-environment}

As a [!DNL Workfront] 管理者は、実稼動環境からカスタム更新サンドボックスにアクセスできます。

>[!NOTE]
>
>アカウントがクラスター 4（EMEA クラスター）の場合、実稼動環境からカスタム更新サンドボックスにアクセスできません。 クラスター 4 にアカウントがある場合にカスタム更新サンドボックスにアクセスする方法について詳しくは、 [クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスへのアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスへのアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

カスタム更新サンドボックスにアクセスするには：

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL システム]** >**[!UICONTROL 環境設定]**.

1. 内 **[!UICONTROL テスト環境]** セクションで、 **[!UICONTROL サンドボックス 1]** または **[!UICONTROL サンドボックス 2]**.

   サポートパッケージでは、1 つまたは 2 つのカスタム更新サンドボックスにアクセスできるかどうかを指定します。

1. カスタム更新サンドボックスの資格情報を使用してログインします。

   カスタム更新サンドボックスの資格情報は、カスタム更新サンドボックスを最後に更新してから実稼動用の資格情報を変更した場合を除き、実稼動用の資格情報と同じです。 ログインは、更新が発生した場合にのみ同期されます。 自動的には同期されません。

   カスタム更新サンドボックスには、バージョンと最終更新日が画面の上部にバナーに表示されます。 実稼動環境からのすべての情報は使用可能で、更新が完了した後で操作できる状態になっています。

## URL を使用したカスタム更新サンドボックスへのアクセス {#access-the-custom-refresh-sandbox-using-a-url}

任意のユーザーは、URL を使用してカスタム更新サンドボックスにアクセスできます。

* [クラスター 1、2、3 および 5 のアカウントのカスタム更新サンドボックスにアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスへのアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### クラスター 1、2、3 および 5 のアカウントのカスタム更新サンドボックスにアクセス {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

サポートパッケージに応じて、1 つまたは 2 つのカスタム更新サンドボックスにアクセスできる必要があります。

URL を使用してカスタム更新サンドボックスにアクセスするには：

1. カスタム更新サンドボックスが 1 つだけの場合は、この URL に移動します。

   https://companyname.sb01.workfront.com （古い URL）:https://cr1.attasksandbox.com/.)

   または、2 つのカスタム更新サンドボックスがある場合、上記の URL に加えて、次の URL に移動して、2 番目のカスタム更新サンドボックスにアクセスすることもできます。

   https://companyname.sb02.workfront.com （古い URL）:https://cr2.attasksandbox.com/)

1. ログイン画面で、カスタム更新サンドボックスの資格情報を使用してログインします。
1. カスタム更新サンドボックスの資格情報は、カスタム更新サンドボックスが最後に更新されてから実稼動用の資格情報を変更している場合を除き、実稼動用の資格情報と同じです。 ログインは、更新が発生した場合にのみ同期されます。 自動的には同期されません。

### クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスへのアクセス {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

次に、 [!DNL Workfront] アカウントはクラスター 4（EMEA クラスター）にあり、URL を使用してのみカスタム更新サンドボックスにアクセスできます。 アカウントが存在するクラスタを確認するには、カスタマーサポートチームにお問い合わせください。

サポートパッケージに応じて、1 つまたは 2 つのカスタム更新サンドボックスにアクセスできる必要があります。

URL を使用してカスタム更新サンドボックスにアクセスするには：

1. カスタム更新サンドボックスが 1 つだけの場合は、この URL に移動します。

   https://companyname.sb01.workfront.com （古い URL）:https://cr3.attasksandbox.com)

   または

   2 つのカスタム更新サンドボックスがある場合は、次の URL のいずれかに移動します。

   https://companyname.sb01.workfront.com （古い URL）:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com （古い URL）:https://cr4.attasksandbox.com)

1. ログイン画面で、カスタム更新サンドボックスの資格情報を使用してログインします。

   カスタム更新サンドボックスの資格情報は、カスタム更新サンドボックスが最後に更新されてから実稼動用の資格情報を変更している場合を除き、実稼動用の資格情報と同じです。 ログインは、更新が発生した場合にのみ同期されます。 自動的には同期されません。

## カスタム更新サンドボックスの更新をスケジュールする

>[!IMPORTANT]
>
>更新の期間は、更新するデータのサイズによって異なります。 更新プロセス中は、カスタム更新サンドボックス環境が（API 呼び出しや統合を含む）何らかの方法で使用されていないことが重要です。これにより、サンドボックスの更新が正常に完了しなくなります。 [!DNL Workfront] は、開始する前にカスタム更新サンドボックス環境を無効にしますが、アクティブなセッションを終了して、サンドボックスの更新が正常におこなわれるようにする必要があります。

カスタム更新サンドボックスの更新をスケジュールした後、 [!UICONTROL キャンセル] をクリックします。 また、後でスケジュールを変更することもできます。

>[!NOTE]
>
>サンドボックスの自動更新をスケジュールすることはできません。

顧客更新サンドボックスの更新をスケジュールするには：

1. カスタム更新サンドボックスにログインします。
1. クリック **[!UICONTROL スケジュール]** 画面上部のバナーで日付を選択し、カレンダーから日付を選択します。
1. 更新を実行する日付を選択し、「 **[!UICONTROL 更新をスケジュール]**.

## カスタム更新サンドボックスから実稼動に切り替え

1. カスタム更新サンドボックスにログインします。

   カスタム更新サンドボックスへのアクセスの詳細については、 [実稼動環境からカスタム更新サンドボックスにアクセスする](#access-the-custom-refresh-sandbox-from-your-production-environment) または [URL を使用したカスタム更新サンドボックスへのアクセス](#access-the-custom-refresh-sandbox-using-a-url).

1. クリック **[!UICONTROL 実稼動に移動]** をクリックします。

   サンドボックスでおこなわれた作業は、 [!UICONTROL 実稼動] 環境は、データの転送が単方向であるので、実稼動からカスタム更新サンドボックスに転送されます。逆ではありません。

## カスタム更新サンドボックスからメールを受信

[!DNL Workfront] は、カスタム更新サンドボックス環境からのすべての電子メール通信を無効にします。 カスタム更新サンドボックス環境から電子メール通知を受け取る場合は、ユーザー設定でこの機能を有効にする必要があります。 カスタム更新サンドボックス環境で電子メール通知を有効にする方法について詳しくは、 [プレビューサンドボックス環境からの E メールの配信を有効にする](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>モバイルアプリのレポート配信およびプッシュ通知は、カスタム更新サンドボックス環境では常に無効になります。 あなたも [!DNL Workfront] 管理者は、カスタム更新サンドボックス環境にアクセスする際に、モバイルアプリのレポート配信またはプッシュ通知を有効にすることができます。\
>実稼動環境向けのレポート配信について詳しくは、 [レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)実稼動環境のモバイルアプリでのプッシュ通知について詳しくは、の節を参照してください。

## カスタム更新サンドボックスでのシングルサインオンの設定

カスタム更新サンドボックスをシングルサインオンソリューションと連携するように設定する場合は、実稼動環境とは別に設定することで設定できます。 カスタム更新サンドボックスの SSO 設定は、実稼動環境の SSO 設定とは独立しています。\
カスタム更新サンドボックスを更新すると、SSO 情報は実稼動環境からコピーされず、カスタム更新サンドボックスの設定が上書きされます。

カスタム更新サンドボックスでシングルサインオンを設定する手順は、実稼動環境で設定する手順と似ています。\
設定に関する詳細 [!DNL Workfront] SSO を使用する場合は、 [Adobe Workfrontでのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>組織の [!DNL Workfront] インスタンスはAdobe IMSで有効です。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

## 使用の意図と可用性

[!DNL Workfront] カスタム更新サンドボックス環境は、パフォーマンスや負荷テストを目的としていません。 代わりに、これらの環境を使用して、組織の既存のワークフローとの機能を検証します。

[!DNL Workfront] カスタム更新サンドボックス環境は、常に使用できるようにすることを意図しています。 通常の営業時間にWorkfrontカスタム更新サンドボックス環境を停止した場合、実稼動に関する問題が発生した場合は、その直後に最初の優先順位が設定されます。 週末（土曜日と日曜日）にWorkfront Custom Refresh Sandbox 環境が停止した場合は、その環境が月曜日に営業時間に実行されるように対処します。
