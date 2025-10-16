---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Slack] から  [!DNL Adobe Workfront]  の項目を検索'
description: ' [!DNL Slack], if your instance of Slack has had the [!DNL Workfront]  アプリがインストールされている場合、 [!DNL Adobe Workfront]  の項目を検索できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 93%

---

# [!DNL Slack] から [!DNL Adobe Workfront] の項目を検索

ご利用の [!DNL Slack] のインスタンスに [!DNL Workfront] アプリがインストールされている場合、[!DNL Slack] から [!DNL Adobe Workfront] の項目を検索できます。

[!DNL Workfront] と [!DNL Slack] の設定について詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) 用の [!DNL Adobe Workfront] の設定を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!DNL Slack] から [!DNL Workfront] の項目を検索する前に、次の操作を行う必要があります。

* [!DNL Slack] 用の [!DNL Workfront] の設定\
   [!DNL Workfront for Slack] の設定の手順については、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

## [!DNL Slack] から [!DNL Workfront] の項目を検索

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  へのアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のいずれかのコマンドを入力します。

   `/workfront search <keyword>`

   または

   `/wf search <keyword>`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。キーワードは大文字と小文字が区別されず、角括弧や引用符なしで入力する必要があります。

1. 表示されるフィールドで、次の中からオブジェクトタイプを選択します。

   * プロジェクト
   * タスク
   * イシュー
   * レポート
   * ユーザー
   * テンプレート
   * ドキュメント
   * ポートフォリオ
   * プログラム
   * ダッシュボード
   * 会社
   * メモ

     一度に選択できるオブジェクトタイプは 1 つだけです。\
      検索条件に一致する項目のリストが表示されます。

1. 項目名をクリックして、ブラウザーの新規タブの [!DNL Workfront] で開きます。
