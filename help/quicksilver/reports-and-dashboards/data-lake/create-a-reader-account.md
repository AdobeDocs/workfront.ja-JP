---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflakeのリーダーアカウントの作成
description: Data Connect データにアクセスするには、まずSnowflake リーダーアカウントを作成する必要があります。
author: Courtney
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 5%

---

# Snowflake のリーダーアカウントまたは接続の作成

Data Connect データにアクセスするには、まず組織のSnowflake リーダー（またはサービス）アカウントを作成し、Data Connectにアクセスするユーザーまたはツールごとに新しい接続を作成する必要があります。

接続を作成した後、「既存の接続」タブのデータ接続ページ（メインメニュー/設定/システム/データ接続）で接続をクリックすると、関連するURLとユーザー名を見つけることができます。

新しく作成した外部製品との接続の使用について詳しくは、[Workfront Data Connectへの接続の確立](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)を参照してください。

## アクセス要件

+++ 展開してアクセス要件を表示します。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>Ultimate</p>
    <p>ワークフロー Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>あなたはWorkfrontの管理者でなければなりません</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リーダーアカウントの作成

接続の作成を開始する前に、組織の新しいSnowflake リーダーアカウントを作成する必要があります。

>[!IMPORTANT]
>
>このプロセスは、組織ごとに1回のみ完了する必要があります。 以下の場所に「**Reader アカウントを作成**」ボタンがない場合、リーダーアカウントは既に作成されています。

リーダーアカウントを作成するには：

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、**Setup**&#x200B;をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. 「**Reader アカウントを作成**」ボタンをクリックして、組織のリーダーアカウントの作成を開始します。 このプロセスは自動的に行われますが、完了するには最大で24時間かかる場合があります。

1. 完了すると、リーダーアカウントがアクティブになったことを示すダイアログウィンドウが表示されます。 ブラウザーページを更新して、**新しい接続を作成** ボタンにアクセスします。

![Reader アカウント作成ダイアログ ](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## 接続の作成

>[!IMPORTANT]
>
>2026年6月、多要素認証（MFA）を使用するには、ユーザー名/パスワードの資格情報が必要になります。 Data Connectから、認証プロセスでMFAで動作しないサードパーティのビジュアライゼーションツール、データプロセッサー、スクリプトにデータを読み込むために使用されるサービスユーザーアカウントのRSAまたはPAT ベースの認証に移行することをお勧めします。


1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、**Setup**&#x200B;をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. 「**新しい接続を作成**」をクリックします。

1. 表示されるウィンドウで、**接続参照の説明**&#x200B;に接続の名前を入力し、**接続ユーザー**&#x200B;にユーザー名を入力して、**接続を生成**&#x200B;をクリックします。

   ![新しい接続を作成](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. 接続の認証方法を選択します。
   * [パスワード認証](#password-authentication)
   * [プログラマティックアクセストークン認証](#programmatic-access-token-authentication)
   * [RSA キー認証](#rsa-key-authentication)

### パスワード認証

1. 「**パスワード**」をクリックし、「**接続を生成**」をクリックします。

1. **デフォルトのパスワード**&#x200B;と、Snowflakeを通じてデータを表示できるURLが生成されます。 初めてSnowflakeにサインインする際に選択したユーザー名でパスワードを使用する必要があります。そのため、URLと同様にパスワードの記録を保持するようにしてください。 確認ボックスをオンにして、**閉じる**&#x200B;をクリックします。

   ![既定のアカウント パスワード ](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. ブラウザーを使用してSnowflakeを開き、前の手順で選択したURLに移動し、前の手順で選択したユーザー名とデフォルトのパスワードを入力してから、**ログイン**&#x200B;をクリックします。

1. 初めて正常にログインすると、新しいパスワードを選択するように求められます。 **新しいパスワード**&#x200B;と&#x200B;**パスワードの確認** フィールドに任意のパスワードを入力し、**送信**&#x200B;をクリックします。

   ![Snowflake パスワードのリセット ](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. ユーザー名と新しいパスワードを使用して、SnowflakeのData Connect データレイクまたは任意のビジネスビジュアライゼーションツールにアクセスできるようになりました。

### プログラマティックアクセストークン認証

1. 「**プログラマティックアクセストークン**」をクリックします。

1. トークンの有効期限を「**有効期限**」フィールドに入力します。 有効期限は、最大365日後まで選択できます。

1. 「**接続を生成**」をクリックします。

1. 認証に使用できるPAT トークンが生成され、Snowflake環境のURLが提供されます。 サードパーティのビジュアライゼーションツールまたはデータプロセッサーからSnowflakeに接続するには、PATとユーザー名を使用します。 URLだけでなく、データの記録も保持するようにしてください。 確認ボックスをオンにして、**閉じる**&#x200B;をクリックします。

   ![ プログラマティック アクセス トークン ダイアログ ](/help/quicksilver/reports-and-dashboards/data-lake/assets/pat-test.png)


### RSA キー認証

1. **RSA キー**&#x200B;をクリックします。

1. **RSA公開鍵** フィールドにRSA公開鍵を入力します。

1. 「**接続を生成**」をクリックします。

1. 接続が生成され、Snowflake環境のURLが提供されます。 RSA キーとユーザー名を使用して、サードパーティのビジュアライゼーションツールまたはデータプロセッサーからSnowflakeに接続できます。



Snowflakeへのログインに選択したユーザー名でRSA キーを使用する必要があります。そのため、URLと同様にRSA キーの記録を保持するようにしてください。 確認ボックスをオンにして、**閉じる**&#x200B;をクリックします。

![RSA キーダイアログ ](assets/rsa-test.png)

## リーダーアカウントの失効

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、**Setup**&#x200B;をクリックします。

1. 左側のパネルで、**システム**/**データアクセス**&#x200B;をクリックします。

1. 取り消すアカウントの右側にあるゴミ箱アイコン ![削除アイコン ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして確認し、**削除**&#x200B;をクリックします。
