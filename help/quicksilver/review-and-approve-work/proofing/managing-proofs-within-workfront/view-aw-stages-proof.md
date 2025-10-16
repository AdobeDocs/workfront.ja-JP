---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: プルーフの自動ワークフローステージの表示
description: 自動ワークフローで設定されたプルーフの進行状況を簡単に追跡できます。プルーフのステージで既に実行された作業を表示、変更、追加、開始およびロックできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 76%

---

# プルーフの自動ワークフローステージの表示

自動ワークフローで設定されたプルーフの進行状況を簡単に追跡できます。プルーフのステージで既に実行された作業を表示、変更、追加、開始およびロックできます。

自動ワークフローのプルーフにステージおよびユーザーを追加する方法について詳しくは、[プルーフの自動ワークフローにステージとユーザーを追加](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>
   <p>任意</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p >
   <p>作業またはプラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、役割またはプルーフ権限プロファイルを確認するには、Workfront または Workfront Proof 管理者にお問い合わせください。

+++

## 自動ワークフローダイアグラムを表示

1. ドキュメントを含むドキュメントリストで、ドキュメントを含む行にポインタを合わせ、「**プルーフワークフロー**」をクリックします。

   自動ワークフローのダイアグラムが、ワークフローのタイトルの直下に表示されます。

   ダイアグラムのステージを示すマークは次のとおりです。

   ![dot.png](assets/dot.png) アクティブなステージ

   ![gray_dot.png](assets/grey-dot.png) 非アクティブなステージ\
   ![sbw-key-icon.png](assets/sbw-key-icon.png) プライベートステージ

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png) ロックされたステージ

   ステージ間の線は、ステージ間の依存関係を表します。非アクティブなステージにつながる線は、ステージがアクティブになるまで点線で示されます。

   ダイアグラム内のステージにポインタを合わせて、その進行状況を表示できます。ステージがアクティブでなく、ステージに対する編集権限がある場合は、「ステージをアクティベート」ボタン ![&#x200B; ステージをアクティベート &#x200B;](assets/activate-stage-btn.png) をクリックして、ステージを開始できます。 ステージがアクティブで、ステージの編集権限を持っている場合は、そのステージをロックできます。![&#x200B; ステージをロック &#x200B;](assets/lock-stage-btn.png) プログレスバー（S、O、C、D）について詳しくは、を参照してください。  [Workfront Proofでプルーフの進捗状況とステータスを表示します &#x200B;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)。

## ステージを表示

1. ドキュメントを含むドキュメントリストで、ドキュメントを含む行にポインタを合わせ、「**プルーフワークフロー**」をクリックします。
1. ダイアグラムで、表示するステージをクリックします。

   ![&#x200B; ステージ図を表示 &#x200B;](assets/view-stage-diagram-350x204.png)

1. ステージの詳細を展開するには、名前の下の横向き矢印をクリックします。

   ![&#x200B; ステージの詳細 &#x200B;](assets/stage-details-caret-350x167.png)

## すべてのステージを表示

自動ワークフローのすべてのステージを表示するには、次の操作を行います。

1. ページ上部の「ビューを変更」ボタン ![&#x200B; ビューを変更 &#x200B;](assets/change-view-btn.png) をクリックし、「**すべてのステージを表示**」をクリックします。

   自動ワークフローのすべてのステージがセクションに表示されますが、詳細は非表示になっています。

1. ステージの詳細を展開するには、名前の下の横向き矢印をクリックします。

## すべてのステージの詳細を表示

自動ワークフローのすべてのステージの詳細を展開して表示するには：

1. ページ上部の「ビューを変更」ボタン ![&#x200B; ビューを変更 &#x200B;](assets/change-view-btn.png) をクリックし、「**すべてのステージを詳細に表示**」をクリックします。
1. ステージの詳細を表示するには、名前の下の下向き矢印をクリックします。
