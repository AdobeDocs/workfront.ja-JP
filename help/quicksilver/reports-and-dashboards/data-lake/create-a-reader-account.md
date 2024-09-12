---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflake用のリーダー（サービス） アカウントを作成します
description: Data Connect データにアクセスするには、まずSnowflakeリーダーアカウントを作成する必要があります。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: c3e18716aa74ed91e21e542437a017586a58d0b3
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 10%

---

# Snowflake用のリーダー（サービス） アカウントを作成します

Data Connect データにアクセスするには、新しい接続ごとにSnowflakeリーダー（またはサービス）アカウントを作成する必要があります。 接続を作成したら、「既存の接続 **」タブの** データアクセス **ページ（** メインメニュー **/** 設定 **/** システム **/** データアクセス ****）で接続をクリックすると、関連する URL とユーザー名が表示されます。

新しく作成した外部データとの接続の使用について詳しくは、[Workfront Data Connect への接続の確立 ](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>次のプランに含まれる：</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>次のプランのアドオンとして購入できます。</p> 
    <ul>
        <li>選択</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect は、従来のWorkfront プランでは使用できません。</p> 
   </td> </td> 
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

+++

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

1. ユーザー名と新しいパスワードを使用して、Snowflakeまたは選択したビジネスビジュアライゼーションツールの Data Connect Data Lake にアクセスできるようになりました。

## リーダーアカウントの取り消し

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. 取り消すアカウントの右側にあるごみ箱アイコン ![ 削除アイコン ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして「**削除**」をクリックします。
