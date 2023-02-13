---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの印刷
description: ダッシュボードは、.dishboard ファイルに印刷または書き出すことができます。PDFファイルに書き出すこともできます。 ダッシュボードを印刷するには、ダッシュボードを表示する権限が必要です。
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: efae17458f2aa08ca2286ef5e43c68d1f9334b7b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# ダッシュボードの印刷

ダッシュボードは、.dishboard ファイルに印刷または書き出すことができます。PDFファイルに書き出すこともできます。 ダッシュボードを印刷するには、ダッシュボードを表示する権限が必要です。

>[!NOTE]
>
>この機能は、標準のダッシュボードビューでのみ使用します。 「プロジェクト」領域に埋め込まれたダッシュボードや、カスタムタブとして設定されたダッシュボードでは使用できません。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、およびカレンダーへのアクセスの表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong>/td&gt; 
   <td> <p>ダッシュボードに対する権限の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ダッシュボードを印刷する前に、ダッシュボードを作成する必要があります。

ダッシュボードの作成について詳しくは、 [ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## ダッシュボードを印刷する際に印刷される情報を理解する

PDFを印刷したり。ダッシュボードファイルとして保存したりすると、Adobe Workfront Web アプリケーションに表示されるダッシュボードの一部の情報が、印刷または書き出ししたファイルに表示されない場合があります。

* [何が表示されますか？](#what-is-displayed)
* [何が表示されないのか](#what-is-not-displayed)

### 何が表示されますか？ {#what-is-displayed}

印刷または書き出したダッシュボードファイルには、次の情報が含まれます。

* ダッシュボードのタイトル
* レポートのタイトル
* レポートが最後に生成された日時のタイムスタンプ
* リスト表示、外部 Web ページ、レポート、カレンダーを含む、ダッシュボード上のすべてのオブジェクト
* 会社のロゴ (Workfrontの管理者がグローバルナビゲーションバーでカスタマイズしている場合 ) Workfrontサイトのブランディングについて詳しくは、 [Adobe Workfrontインスタンスのブランディング](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### 何が表示されないのか {#what-is-not-displayed}

次の情報は、印刷または書き出しされたダッシュボードファイルには含まれません。

* Workfrontナビゲーションバー
* Workfrontに固有のその他の書式
* レポートのサイズ、個々の列の数と幅に応じて、ダッシュボードをエクスポートして印刷すると、一部の列が切れてしまう場合があります。

## ダッシュボードの印刷

1. 印刷するダッシュボードに移動します。
1. 次のいずれかの操作を行います。

   * クリック **ダッシュボードのアクション** > **印刷**

   * 押す **Ctrl+P** （Windows の場合）または **Command + P** (Mac)

      >[!IMPORTANT]
      >
      >* ダッシュボードがカスタムタブに埋め込まれている場合、これらのオプションはどちらも使用できません。 カスタムタブの作成について詳しくは、 [カスタムタブまたはセクションの作成](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
      >* Internet Explorer ブラウザーを使用している場合、キーボードショートカットオプションは使用できません。


1. 内 **宛先** 「 」フィールドで、使用可能な各種印刷オプションから選択します。\
   印刷オプションは、使用するブラウザーとブラウザーのバージョンによって異なります。

1. （オプション）ダッシュボードを。PDFファイルとして保存し、 **保存** をクリックして。PDFを保存します。\
   ダッシュボードを.dashboard ファイルとして保存する方法については、「PDF」を参照してください。 [ダッシュボードのエクスポート](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. クリック **印刷**.
