---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの印刷
description: ダッシュボードを印刷したり .PDF ファイルに書き出したりできます。ダッシュボードを印刷するには、ダッシュボードを表示する権限が必要です。
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 95%

---

# ダッシュボードの印刷

<!-- Audited: 1/2025 -->

ダッシュボードを印刷したり .PDF ファイルに書き出したりできます。ダッシュボードを印刷するには、ダッシュボードを表示する権限が必要です。

>[!NOTE]
>
>この機能は、標準のダッシュボードビューでのみ使用できます。プロジェクトエリアに埋め込まれたダッシュボードや、カスタムタブとして設定されたダッシュボードでは使用できません。

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
   <td> 
      <p>標準</p>
      <p>ワークまたはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボードおよびカレンダーへのアクセスを編集する</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ダッシュボードの表示権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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

   * **ダッシュボード アクション**/**印刷プレビュー** をクリックします

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
