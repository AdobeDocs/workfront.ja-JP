---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets や Assets Essentials 用のリンクされたアセットを証明
description: Experience Manager Assets Essentials からアセットをリンクしたら、プルーフを作成し、アセットをレビューしてコメントを追加するようにユーザーを割り当てます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 78%

---

# Experience Manager Assets や Assets Essentials 用のリンクされたアセットを証明

Experience Manager Assets Essentials からアセットをリンクしたら、プルーフを作成し、アセットをレビューしてコメントを追加するようにユーザーを割り当てます。

## アクセス要件

<!-- Audited: 4/2025 -->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>標準</p>
   <p>ワークまたはそれ以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">追加製品</td> 
   <td>Experience Manager as a Cloud Service または Assets Essentials を使用するには、Admin Console に製品にユーザーとして追加されている必要があります。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示アクセス権またはそれ以上の権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

開始する前の確認事項。

* Workfront 管理者は、Experience Manager 統合を設定する必要があります。詳しくは、[Experience Manager Assets as a Cloud Service の統合を設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)または[Experience Manager Assets Essentials の統合を設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。

## プルーフを作成

静的なプルーフ、ビデオやインタラクティブなプルーフを作成できます。

プルーフを作成するには、以下のように行います。

1. プルーフが必要なプロジェクト、タスク、またはイシューに移動し、**ドキュメント**&#x200B;セクションをクリックします。
1. ドキュメントにポインタを合わせて、ドキュメント名の下に表示される&#x200B;**プルーフを作成**&#x200B;リンクをクリックします。

   >[!NOTE]
   >
   >ユーザープロファイルで&#x200B;**ドキュメントのアップロード時にプルーフを自動的に生成**&#x200B;を有効にしている場合、システムはシンプルなプルーフを自動的に作成します。

1. ドロップダウンから次のいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>シンプルなプルーフ</strong></td> 
      <td>このオプションを選択すると、ワークフローが添付されていないプルーフが作成され、デフォルトのプルーフ設定が適用されます。プルーフの作成後に、デフォルトのプルーフ設定を更新したり、ワークフローを追加したりできます。 プルーフの設定について詳しくは、<a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">プルーフの設定を編集</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>高度なプルーフ</strong></td> 
      <td> <p>このオプションを使用すると、基本的または高度なワークフローを設定し、作成するプルーフの設定を変更できます。詳しくは、以下を参照してください。 </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">基本ワークフローを使用した詳細プルーフの作成</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">自動ワークフローを使用して高度なプルーフを作成</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 既存のプルーフを管理

プルーフを作成したら、次の操作を実行できます。

* 現在のステージアクティビティを表示
* レビュアーと締め切りをアップデート
* ワークフローを編集

既存のプルーフの管理方法について詳しくは、[Adobe Workfront内でプルーフを管理する：記事インデックス &#x200B;](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md) を参照してください。

## プルーフのレビュー

割り当てられたレビュー担当者は、次の操作を行うことができます。

* アセットを表示してコメントを付ける
* コメントへのアクションの追加
* バージョンの比較
* プルーフの承認または却下

プルーフツールでできることについて詳しくは、[Adobe Workfront内でプルーフを確認する：記事のインデックス &#x200B;](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md) を参照してください。
