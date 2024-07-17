---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Snowflake用のリーダー（サービス） アカウントを作成します
description: Workfront Data Lake のデータにアクセスするには、まずSnowflake用のリーダーアカウントを作成する必要があります。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 10%

---

# Snowflake用のリーダー（サービス） アカウントを作成します

Workfront Data Lake のデータにアクセスするには、新しい接続ごとにSnowflakeリーダー（またはサービス）アカウントを作成する必要があります。 接続を作成したら、「既存の接続 **」タブの** データアクセス **ページ（** メインメニュー **/** 設定 **/** システム **/** データアクセス ****）で接続をクリックすると、関連する URL とユーザー名が表示されます。

外部の商品と新しく作成した接続の使用について詳しくは、[Workfront Data Lake への接続の確立 ](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md) を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>未定</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## リーダーアカウントの作成

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. **新しい接続を作成** をクリックします。

1. 表示されたウィンドウで、「**接続参照の説明**」に接続の名前を、「**接続ユーザー**」にユーザー名を入力し、「**接続を生成**」をクリックします。

   ![ リーダーアカウントの作成 ](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. **デフォルトのパスワード** と、Snowflakeを使用してデータを表示できる URL が生成されます。 Snowflakeへの初めてのログイン時に選択したユーザー名とパスワードを使用する必要があるので、URL と同様にパスワードも記録しておいてください。 完了したことを示すボックスをオンにし、「**閉じる**」をクリックします。

   ![ デフォルトのアカウントパスワード ](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. ブラウザーを使用してSnowflakeを開いて前の手順の URL に移動し、選択したユーザー名と前の手順のデフォルトのパスワードを入力して、「**ログイン**」をクリックします。

1. 初めてログインに成功すると、新しいパスワードを選択するように求められます。 「**新しいパスワード**」フィールドと「**パスワードを確認**」フィールドの両方に目的のパスワードを入力し、「**送信**」をクリックします。

   ![Snowflakeパスワードのリセット ](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. これで、ユーザー名と新しいパスワードを使用して、Snowflakeまたは選択したビジネスビジュアライゼーションツールでWorkfront Data Lake にアクセスできるようになりました。

## リーダーアカウントの取り消し

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. 取り消すアカウントの右側にあるごみ箱アイコン ![ 削除アイコン ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして「**削除**」をクリックします。
