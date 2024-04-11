---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Snowflake用のリーダー（サービス） アカウントを作成します
description: Workfront Data Lake のデータにアクセスするには、まずSnowflake用のリーダーアカウントを作成する必要があります。
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d24659833f0ac0ceeecb245358f2ade8bd08a17
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 5%

---

# Snowflake用のリーダー（サービス） アカウントを作成します

Workfront Data Lake データにアクセスするには、まずSnowflake用のリーダーアカウントを作成する必要があります。 さらに、データへの接続を計画している外部ツールの場合は、許可リストに IP を追加する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

このテーブルの情報の詳細については、を参照してください [Workfrontのドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## リーダーアカウントの作成

1. 「」をクリックします **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅、または（利用可能な場合は）をクリックし、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅のをクリックし、 **設定**.

1. 左側のパネルで、 **システム** > **データアクセス**.

1. クリック **新しい接続を作成**

1. 表示されるウィンドウで、に接続の名前を入力します。 **接続リファレンスの説明** およびユーザー名： **接続ユーザー**&#x200B;を選択し、 **接続を生成**.

   ![リーダーアカウントを作成](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **デフォルトのパスワード** と、Snowflakeを通じてデータを表示できる URL が生成されます。 Snowflakeへの初めてのログイン時に選択したユーザー名とパスワードを使用する必要があるので、URL と同様にパスワードも記録しておいてください。 確認ボックスをチェックし、 **閉じる**.

   ![デフォルトのアカウントパスワード](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. ブラウザーを使用してSnowflakeを開いて前の手順の URL に移動し、選択したユーザー名と前の手順のデフォルトパスワードを入力して「」をクリックします **ログイン**.

1. 初めてログインに成功すると、新しいパスワードを選択するように求められます。 次の両方に、目的のパスワードを入力します **新しいパスワード** および **パスワードの確認** フィールドを選択してから、 **Submit**.

   ![Snowflakeパスワードをリセット](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. これで、ユーザー名と新しいパスワードを使用して、SnowflakeでWorkfront Data Lake にアクセスできるようになりました。

## 許可リストに IP を追加

1. 「」をクリックします **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅、または（利用可能な場合は）をクリックし、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅のをクリックし、 **設定**.

1. 左側のパネルで、 **システム** > **データアクセス**.

1. 「」をクリック **許可された IP** タブをクリックしてから、 **許可リストに IP アドレスを追加** ボタン。

   ![IP アドレスを追加](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

1. IP アドレスの名前を **IP アドレスの説明** で使用するツールの IP アドレスを入力します **IP アドレス**&#x200B;を選択し、 **許可リストに IP を追加**.

## リーダーアカウントを失効させるか、許可リストから IP アドレスを削除します

1. 「」をクリックします **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅、または（利用可能な場合は）をクリックし、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅のをクリックし、 **設定**.

1. 左側のパネルで、 **システム** > **データアクセス**.

1. ごみ箱アイコンをクリック ![アイコンを削除](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 取り消すアカウントの右側に表示されます。

   または

   「」をクリック **許可された IP** タブをクリックしてから、ごみ箱アイコンをクリックします ![アイコンを削除](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 削除する IP アドレスの右側に表示されます。

1. 表示されるウィンドウで、チェックボックスをオンにして確認し、 **削除**.
