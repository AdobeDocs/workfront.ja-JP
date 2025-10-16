---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 拡張コネクターでのリンク済みアセットのプルーフ
description: Experience Manager Assets からアセットをリンクしたら、プルーフを作成し、アセットをレビューしてコメントを追加するようにユーザーを割り当てます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 95%

---

# 拡張コネクターでのリンク済みアセットのプルーフ

Experience Manager Assets からアセットをリンクしたら、プルーフを作成し、アセットをレビューしてコメントを追加するようにユーザーを割り当てます。リンクされたアセットから作成されたプルーフは、プルーフストレージの割り当てにカウントされます。

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
   <p>ワークまたはそれ以上</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">その他の製品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントへの表示アクセス権以上</p> </td> 
  </tr> 
 </tbody> 
</table>


詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

開始する前に、

* Workfront for Experience Manager 拡張コネクタをインストール

## プルーフを作成

静的なプルーフ、ビデオやインタラクティブなプルーフを作成できます。

プルーフを作成するには、以下のように行います。

1. プルーフが必要なプロジェクト、タスク、またはイシューに移動し、**ドキュメント**&#x200B;セクションをクリックします。
1. ドキュメントにポインタを合わせて、ドキュメント名の下に表示される&#x200B;**プルーフを作成**&#x200B;リンクをクリックします。

   >[!NOTE]
   >
   >ユーザープロファイルで&#x200B;**ドキュメントのアップロード時にプルーフを自動的に生成**&#x200B;を有効にしている場合、システムはシンプルなプルーフを自動的に作成します。

1. 以下のうちのいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">シンプルなプルーフ</td> 
      <td>このオプションを選択すると、ワークフローが添付されていないプルーフが作成され、デフォルトのプルーフ設定が適用されます。プルーフの作成後に、デフォルトのプルーフ設定をアップデートしたり、ワークフローを追加したりすることができます。プルーフの設定について詳しくは、<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">プルーフの設定を編集</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">高度なプルーフ</td> 
      <td> <p>このオプションを使用すると、基本的または高度なワークフローを設定し、作成するプルーフの設定を変更できます。詳しくは、次を参照してください。 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">基本ワークフローを使用した高度なプルーフを作成</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">自動ワークフローを使用して高度なプルーフを作成</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 既存のプルーフを管理

プルーフを作成したら、以下のような操作を実行できます。

* 現在のステージアクティビティを表示
* レビュアーと締め切りをアップデート
* ワークフローを編集

既存のプルーフの管理方法について詳しくは、[Adobe Workfront 内でプルーフを管理](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)を参照してください。

## プルーフのレビュー

割り当てられたレビュアーは、以下のことを行います。

* アセットを表示してコメントを付ける
* コメントへのアクションの追加
* バージョンの比較
* プルーフの承認または却下

プルーフツールを使用して実行できる操作について詳しくは、[Adobe Workfront 内でのプルーフの確認](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)を参照してください。
