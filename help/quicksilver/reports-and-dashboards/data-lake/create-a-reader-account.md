---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflake用のリーダーアカウントの作成
description: Data Connect データにアクセスするには、まずSnowflake リーダーアカウントを作成する必要があります。
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 9cf221bda04614856a6a3670100742340fb73aee
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 6%

---

# Snowflakeのリーダーアカウントまたは接続を作成する

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

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データ接続** をクリックします。

1. **新しい接続を作成** をクリックします。

1. 表示されたウィンドウで、「**接続参照の説明**」に接続の名前を、「**接続ユーザー**」にユーザー名を入力し、「**接続を生成**」をクリックします。

   ![&#x200B; 新しい接続の作成 &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. **デフォルトのパスワード** と、Snowflakeでデータを表示できる URL が生成されます。 Snowflakeへの初めてのログインで選択したユーザー名とパスワードを使用する必要があるので、URL と同様にパスワードも記録しておいてください。 完了したことを示すボックスをオンにし、「**閉じる**」をクリックします。

   ![&#x200B; デフォルトのアカウントパスワード &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. ブラウザーを使用してSnowflakeを開き、前の手順の URL に移動して、選択したユーザー名と前の手順のデフォルトのパスワードを入力し、「**ログイン**」をクリックします。

1. 初めてログインに成功すると、新しいパスワードを選択するように求められます。 「**新しいパスワード**」フィールドと「**パスワードを確認**」フィールドの両方に目的のパスワードを入力し、「**送信**」をクリックします。

   ![Snowflakeのパスワードをリセット &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. これで、ユーザー名と新しいパスワードを使用して、Snowflakeの Data Connect Data Lake または選択したビジネスビジュアライゼーションツールにアクセスできるようになりました。

## リーダーアカウントの取り消し

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. 取り消すアカウントの右側にあるごみ箱アイコン ![&#x200B; 削除アイコン &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして「**削除**」をクリックします。
