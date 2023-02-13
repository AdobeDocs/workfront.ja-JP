---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ZIP ファイル内のインタラクティブコンテンツの配達確認の作成
description: ZIP ファイルに保存された、Web サイト以外のインタラクティブコンテンツの配達確認を生成できます。 このタイプの Web コンテンツの例としては、ストリーミングビデオまたはオーディオを含む広告、HTMLアニメーション、インタラクティブバナーなどがあります。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# ZIP ファイル内のインタラクティブコンテンツの配達確認の作成

ZIP ファイルに保存された、Web サイト以外のインタラクティブコンテンツの配達確認を生成できます。 このタイプの Web コンテンツの例としては、ストリーミングビデオまたはオーディオを含む広告、HTMLアニメーション、インタラクティブバナーなどがあります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：プレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャ以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## ZIP ファイル内のインタラクティブコンテンツの配達確認の作成

ZIP ファイルにインタラクティブコンテンツを配達確認に追加すると、Adobe Workfrontは圧縮されたドキュメントの配達確認を作成します。 ファイルサイズに応じて、アップロードの読み込み時間は異なる場合があります。 サイズの大きいファイルは、作成に時間がかかります。 ページから移動すると、Workfrontは引き続きファイルを作成します。 最大ファイルアップロードサイズは 4GB です。 

1. ZIP バンドルファイルを作成して、コンテンツを準備します。

   ZIP ファイルは、次の要件を満たしている必要があります。

   * CSS、JavaScript、ビデオ、サウンド、画像などのすべてのアセットをバンドルファイルに含める必要があります。
   * メインファイル（index.html、index.htm など）がルートフォルダーにあり、そこに格納されている唯一の.html/.htm ファイルであることを確認します。

      メインファイルがルートフォルダーに配置されていない場合、Workfrontはそのフォルダーを検索してメインファイルを見つけます。

   * 最大バンドルサイズは 500 MB です。
   * iOSで作成された ZIP ファイルの場合、このツールはコンテンツが配置されている適切なフォルダーを自動的に識別します。

1. ZIP ファイルをアップロードするプロジェクト、タスクまたは問題報告に移動します。
1. クリック **ドキュメント** をクリックします。
1. クリック **新規追加**&#x200B;を選択し、「**配達確認** をクリックします。
1. 内 **ファイルを追加** セクションで、必要な ZIP ファイルをドラッグ&amp;ドロップまたは参照します。
1. クリック **配達確認を作成** をクリックして、確認プロセスを行わずに簡単な配達確認を作成します。\
   または\
   詳細な配達確認を設定して続行します。

   * [基本ワークフローを使用した詳細な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
