---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: 無効,パブリック,共有,プルーフ,パブリック,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 公開 URL または埋め込みコードでのプルーフの共有の無効化
description: パブリック URL でプルーフを共有する機能や、プルーフごとまたは個々のユーザーごとにプルーフにコードを埋め込む機能を無効にできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '320'
ht-degree: 100%

---

# 公開 URL または埋め込みコードでのプルーフの共有の無効化

パブリック URL でプルーフを共有する機能や、プルーフごとまたは個々のユーザーごとにプルーフにコードを埋め込む機能を無効にできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Select または Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## プルーフごとに無効化

プルーフの所有者または作成者であるか、プルーフの役割が作者または進行管理者になっている必要があります。

1. プルーフを含んだプロジェクトで、左パネルの「**ドキュメント**」をクリックします。
1. プルーフにポインタを合わせて、「**ドキュメントの詳細**」を選択します。
1. 左パネルで「**プルーフ ビューアの設定**」をクリックして、「**パブリック URL または埋め込みコードによるプルーフの共有を許可**」チェックボックスをオフにします。

   ![](assets/proofing-viewer-settings-350x200.png)

1. 「**保存**」をクリックします。

## ユーザーごとに無効化

Workfront インスタンスで、個々のユーザーごとにパブリックプルーフ設定を無効にできます。この変更を行うには、管理者のプルーフ権限プロファイルが必要です。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、「**プルーフ**」をクリックします。
1. 右上隅付近にある「**アカウント設定**」をクリックします。
1. 「**ユーザー**」タブをクリックし、ユーザーの名前をクリックします。
1. 「**デフォルトのプルーフ設定**」セクションで、「**パブリック共有**」チェックボックスをオフにします。

   ![](assets/default-proof-settings--public-sharing-350x210.png)
