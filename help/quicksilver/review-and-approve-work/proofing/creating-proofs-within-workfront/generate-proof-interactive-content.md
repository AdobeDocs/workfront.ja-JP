---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ZIP ファイル内のインタラクティブコンテンツのプルーフを作成
description: ZIP ファイルに保存された web サイト以外のインタラクティブコンテンツのプルーフを生成できます。 このタイプの web コンテンツの例には、ストリーミングビデオまたはオーディオを含む広告、HTML アニメーション、インタラクティブバナーなどがあります。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
TQID: https://experienceleague.adobe.com/wJNC4pCRhTpOfoiB1X6-6vKrYvWA2EaR-x2HfhwcDaY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 93%

---

# ZIP ファイル内のインタラクティブコンテンツのプルーフを作成

ZIP ファイルに保存された web サイト以外のインタラクティブコンテンツのプルーフを生成できます。 このタイプの web コンテンツの例には、ストリーミングビデオまたはオーディオを含む広告、HTML アニメーション、インタラクティブバナーなどがあります。

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
   <p>作業または計画</p> 
   </td> 
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

## ZIP ファイル内のインタラクティブコンテンツのプルーフを作成

ZIP ファイル内のインタラクティブコンテンツをプルーフに追加すると、Adobe Workfrontは圧縮されたドキュメントのプルーフを作成します。ファイルサイズに応じて、アップロードの読み込み時間が異なる場合があります。大きなファイルの作成には時間がかかります。ページから移動すると、Workfrontで引き続きファイルを作成できます。 最大ファイルアップロードサイズは4GBです。 

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
