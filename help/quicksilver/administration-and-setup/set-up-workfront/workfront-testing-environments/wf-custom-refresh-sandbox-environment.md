---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront]  カスタム更新サンドボックス環境'
description: カスタム更新サンドボックスは、実稼動環境のデータを使用してテストし作業できる環境です。トレーニングの実行、セットアップ機能の決定に最適です。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 8ceb370df6ff6f3a7a4376d6086fbabe99609e29
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 95%

---

# [!DNL Adobe Workfront] カスタム更新サンドボックス環境

カスタム更新サンドボックスは、実稼動環境のデータを使用してテストし作業できる環境です。トレーニングの実行、セットアップ機能の決定に最適です。

>[!NOTE]
>
>これは、お客様の [!DNL Workfront] 実稼動環境を複製するテスト環境でもあるプレビューサンドボックスとは異なります。
>
>* 実稼動環境で使用できるようになる前に、プレビューサンドボックスに新しい機能が導入されています。
>* カスタム更新サンドボックスには、実稼動環境で使用できるようになる前に、新しい機能は導入されません。
>
>  また、プレビューサンドボックスには必要ないカスタム更新サンドボックスを取得するための追加費用も発生します。
>
>  プレビューサンドボックスについて詳しくは、[ [!DNL Adobe Workfront]  プレビューサンドボックス環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。


## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] プラン</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] ライセンス</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>[!DNL Workfront] の管理者になる必要があります。[!DNL Workfront] 管理者について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">サポートパッケージ</td> 
   <td> <p>[!UICONTROL Plus]、[!UICONTROL Preferred]、または [!UICONTROL Enterprise]</p> <p>標準サポートパッケージは、カスタム更新サンドボックスにアクセスできませんが、プレビューサンドボックスにアクセスできます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタム更新サンドボックスの更新

カスタム更新サンドボックスには、実際の実稼動データが含まれ、更新するようにスケジュールするまで更新されません。更新のスケジュールは、都合の良いときに、週に 1 回程度の頻度で設定できます。

>[!NOTE]
>
>* 現在の日付の更新をスケジュールすることはできません。例えば、今日が 6月1日の場合、更新をスケジュールできる最も早い日は 6月2日です。
>* スケジュールされた更新は、ユーザーのクラスターに基づいて、夜間に発生する場合があります（米国のクラスターは、米国の夜間に更新されます）。 キュー内の他のお客様とデータの更新量が異なるので、特定の時間は予測できません。 キューに大規模な顧客が多い場合は、更新はその日の後、または翌日まで実行されない可能性があります。
>* カスタム更新サンドボックスには、実稼動環境と同じ製品機能が常に含まれます。ただし、カスタム更新サンドボックスを更新すると、ログイン画面の背景色に対するブランディングのみが保持されます。ログイン画面とナビゲーションバーのロゴが [!DNL Workfront] のデフォルトにリセットされると、更新前に変更したブランディング画像は表示されません。
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 実稼動環境からカスタム更新サンドボックスにアクセス {#access-the-custom-refresh-sandbox-from-your-production-environment}

[!DNL Workfront] 管理者は、実稼動環境からカスタム更新サンドボックスにアクセスできます。

>[!NOTE]
>
>アカウントがクラスター 4（EMEA クラスター）にある場合は、実稼動環境からカスタム更新サンドボックスにアクセスできません。クラスター 4 にアカウントがある場合にカスタム更新サンドボックスにアクセスする方法について詳しくは、[クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスへのアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)[クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスへのアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)を参照してください。

カスタム更新サンドボックスへのアクセス方法：

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**[!UICONTROL 設定]**」![](assets/gear-icon-settings.png) をクリックします。

1. **[!UICONTROL システム]**／**[!UICONTROL 環境設定]**&#x200B;をクリックします。

1. Adobe Analytics の「**[!UICONTROL テスト環境]**」セクションで、「**[!UICONTROL サンドボックス 1]**」または「**[!UICONTROL サンドボックス 2]**」をクリックします。

   サポートパッケージでは、1 つまたは 2 つのカスタム更新サンドボックスにアクセスできるかどうかを指定します。

1. カスタム更新サンドボックスの資格情報を使用してログインします。

   カスタム更新サンドボックスの資格情報は、カスタム更新サンドボックスが最後に更新されてから実稼動環境の資格情報を変更しない限り、実稼動環境の資格情報と同じです。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。

   カスタム更新サンドボックスには、バージョンと最終更新日が画面の上部のバナーに表示されます。実稼動からのすべての情報は使用可能で、更新が完了した後で操作できる状態になっています。

## URL を使用したカスタム更新サンドボックスにアクセス {#access-the-custom-refresh-sandbox-using-a-url}

すべてのユーザーは、URL を使用してカスタム更新サンドボックスにアクセスできます。

* [クラスター 1、2、3、5 のアカウントのカスタム更新サンドボックスにアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスにアクセス](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### クラスター 1、2、3、5 のアカウントのカスタム更新サンドボックスにアクセス {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

サポートパッケージに応じて、1 つまたは 2 つのカスタム更新サンドボックスにアクセスできます。

URL を使用してカスタム更新サンドボックスにアクセスするには：

1. カスタム更新サンドボックスが 1 つだけの場合は、この URL に移動します。

   https://companyname.sb01.workfront.com（古い URL:https://cr1.attasksandbox.com/）。

   または、カスタム更新サンドボックスが 2 つある場合は、上記の URL に加えて、次の URL に移動して、2 番目のカスタム更新サンドボックスにアクセスすることもできます。

   https://companyname.sb02.workfront.com（古い URL:https://cr2.attasksandbox.com/）

1. ログイン画面で、カスタム更新サンドボックスの資格情報を使用してログインします。
1. カスタム更新サンドボックスの資格情報は、カスタム更新サンドボックスが最後に更新されてから実稼動用の資格情報を変更している場合を除き、実稼動用の資格情報と同じです。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。

### クラスター 4 のアカウント（EMEA アカウント）のカスタム更新サンドボックスにアクセス {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

[!DNL Workfront] アカウントがクラスター 4（EMEA クラスター）にある場合は、URL を使用してのみカスタム更新サンドボックスにアクセスできます。アカウントが存在するクラスタを確認するには、カスタマーサポートチームにお問い合わせください。

サポートパッケージに応じて、1 つまたは 2 つのカスタム更新サンドボックスにアクセスできます。

URL を使用してカスタム更新サンドボックスにアクセスするには：

1. カスタム更新サンドボックスが 1 つだけの場合は、この URL に移動します。

   https://companyname.sb01.workfront.com（古い URL:https://cr3.attasksandbox.com）

   または

   カスタム更新サンドボックスが 2 つある場合は、次のいずれかの URL に移動します。

   https://companyname.sb01.workfront.com（古い URL:https://cr3.attasksandbox.com）

   https://companyname.sb02.workfront.com（古い URL:https://cr4.attasksandbox.com）

1. ログイン画面で、カスタム更新サンドボックスの資格情報を使用してログインします。

   カスタム更新サンドボックスの資格情報は、カスタム更新サンドボックスが最後に更新されてから実稼動用の資格情報を変更している場合を除き、実稼動用の資格情報と同じです。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。

## カスタム更新サンドボックスの更新のスケジュール

>[!IMPORTANT]
>
>更新の期間は、更新するデータのサイズによって異なります。更新プロセス中は、カスタム更新サンドボックス環境が何らかの方法で（API 呼び出しや統合など）使用されていないことが重要です。使用されている場合、サンドボックスの更新は正常に完了しません。[!DNL Workfront] は、開始する前にカスタム更新サンドボックス環境を無効にしますが、アクティブなセッションを終了して、サンドボックスの更新が正常に行われるようにする必要があります。

カスタム更新サンドボックスの更新をスケジュールした後、ページ上部の「[!UICONTROL キャンセル]」をクリックすると、キャンセルできます。また、後でスケジュールを変更することもできます。

>[!NOTE]
>
>サンドボックスの自動更新をスケジュールすることはできません。

カスタム更新サンドボックスの更新をスケジュールするには、以下を実行します。

1. カスタム更新サンドボックスにログインします。
1. 画面上部のバナーで「**[!UICONTROL スケジュール]**」をクリックし、カレンダーから日付を選択します。
1. 更新を実行する日付を選択し、「**[!UICONTROL 更新をスケジュール]**」をクリックします。

## カスタム更新サンドボックスから実稼動に切り替え

1. カスタム更新サンドボックスにログインします。

   カスタム更新サンドボックスへのアクセスについて詳しくは、[実稼動環境からカスタム更新サンドボックスにアクセス](#access-the-custom-refresh-sandbox-from-your-production-environment)または [URL を使用してカスタム更新サンドボックスにアクセス](#access-the-custom-refresh-sandbox-using-a-url)を参照してください。

1. 画面上部のバナーで「**[!UICONTROL 実稼動に移動]**」をクリックします。

   サンドボックスで行った作業は、[!UICONTROL 実稼動]環境では表示されません。データの転送は、実稼動からカスタム更新サンドボックスの一方向であり、逆はないためです。

## カスタム更新サンドボックスからメールの受信

[!DNL Workfront] は、カスタム更新サンドボックス環境からのすべてのメール通信を無効にします。カスタム更新サンドボックス環境からメール通知を受け取る場合は、ユーザー設定でこの機能を有効にする必要があります。カスタム更新サンドボックス環境でメール通知を有効にする方法について詳しくは、[プレビューサンドボックス環境からのメール配信の有効化](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)を参照してください。

>[!NOTE]
>
>モバイルアプリのレポート配信およびプッシュ通知は、カスタム更新サンドボックス環境では常に無効になります。ユーザーも [!DNL Workfront] 管理者も、カスタム更新サンドボックス環境にアクセスする際に、モバイルアプリのレポート配信やプッシュ通知を有効にすることはできません。\
>実稼動環境でのレポート配信について詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。実稼動環境のモバイルアプリでのプッシュ通知について詳しくは、の節を参照してください。

## カスタム更新サンドボックスでのシングルサインオンの設定

カスタム更新サンドボックスをシングルサインオンソリューションと連携するように設定する場合は、実稼動環境とは別に設定することで実現できます。カスタム更新サンドボックスの SSO 設定は、実稼動環境の SSO 設定とは独立しています。\
カスタム更新サンドボックスが更新されると、SSO 情報は実稼動環境からコピーされず、カスタム更新サンドボックスの設定が上書きされます。

カスタム更新サンドボックスでシングルサインオンを設定する手順は、実稼動環境で設定する手順と似ています。\
[!DNL Workfront] でのシングルサインオンの設定について詳しくは、[Adobe Workfront でのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)を参照してください。

>[!NOTE]
>
>組織の [!DNL Workfront] インスタンスが Adobe IMS によって有効化されている場合は使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

## 使用目的と可用性

* [!DNL Workfront] カスタム更新サンドボックス環境は、パフォーマンスや負荷テストを目的としていません。組織の既存のワークフローとの機能性が検証されます。

* [!DNL Workfront] カスタム更新サンドボックス環境は、常に使用可能であることを目的としています。通常の営業時間中の Workfront カスタム更新サンドボックス環境の停止は、実稼働環境の問題が存在する場合、その問題の解決に続いて最優先事項となります。週末（土曜日と日曜日）に Workfront カスタム更新サンドボックス環境が停止した場合は、その環境が月曜日の営業時間に実行されるように対処されます。

* カスタム更新サンドボックス環境では、校正を使用できません。
