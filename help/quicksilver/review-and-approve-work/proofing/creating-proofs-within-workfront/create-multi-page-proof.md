---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 複数ページのプルーフを作成する
description: 複数ファイルを単一の複数ページのプルーフに結合できます。レビュアーは、プルーフビューアのナビゲーションツールを使用して、複数ページのプルーフでページを参照できます。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 96%

---

# 複数ページのプルーフを作成する

複数ファイルを単一の複数ページのプルーフに結合できます。レビュアーは、プルーフビューアのナビゲーションツールを使用して、複数ページのプルーフでページを参照できます。

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
    <p>作業またはプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 複数ページのプルーフを作成する

このオプションが有効になっている場合、静的ファイルおよび web サイトを単独のプルーフで使用できます。このオプションを無効にすると、すべてのドキュメントと web サイトは別々のプルーフとして生成され、一度に最大 100 個のファイルをアップロードできます。

複数ページのプルーフを作成するには：

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
