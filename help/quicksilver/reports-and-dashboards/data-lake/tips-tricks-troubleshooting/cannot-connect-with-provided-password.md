---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI ツールは、指定されたパスワードではに接続できません
description: Power BI ツールから Data Connect にログインしようとすると、ログインエラーが発生します。
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---


# Power BI ツールは指定されたパスワードで接続できません

## 問題

Power BI ツールから Data Connect にログインしようとすると、次のエラーが表示されます。

`Cannot connect from BI tool with provided password`

## 原因

JDBC 接続を作成する際に、Workfrontによって Data Connect 用の一時パスワードが指定されます。

Power BIから Data Connect にアクセスする前に、提供された接続詳細を使用してログインし、一時パスワードを更新して、ログインに進む必要があります。


## ソリューション

Workfrontで接続パスワードをリセットしてから、接続を編集ダイアログボックスに表示されるリンクを使用して新しいパスワードを作成します。

### Workfrontの接続パスワードのリセット

1. Workfront/設定/システム/データ接続に移動します。
1. リストから接続を検索して開きます。
1. 「**接続パスワードのリセット**」で、パスワードのリセットを確認するチェックボックスをオンにします。
1. **接続パスワードのリセット** をクリックします。
   ![ 接続パスワードのリセット ](assets/reset-password.png)
1. 以下の節に進みます。

### 接続の新しいパスワードの作成

1. URL をコピーし、新しいブラウザータブに貼り付けます。
1. Workfrontで、「Connection User name」と「Default Password」をコピーして、新しいブラウザータブに貼り付けます。
   ![url とデフォルトのパスワードをコピー ](assets/link-password.png)
1. **ログイン** をクリックします。
1. 新しいパスワードを入力し、「**送信**」をクリックします。
1. Power BI ツールに移動し、新しいパスワードでログインします。

