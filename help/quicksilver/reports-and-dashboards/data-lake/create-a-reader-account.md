---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflake用のリーダーアカウントの作成
description: Data Connect データにアクセスするには、まずSnowflake リーダーアカウントを作成する必要があります。
author: Courtney
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 32f738e56a471407997031e13bb22abe81ac535c
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 5%

---

# Snowflake のリーダーアカウントまたは接続の作成

Data Connect データにアクセスするには、まず組織のSnowflake リーダー（またはサービス）アカウントを作成してから、Data Connect にアクセスするユーザーまたはツールごとに新しい接続を作成する必要があります。

接続を作成したら、「既存の接続」タブのデータ接続ページ（メインメニュー/設定/システム/データ接続）で接続をクリックすると、関連する URL とユーザー名が表示されます。

新しく作成した外部データとの接続の使用について詳しくは、[Workfront Data Connect への接続の確立 &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

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
   <td> <p>Workfront管理者である必要があります</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リーダーアカウントの作成

接続の作成を開始するには、組織の新しいSnowflake リーダーアカウントを作成する必要があります。

>[!IMPORTANT]
>
>このプロセスは、組織ごとに 1 回だけ完了する必要があります。 以下に説明する場所に「**Reader アカウントを作成**」ボタンがない場合、リーダーアカウントは既に作成されています。

リーダーアカウントを作成するには：

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データ接続** をクリックします。

1. 「**Reader アカウントを作成**」ボタンをクリックして、組織のリーダーアカウントの作成を開始します。 この処理は自動的に行われますが、完了するまでに最大 24 時間かかる場合があります。

1. 完了すると、リーダーアカウントがアクティブになったことを説明するダイアログウィンドウが表示されます。 ブラウザーページを更新して、「**新しい接続を作成**」ボタンにアクセスできるようにします。

![Reader アカウントが作成されましたダイアログ &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## 接続の作成

>[!IMPORTANT]
>
>2026 年 6 月に、多要素認証（MFA）を使用するために、ユーザー名とパスワードの資格情報が必要になります。 Data Connect からサードパーティのビジュアライゼーションツール、データプロセッサー、スクリプトにデータを読み込むために使用されるサービスユーザーアカウントについては、認証プロセスで MFA と連携しない場合は、RSA または PAT ベースの認証に移行することをお勧めします。


1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データ接続** をクリックします。

1. **新しい接続を作成** をクリックします。

1. 表示されたウィンドウで、「**接続参照の説明**」に接続の名前を、「**接続ユーザー**」にユーザー名を入力し、「**接続を生成**」をクリックします。

   ![&#x200B; 新しい接続の作成 &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. 接続の認証方法を選択してください：
   * [パスワード認証](#password-authentication)
   * [プログラムによるアクセストークン認証](#programmatic-access-token-authentication)
   * [RSA キー認証](#rsa-key-authentication)

### パスワード認証

1. **パスワード**/**接続を生成** をクリックします。

1. **デフォルトのパスワード** と、Snowflakeでデータを表示できる URL が生成されます。 Snowflakeへの初めてのログインでは、選択したユーザー名とパスワードを使用する必要があります。そのため、URL と同様に記録が保持されていることを確認します。 完了したことを示すボックスをオンにし、「**閉じる**」をクリックします。

   ![&#x200B; デフォルトのアカウントパスワード &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. ブラウザーを使用してSnowflakeを開き、前の手順の URL に移動して、選択したユーザー名と前の手順のデフォルトのパスワードを入力し、「**ログイン**」をクリックします。

1. 初めてログインに成功すると、新しいパスワードを選択するように求められます。 「**新しいパスワード**」フィールドと「**パスワードを確認**」フィールドの両方に目的のパスワードを入力し、「**送信**」をクリックします。

   ![Snowflakeのパスワードをリセット &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. これで、ユーザー名と新しいパスワードを使用して、Snowflakeの Data Connect Data Lake または選択したビジネスビジュアライゼーションツールにアクセスできるようになりました。

### プログラムによるアクセストークン認証

1. **プログラムによるアクセストークン** をクリックします。

1. **有効期限** フィールドに、トークンの有効期限を入力します。 有効期限は最大 365 日後まで選択できます。

1. **接続を生成** をクリックします。

1. 認証に使用できる PAT トークンが生成され、Snowflake環境の URL が提供されます。 指定した PAT およびユーザー名を使用して、サードパーティのビジュアライゼーションツールまたはデータプロセッサーからSnowflakeに接続できます。 必ず、URL と共に記録を残してください。 完了したことを示すボックスをオンにし、「**閉じる**」をクリックします。

   ![&#x200B; プログラムによるアクセストークンダイアログ &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/pat-test.png)


### RSA キー認証

1. **RSA キー** をクリックします。

1. 「**RSA 公開鍵**」フィールドに RSA 公開鍵を入力します。

1. **接続を生成** をクリックします。

1. 接続が生成され、Snowflake環境の URL が提供されます。 指定した RSA キーとユーザー名を使用して、サードパーティのビジュアライゼーションツールまたはデータプロセッサーからSnowflakeに接続できます。



Snowflakeへのログインに選択したユーザー名で RSA キーを使用する必要があるので、URL と同様に記録が保持されていることを確認します。 完了したことを示すボックスをオンにし、「**閉じる**」をクリックします。

![RSA キーダイアログ &#x200B;](assets/rsa-test.png)

## リーダーアカウントの取り消し

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. 取り消すアカウントの右側にあるごみ箱アイコン ![&#x200B; 削除アイコン &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして「**削除**」をクリックします。
