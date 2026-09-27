---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: '[!DNL Slack] から [!DNL Adobe Workfront] の項目を検索'
description: Slackのインスタンスに[!DNL Workfront] アプリがインストールされている場合は、[!DNL Slack]から[!DNL Adobe Workfront]項目を検索できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: 'https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
    internal-label: Adobe Workfront for Slack
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 92%
---
# [!DNL Slack] から [!DNL Adobe Workfront] の項目を検索

ご利用の [!DNL Slack] のインスタンスに [!DNL Workfront] アプリがインストールされている場合、[!DNL Slack] から [!DNL Adobe Workfront] の項目を検索できます。

[!DNL Workfront] と [!DNL Slack] の設定について詳しくは、[&#x200B; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) 用の [!DNL Adobe Workfront] の設定を参照してください。

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
   [!DNL Workfront for Slack] の設定の手順については、[&#x200B; [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

## [!DNL Slack] から [!DNL Workfront] の項目を検索

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[&#x200B; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  へのアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のいずれかのコマンドを入力します。

   `/workfront search <keyword>`

   または

   `/wf search <keyword>`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。 キーワードは大文字と小文字が区別されず、角括弧や引用符なしで入力する必要があります。

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
