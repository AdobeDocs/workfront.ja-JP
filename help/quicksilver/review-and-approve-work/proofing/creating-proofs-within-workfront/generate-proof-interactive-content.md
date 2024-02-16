---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ZIP ファイル内のインタラクティブコンテンツのプルーフを作成
description: ZIP ファイルに保存された web サイト以外のインタラクティブコンテンツのプルーフを生成できます。このタイプの web コンテンツの例には、ストリーミングビデオまたはオーディオを含む広告、HTML アニメーション、インタラクティブバナーなどがあります。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 100%

---

# ZIP ファイル内のインタラクティブコンテンツのプルーフを作成

ZIP ファイルに保存された web サイト以外のインタラクティブコンテンツのプルーフを生成できます。このタイプの web コンテンツの例には、ストリーミングビデオまたはオーディオを含む広告、HTML アニメーション、インタラクティブバナーなどがあります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## ZIP ファイル内のインタラクティブコンテンツのプルーフを作成

ZIP ファイル内のインタラクティブコンテンツをプルーフに追加すると、Adobe Workfront によって圧縮されたドキュメントのプルーフが作成されます。ファイルサイズに応じて、アップロードの読み込み時間は異なる場合があります。ファイルのサイズが大きいと、作成に時間がかかります。ページから移動しても、Workfront はファイルの作成を続行します。最大ファイルアップロードサイズは 4 GB です。 

1. ZIP バンドルファイルを作成して、コンテンツを準備します。

   ZIP ファイルは、次の要件を満たしている必要があります。

   * CSS、JavaScript、ビデオ、サウンド、画像などのすべてのアセットをバンドルファイルに含める必要があります。
   * メインファイル（index.html、index.htm など）がルートフォルダーにあり、メインファイル以外の .html／.htm ファイルがルートフォルダーに格納されていないことを確認してください。

     メインファイルがルートフォルダーに配置されていない場合、Workfront はメインファイルを見つけるためにフォルダーを検索します。

   * 最大バンドルサイズは 500 MB です。
   * ZIP ファイルが iOS で作成された場合、このツールはコンテンツが配置されている適切なフォルダーを自動的に特定します。

1. ZIP ファイルをアップロードするプロジェクト、タスクまたはイシューに移動します。
1. 左側のパネルで「**ドキュメント**」をクリックします。
1. 「**新規追加**」をクリックし、表示されるメニューで「**プルーフ**」を選択します。
1. 「**ファイルの追加**」セクションで、必要な ZIP ファイルをドラッグ＆ドロップするか参照します。
1. 「**プルーフを作成**」をクリックして、レビュープロセスを伴わないシンプルなプルーフを作成します。\
   または\
   高度なプルーフの設定を続行します。

   * [基本ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
