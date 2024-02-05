---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Web プルーフビューアとデスクトッププルーフビューアの違いの概要
description: デスクトップ版と Web 版の校正ビューアの違いについて説明します。
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 98%

---

# Web プルーフビューアとデスクトッププルーフビューアの違いの概要

Adobe Workfront には 2 種類のプルーフビューアが用意されています。

* **Web プルーフビューア：**&#x200B;静的ファイルとビデオファイルのプルーフを主な目的として設計されています。Google Chrome、Firefox または Safari で動作します。
* **デスクトッププルーフビューア：**&#x200B;インタラクティブファイルとビデオおよび静的ファイルのプルーフを目的として設計されています。ワークステーションでスタンドアロンアプリケーションとして動作します。詳しくは、[デスクトッププルーフビューアについて](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)を参照してください。

* セキュリティ上の理由により組織でデスクトッププルーフビューアアプリを使用できない場合、Workfront の管理者は、ZIP アーカイブファイルにまとめられたインタラクティブコンテンツを web プルーフビューアでレビューできるようにシステムを設定できます。詳しくは、[Web プルーフビューアでのインタラクティブコンテンツのプルーフの設定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md)を参照してください。

次のリストは、特定のコンテンツタイプのプルーフに使用できるプルーフビューアを理解するのに役立ちます。

* **インタラクティブ web コンテンツ - URL**：URL を使用して web コンテンツのプルーフを作成し、コンテンツのプルーフをインタラクティブに行う場合は、デスクトッププルーフビューアを使用する必要があります。
* **インタラクティブ web コンテンツ - ZIP ファイル**：ZIP ファイルを使用して web コンテンツのプルーフを作成する場合は、web プルーフビューアを使用するか（一部制限事項あり）デスクトッププルーフビューアを使用できます。インタラクティブコンテンツに web プルーフビューアを使用する場合の制限事項については、[Web プルーフビューアでのインタラクティブコンテンツのプルーフの設定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md)を参照してください。

* **静的コンテンツとビデオコンテンツ**：静的コンテンツを含んだプルーフを作成する場合は、web プルーフビューアまたはデスクトッププルーフビューアを使用できます。

## 静的プルーフ

| **機能** | **Web プルーフビューア** | **デスクトッププルーフビューア** |
|---|---|---|
| 静的プルーフを開く | ✓ | ✓&#42; |
| 単一表示、見開き表示、連続表示 | ✓ | ✓&#42; |
| パン | ✓ | ✓&#42; |
| ズーム | ✓ | ✓&#42; |
| 回転 | ✓ | ✓&#42; |
| 測定ツール | ✓（カスタムサイズのエリアを設定） | ✓&#42; |
| サムネール表示 | ✓ | ✓&#42; |
| 静的プルーフナビゲーター | ✓ | ✓&#42; |
| ドキュメント検索 | ✓ | ✓&#42; |
| 複数ページへのコメントの投稿 | ✓（すべてのビューで使用可能） | ✓&#42;（すべてのビューで使用可能） |
| 静的プルーフの高度なショートカット | ✓（詳しくは、[プルーフビューアのキーボードショートカット](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)を参照してください） | ✓&#42;（詳しくは、[プルーフビューアのキーボードショートカット](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)を参照してください） |

{style="table-layout:auto"}

&#42; この機能は、Workfront 管理者がデスクトッププルーフビューアをすべてのプルーフのデフォルトビューアとして設定している場合にのみ有効です。

## ビデオプルーフ

| **機能** | **Web プルーフビューア** | **デスクトッププルーフビューア** |
|---|---|---|
| ビデオプルーフを開く | ✓ | ✓&#42; |
| バッファリング | ✓ | ✓&#42; |
| 時間を使用したレビュー | ✓ | ✓&#42; |
| フレームまたはタイムコードを使用したレビュー | ✓ | ✓&#42; |
| レビュー速度の増減 | ✓ | ✓&#42; |
| 音量の調節 | ✓ | ✓&#42; |
| フルスクリーンモード | ✓ | ✓&#42; |
| 範囲コメント | ✓ | ✓&#42; |
| ビデオプルーフのリピート再生（ビデオが終了すると自動的に開始） | ✓ | ✓&#42; |
| 高度なビデオショートカット | ✓（詳しくは、[プルーフビューアのキーボードショートカット](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)を参照してください） | ✓&#42; |

{style="table-layout:auto"}

&#42; この機能は、デスクトッププルーフビューアがすべてのプルーフのデフォルトビューアとして設定されている場合にのみ有効です。

## インタラクティブプルーフ

| **機能**  | **Web プルーフビューア** | **デスクトッププルーフビューア** |
|---|---|---|
| ZIP ファイルにまとめられたコンテンツから作成されたインタラクティブプルーフを開く | ✓ | ✓（推奨） |
| URL から作成されたインタラクティブプルーフを開く | サポートされていません | ✓ |
| 様々な画面サイズでインタラクティブプルーフ（ZIP ファイルにまとめられたコンテンツから作成）を表示 | ✓ | ✓ |
| 様々なデバイスに対応するインタラクティブプルーフ（ZIP ファイルにまとめられたコンテンツから作成）の表示 | サポートされていません | ✓ |
| セキュリティで保護されていない（HTTP）サイトのレビュー | サポートされていません | ✓ |
| iFrame 保護サイト（iFrame 内での表示から保護されたサイト）のレビュー | サポートされていません | ✓ |

