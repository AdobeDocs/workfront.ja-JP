---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの印刷
description: ダッシュボードを印刷したり .PDF ファイルに書き出したりできます。ダッシュボードを印刷するには、ダッシュボードを表示する権限が必要です。
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: efae17458f2aa08ca2286ef5e43c68d1f9334b7b
workflow-type: ht
source-wordcount: '503'
ht-degree: 100%

---

# ダッシュボードの印刷

ダッシュボードを印刷したり .PDF ファイルに書き出したりできます。ダッシュボードを印刷するには、ダッシュボードを表示する権限が必要です。

>[!NOTE]
>
>この機能は、標準のダッシュボードビューでのみ使用できます。プロジェクトエリアに埋め込まれたダッシュボードや、カスタムタブとして設定されたダッシュボードでは使用できません。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボードおよびカレンダーの表示アクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクトの権限</strong>/td&gt; 
   <td> <p>ダッシュボードの表示権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

ダッシュボードを印刷するには、まずダッシュボードを作成する必要があります。

ダッシュボードの作成については、[ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)を参照してください。

## ダッシュボードの印刷時に印刷される情報について

ダッシュボードを印刷するか .PDF ファイルとして保存すると、Adobe Workfront web アプリケーションに表示されるダッシュボードの一部の情報が、印刷または書き出されたファイルに表示されない場合があります。

* [表示される情報](#what-is-displayed)
* [表示されない情報](#what-is-not-displayed)

### 表示される情報 {#what-is-displayed}

印刷または書き出されたダッシュボードファイルには、次の情報が含まれます。

* ダッシュボードのタイトル
* レポートのタイトル
* レポートが前回生成されたときのタイムスタンプ
* リスト表示、外部 web ページ、レポート、カレンダーなど、ダッシュボード上のすべてのオブジェクト
* 会社のロゴ（Workfront 管理者がグローバルナビゲーションバーでカスタマイズしてある場合）。Workfront サイトのブランディングについて詳しくは、[Adobe Workfront インスタンスのブランディング](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)を参照してください。

### 表示されない情報 {#what-is-not-displayed}

印刷または書き出されたダッシュボードファイルには、次の情報が含まれません。

* Workfront ナビゲーションバー
* Workfront に固有のその他のあらゆる書式
* レポートのサイズや個々の列の数と幅によっては、ダッシュボードを書き出したり印刷したりすると、一部の列が切れてしまう場合があります。

## ダッシュボードの印刷

1. 印刷するダッシュボードに移動します。
1. 次のいずれかの操作を行います。

   * **ダッシュボードの操作**／**印刷**&#x200B;をクリックします。

   * **Ctrl + P** キー（Windows の場合）または **Command + P** キー（Mac の場合）を押します。

     >[!IMPORTANT]
     >
     >* ダッシュボードがカスタムタブに埋め込まれている場合、これらのオプションはどれも使用できません。カスタムタブの作成については、[カスタムタブまたはセクションの作成](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)を参照してください。
     >* Internet Explorer ブラウザーを使用している場合、キーボードショートカットオプションは使用できません。

1. 「**宛先**」フィールドで、使用可能な各種印刷オプションから選択します。\
   印刷オプションは、使用するブラウザーとブラウザーのバージョンに応じて異なります。

1. （オプション）ダッシュボードを .PDF ファイルとして保存し、「**保存**」をクリックして PDF を保存します。\
   ダッシュボードを .PDF ファイルとして保存する方法については、[ダッシュボードの書き出し](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)を参照してください。

1. 「**印刷**」をクリックします。
