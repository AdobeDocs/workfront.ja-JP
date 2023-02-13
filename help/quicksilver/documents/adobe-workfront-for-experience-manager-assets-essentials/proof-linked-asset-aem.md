---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: リンクされたアセットのExperience Manager AssetsまたはAssets Essentialsでの配達確認
description: Experience Manager Assets Essentials からアセットをリンクしたら、配達確認を作成し、そのアセットに対するレビューとコメントをユーザーに割り当てることができます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# リンクされたアセットのExperience Manager AssetsまたはAssets Essentialsでの配達確認

Experience Manager Assets Essentials からアセットをリンクしたら、配達確認を作成し、そのアセットに対するレビューとコメントをユーザーに割り当てることができます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス*</td> 
   <td> <p>仕事以上</p>
   <p>ユーザーの校正が有効になっている必要があります。</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>as a Cloud ServiceのExperience ManagerまたはAssets Essentialsがあり、ユーザーとして製品に追加されている必要があります。Admin Console。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>アクセス権以上の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

始める前に

* Workfront管理者は、統合を設定する必要があります。 詳しくは、 [Experience Manager Assets統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## プルーフを作成

静的な配達確認、ビデオ配達確認またはインタラクティブな配達確認を作成できます。

配達確認を作成するには：

1. 配達確認を行うプロジェクト、タスクまたは問題報告に移動し、 **ドキュメント** 」セクションに入力します。
1. ドキュメントの上にマウスポインターを置いて、 **配達確認を作成** ドキュメント名の下に表示されるリンク。

   >[!NOTE]
   >
   >次の場合： **ドキュメントのアップロード時に配達確認を自動生成** 「 」をユーザープロファイルで有効にすると、シンプルな配達確認が自動的に作成されます。

1. 次のいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>簡易配達確認</strong></td> 
      <td>このオプションを選択すると、ワークフローが添付されていない配達確認が作成され、デフォルトの配達確認設定が適用されます。 デフォルトの配達確認設定を更新したり、配達確認の作成後にワークフローを追加したりできます。 配達確認の設定について詳しくは、 <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">配達確認の設定を編集</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>高度な配達確認</strong></td> 
      <td> <p>このオプションを使用すると、基本または詳細ワークフローを設定し、作成する配達確認の配達確認設定を変更できます。 詳しくは、 </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">基本ワークフローを使用した詳細な配達確認の作成</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">自動ワークフローを使用した高度な配達確認の作成</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 既存の配達確認を管理

配達確認を作成したら、次のような操作を実行できます。

* 現在のステージアクティビティを表示
* レビュー担当者とデッドラインを更新
* ワークフローを編集

既存の配達確認の管理方法について詳しくは、 [Adobe Workfront内での配達確認の管理](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## 配達確認の確認

割り当てられたレビュー担当者は、

* アセットを表示してコメントを付ける
* コメントへのアクションの追加
* バージョンの比較
* 配達確認を承認または却下

校正ツールを使用して実行できる操作の詳細については、 [Adobe Workfront内での配達確認の確認](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