{style="table-layout:auto"}

## コメント

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>機能</th> 
   <th>Web プルーフビューア </th> 
   <th>デスクトッププルーフビューア </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>コメントの追加、削除および編集</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>返信の追加と削除</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>長方形、矢印、線、フリーハンドおよびハイライト表示マークアップツール</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>ポリラインツール</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>切り抜きマスクマークアップツール</p> </td> 
   <td>サポートされていません</td> 
   <td>サポートされていません</td> 
  </tr> 
  <tr> 
   <td> <p>テキスト選択マークアップツール</p> </td> 
   <td>✓（静的プルーフのみ）</td> 
   <td>✓（静的プルーフのみ）</td> 
  </tr> 
  <tr> 
   <td> <p>マークアップの色の変更</p> </td> 
   <td>✓（32 色を使用可能）</td> 
   <td>✓（32 色を使用可能）</td> 
  </tr> 
  <tr> 
   <td> <p>マークアップの不透明度の変更</p> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p>マークアップの太さの変更</p> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p>マークアップの切り取り、コピーおよびペースト</p> </td> 
   <td> サポートされていません</td> 
   <td> サポートされていません</td> 
  </tr> 
  <tr> 
   <td> <p>最後の操作の取り消しおよびやり直し</p> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p>マークアップの複製</p> </td> 
   <td> サポートされていません</td> 
   <td> サポートされていません</td> 
  </tr> 
  <tr> 
   <td>コメントへのアクションの設定</td> 
   <td>✓（アクションは、アクションの設定後すぐにコメントに表示されます）</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>マークアップの色をデフォルトに設定</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>コメントを解決</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>コメントのロック</p> </td> 
   <td>サポートされていません</td> 
   <td> サポートされていません</td> 
  </tr> 
  <tr> 
   <td> <p>ユーザーのタグ付け</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>コメントの再開</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>コメントリストをコンパクトビューで表示</p> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p>標準ビュー、フルビューまたは単一ビューでコメントリストを表示</p> </td> 
   <td>今後に予定</td> 
   <td>今後に予定</td> 
  </tr> 
  <tr> 
   <td> <p>コメントの検索</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>ユーザーによるコメントのフフィルタリング</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>ユーザーによるコメントと返信のフィルタリング</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>コメントの並べ替え</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>コメントの自動更新</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 決定

| 機能 | Web プルーフビューア | デスクトッププルーフビューア |
|---|---|---|
| 意思決定 | ✓ | ✓ |
| 決定のカスタマイズ | ✓ | ✓ |

{style="table-layout:auto"}

## プルーフの比較

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>機能</th> 
   <th>Web プルーフビューア </th> 
   <th>デスクトッププルーフビューア </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プルーフの様々なバージョンの比較</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>個別のプルーフの比較</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## プルーフ操作

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>機能</th> 
   <th>Web プルーフビューア </th> 
   <th>デスクトッププルーフビューア </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プルーフのバージョンの変更</td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>新しいバージョンを作成</td> 
   <td> <p>Workfront Proof でのみ使用可能（今後 Workfront 内でのプルーフ時に予定）<br></p> </td> 
   <td>Workfront Proof でのみ使用可能（今後 Workfront 内でのプルーフ時に予定）</td> 
  </tr> 
  <tr> 
   <td>プルーフ詳細のレビュー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プルーフワークフローのレビュー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ワークフローステージの編集</td> 
   <td>サポートされていません</td> 
   <td>サポートされていません</td> 
  </tr> 
  <tr> 
   <td>プルーフの共有</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>チーム URL の取得</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>メール通知の変更</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>元のファイルをダウンロード</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プルーフとステージのロックおよびロック解除</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プルーフの概要の印刷</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プルーフの削除</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>同じフォルダーからのプルーフの管理</td> 
   <td><strong>Workfront Proof でのみ使用可能</strong> </td> 
   <td><strong>Workfront Proof でのみ使用可能</strong> </td> 
  </tr> 
  <tr> 
   <td>ブランディング（カスタムロゴ）</td> 
   <td>✓</td> 
   <td> ✓<br>（ローンチページの Workfront ロゴ） </td> 
  </tr> 
  <tr> 
   <td>カスタムリンク（Workfront Proof のみ）</td> 
   <td>サポートされていません</td> 
   <td> サポートされていません</td> 
  </tr> 
  <tr> 
   <td>Basecamp 統合（Workfront Proof のみ）</td> 
   <td>今後に予定</td> 
   <td>今後に予定</td> 
  </tr> 
  <tr> 
   <td>プレゼンスインジケーター</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プルーフの自動更新（権限の変更と新規バージョン）</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## ミニビューア

| **機能**  | **Web プルーフビューア**  | **デスクトッププルーフビューア** |
|---|---|---|
| 埋め込みコード | 静的プルーフとネイティブビデオプルーフについて今後に予定 | サポートされていません |

{style="table-layout:auto"}

## 翻訳

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>機能</strong> </th> 
   <th><strong>Web プルーフビューア</strong> </th> 
   <th><strong>デスクトッププルーフビューア</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>英語以外の言語のサポート</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
