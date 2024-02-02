---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 複数ページのプルーフを作成する
description: 複数ファイルを単一の複数ページのプルーフに結合できます。レビュアーは、プルーフビューアのナビゲーションツールを使用して、複数ページのプルーフでページを参照できます。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '689'
ht-degree: 100%

---

# 複数ページのプルーフを作成する

複数ファイルを単一の複数ページのプルーフに結合できます。レビュアーは、プルーフビューアのナビゲーションツールを使用して、複数ページのプルーフでページを参照できます。

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
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンス、プルーフ権限プロファイルを確認するには、Workfront 管理者または Workfront Proof 管理者にお問い合わせください。

## 複数ページのプルーフを作成する

このオプションが有効になっている場合、静的ファイルおよび web サイトを単独のプルーフで使用できます。このオプションを無効にすると、すべてのドキュメントと web サイトは別々のプルーフとして生成され、一度に最大 100 個のファイルをアップロードできます。

複数ページのプルーフの作成方法は、次の通りです。

1. プルーフが必要なプロジェクト、タスク、またはイシューに移動し、「**ドキュメント**」セクションをクリックします。
1. **新規追加**／**プルーフ**&#x200B;をクリックします。
1. ファイルをドラッグ＆ドロップするか、ファイルエクスプローラーからファイルを参照して選択します。一度に最大 50 個のファイルをアップロードできます。ファイルの制限について詳しくは、この記事内の[考慮事項](#considerations)の節を参照してください。

   >[!NOTE]
   >
   >ビデオやインタラクティブ web サイトを含むインタラクティブファイルを結合して、単一のプルーフにすることはできません。

1. **単一のプルーフ**&#x200B;の「**互換性のあるファイルを単一のプルーフに結合**」オプションを有効にします。
1. 「**プルーフ名**」フィールドで、結合したプルーフの新しい名前を指定します。
1. （オプション）アップロードしたファイルのリストで、ファイルをドラッグして並べ替えます。ファイルの順序は、結合したプルーフのページ順です。
1. （オプション）新しいプルーフページから 1 つのファイルを削除するには、そのファイルの上にポインタを合わせて、右側に表示される&#x200B;**ごみ箱**&#x200B;アイコンをクリックします。

   または

   アップロードしたすべてのファイルを一度に削除するには、リストの右上隅にある「**すべて削除**」をクリックします。

1. すべてのファイルをアップロードしたら、基本のプルーフと自動プルーフのどちらを設定するかを決定する必要があります。

   * 基本的なプルーフを使用すると、プルーフに必要な数のレビュアーを追加できますが、レビュアーはステージ別に整理されません。追加したすべてのレビュアーは、プルーフを作成した後すぐにそのプルーフにアクセスできます。プルーフの基本を設定するには、[基本ワークフローを使用した詳細なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)を参照してください。
   * 自動プルーフを使用すると、プルーフがステージからステージに移動し、Adobe Workfront は、プルーフを確認する順番が来たことを各ユーザーに通知します。自動プルーフを設定するには、[自動ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)を参照してください。

## 考慮事項 {#considerations}

ファイルを 1 つのプルーフに結合する際は、次の点を考慮してください。

* 最大 500 個の個別のファイルをアップロードできます。
* 合計最大 2,000 ページの様々なタイプの静的ファイル（例えば、PDF、JPG、DOC、PPT、EXC）を結合することができます。
* 静的な web キャプチャを組み合わせることができます。
* GIF ファイルを組み合わせることはできますが、アニメーション GIF は静的ファイルとして処理されます。
* AV ファイルとインタラクティブ web キャプチャを組み合わせることはできません。
* プルーフのサムネール画像は、プルーフの最初のページから取得されます（[Workfront Proof でプルーフの詳細を管理](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)を参照してください）。
* プルーフの詳細ページで、プルーフ作成のために組み合わされたファイルの名前を確認します。詳しくは、[Workfront Proof でプルーフの詳細を管理](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)を参照してください。
* プルーフでオリジナルファイルをダウンロードするオプションが有効になっている場合は、プルーフを作成するために組み合わされたすべてのファイルを .zip ファイルとしてダウンロードできます。詳しくは、[Workfront Proof に保存されたファイルのダウンロード](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md)を参照してください。
