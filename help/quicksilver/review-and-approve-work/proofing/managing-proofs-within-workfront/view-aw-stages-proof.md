---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 配達確認の自動ワークフローステージの表示
description: 自動ワークフローで設定された配達確認の進行状況を簡単に追跡できます。 配達確認のステージで既に実行された作業を表示、変更、追加、開始およびロックできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# 配達確認の自動ワークフローステージの表示

自動ワークフローで設定された配達確認の進行状況を簡単に追跡できます。 配達確認のステージで既に実行された作業を表示、変更、追加、開始およびロックできます。

自動ワークフローを使用した配達確認へのステージおよびユーザーの追加について詳しくは、 [配達確認の自動ワークフローへのステージおよびユーザーの追加](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

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
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## 自動ワークフロー図を表示する

1. ドキュメントを含むドキュメントリストで、ドキュメントを含む行の上にマウスポインターを置いて、 **校正ワークフロー**.

   自動ワークフローのダイアグラムがワークフロータイトルのすぐ下に表示されます。

   ダイアグラムのステージは、次のようにマークされます。

   ![dot.png](assets/dot.png) アクティブステージ

   ![gray_dot.png](assets/grey-dot.png) 非アクティブなステージ\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  プライベートステージ

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  ロックされたステージ

   ステージ間の行は、ステージ間の依存関係を表します。 非アクティブなステージに至る線は、ステージがアクティブになるまで点線で表示されます。

   ダイアグラムのステージの上にマウスポインターを置くと、その進行状況を表示できます。 ステージがアクティブでなく、ステージ上で編集権限を持っている場合は、「ステージをアクティブ化」ボタンをクリックできます ![](assets/activate-stage-btn.png) をクリックして、ステージを開始します。 ステージがアクティブで、ステージ上に編集権限がある場合は、そのステージをロックできます。 ![](assets/lock-stage-btn.png) プログレスバー (S、O、C、D) について詳しくは、  [Workfrontの配達確認での配達確認の進行状況とステータスの表示](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## ステージの表示

1. ドキュメントを含むドキュメントリストで、ドキュメントを含む行の上にマウスポインターを置いて、 **校正ワークフロー**.
1. ダイアグラムで、表示するステージをクリックします。

   ![](assets/view-stage-diagram-350x204.png)

1. ステージの詳細を展開するには、名前の下の横向き矢印をクリックします。

   ![](assets/stage-details-caret-350x167.png)

## すべてのステージを表示

自動ワークフローのすべてのステージを表示するには、次の手順に従います。

1. ページ上部の「ビューを変更」ボタンをクリックします。 ![](assets/change-view-btn.png)を選択し、「 **すべてのステージを表示**.

   自動ワークフローのすべてのステージが「 」セクションに表示されますが、詳細は非表示になっています。

1. ステージの詳細を展開するには、名前の下の横向き矢印をクリックします。

## すべてのステージの詳細を表示

自動ワークフローのすべてのステージの詳細を展開して表示するには：

1. ページ上部の「ビューを変更」ボタンをクリックします。 ![](assets/change-view-btn.png)を選択し、「 **すべてのステージの詳細を表示**.
1. ステージの詳細を表示するには、名前の下の下向き矢印をクリックします。
