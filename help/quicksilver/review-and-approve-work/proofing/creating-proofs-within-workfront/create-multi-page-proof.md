---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 複数ページの配達確認の作成
description: 複数のファイルを組み合わせて、1 つの複数ページの配達確認にすることができます。 レビュー担当者は、校正ビューアのナビゲーションツールを使用して、複数ページの配達確認でページを閲覧できます。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# 複数ページの配達確認の作成

複数のファイルを組み合わせて、1 つの複数ページの配達確認にすることができます。 レビュー担当者は、校正ビューアのナビゲーションツールを使用して、複数ページの配達確認でページを閲覧できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：選択またはプレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
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

&#42;保有しているプラン、ライセンス、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfront Proof 管理者に問い合わせてください。

## 複数ページの配達確認の作成

このオプションを有効にすると、静的ファイルおよび Web サイトを 1 つの配達確認で使用できます。 このオプションを無効にすると、すべてのドキュメントと Web サイトは個々の配達確認として生成され、一度に 100 個までのファイルをアップロードできます。

複数ページの配達確認を作成するには：

1. 配達確認を行うプロジェクト、タスクまたは問題報告に移動し、 **ドキュメント** 」セクションに入力します。
1. クリック **新規追加** > **配達確認** .
1. ファイルをドラッグ&amp;ドロップするか、エクスプローラーからファイルを参照して選択します。 一度に 50 個までのファイルをアップロードできます。 ファイルの制限について詳しくは、 [注意点](#considerations) 」の節を参照してください。

   >[!NOTE]
   >
   >ビデオやインタラクティブ Web サイトを含むインタラクティブファイルを結合して、1 つの配達確認にすることはできません。

1. の下 **単一の配達確認**、オプションを有効にします。 **互換性のあるすべてのファイルを 1 つの配達確認に結合する**.
1. 内 **配達確認名** 「 」フィールドで、組み合わせ配達確認の新しい名前を指定します。
1. （オプション）アップロードしたファイルのリストで、ファイルをドラッグして並べ替えます。 ファイルの順序は、組み合わせ配達確認のページ順です。
1. （オプション）新しい配達確認ページから 1 つのファイルを削除するには、そのファイルの上にマウスポインターを置いて、 **ごみ箱** 右側に表示されるアイコン

   または

   アップロードしたすべてのファイルを一度に削除するには、 **すべて削除** をクリックします。

1. すべてのファイルをアップロードしたら、基本の配達確認と自動配達確認のどちらを設定するかを決定する必要があります。

   * 基本的な配達確認を使用すると、配達確認に必要な数のレビュー担当者を追加できますが、レビュー担当者は段階別に整理されません。 追加したすべてのレビュー担当者は、作成後すぐに配達確認にアクセスできます。 基本の配達確認を設定するには、 [基本ワークフローを使用した詳細な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * 自動配達確認を使用すると、配達確認がステージからステージに移動し、Adobe Workfrontは、配達確認を確認する順番が来たことを各ユーザーに通知します。 自動配達確認を設定するには、 [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 注意点 {#considerations}

ファイルを 1 つの配達確認に組み合わせる際は、次の点を考慮してください。

* 最大 500 個の個別のファイルをアップロードできます。
* 様々なタイプの静的ファイル (PDF、JPG、DOC、PPT、EXC など ) を、合計 2,000 ページまで組み合わせることができます。
* 静的な Web キャプチャを組み合わせることができます。
* 複数のGIF・ファイルを組み合わせるただし、アニメーションGIFは静的ファイルとして処理されます。
* AV ファイルとインタラクティブ Web キャプチャを組み合わせることはできません。
* 配達確認のサムネール画像は、配達確認の最初のページから取得されます ( [Workfront配達確認で配達確認の詳細を管理](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)) をクリックします。
* 組み合わせられたファイルの名前を確認して、配達確認の詳細ページで配達確認を作成できます。 詳しくは、 [Workfront配達確認で配達確認の詳細を管理](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* 配達確認で元のファイルをダウンロードするオプションが有効になっている場合は、組み合わされたすべてのファイルをダウンロードして、配達確認を.zip ファイルとして作成できます。 詳しくは、  [Workfront Proof に保存されたファイルのダウンロード](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
