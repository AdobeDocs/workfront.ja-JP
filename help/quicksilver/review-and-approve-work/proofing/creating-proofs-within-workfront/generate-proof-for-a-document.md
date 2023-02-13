---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ドキュメントの配達確認の作成
description: ドキュメントをWorkfrontにアップロードする際に、そのドキュメントの配達確認を生成できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# ドキュメントの配達確認の作成

ドキュメントをWorkfrontにアップロードする際に、そのドキュメントの配達確認を生成できます。

Adobe Workfrontに既にアップロードされているドキュメントの配達確認や、既にWorkfrontにある新しいバージョンの配達確認を生成することもできます。

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

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

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## ドキュメントのアップロードと配達確認の作成

1. 新しい配達確認を作成するプロジェクト、タスクまたは問題報告に移動します。
1. 次をクリック： **ドキュメント** タブをクリックします。
1. ドキュメントをクリック ![](assets/document-icon.png) をクリックします。
1. クリック **新規追加**&#x200B;を選択し、「 **配達確認** をクリックします。

   >[!TIP]
   >
   >次の項目を有効にすると、 **ドキュメントのアップロード時に配達確認を自動生成** を設定して、この処理を自動化します。 詳しくは、 [設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. 内 **新しい配達確認** 表示されるページで、以下の操作を実行できます。

   * [基本ワークフローを使用した詳細な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## ドキュメントをアップロードし、配達確認の新しいバージョンを作成する

1. 既存の配達確認の新しいバージョンを作成するプロジェクト、タスクまたは問題を開きます。
1. 次をクリック： **ドキュメント** タブをクリックします。
1. 新しいバージョンを追加するドキュメントを選択します。
1. クリック **新規追加** > **バージョン** > **配達確認**.
1. 内 **新しい配達確認のバージョン** 表示されるページで、以下の操作を実行できます。

   * [基本ワークフローを使用した詳細な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## ドラッグ&amp;ドロップを使用して、新しいバージョンの簡単な配達確認を生成します

ファイルシステム（デスクトップなど）からドキュメントをドラッグ&amp;ドロップして、新しい配達確認または既存の配達確認の新しいバージョンを作成できます。 配達確認には、新しい配達確認を作成するか新しいバージョンを作成するかに応じて、次の設定が含まれます。

* **新しい配達確認：** 自分とのみ共有される、簡単な配達確認を作成します。 配達確認の作成後に共有設定を変更できます。詳しくは、 [配達確認の設定を編集](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **既存の配達確認の新しいバージョン：** 以前のバージョンと同じ配達確認設定を持つ新しいバージョンを作成します。

ドラッグ&amp;ドロップを使用して新しい配達確認または新しい配達確認バージョンを生成するには：

1. 「 」の説明に従って、配達確認が自動的に生成されるように設定されていることを確認します。
1. 続行  [ファイルシステムからAdobe Workfrontにドキュメントを追加する](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)：ドキュメントを追加するドラッグ&amp;ドロップ方法を説明します。 

## 既存のドキュメントの配達確認の作成

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
      <td role="rowheader">簡易配達確認</td> 
      <td>このオプションを選択すると、ワークフローが添付されていない配達確認が作成され、デフォルトの配達確認設定が適用されます。 デフォルトの配達確認設定を更新したり、配達確認の作成後にワークフローを追加したりできます。 配達確認の設定について詳しくは、 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">配達確認の設定を編集</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">高度な配達確認</td> 
      <td> <p>このオプションを使用すると、基本または詳細ワークフローを設定し、作成する配達確認の配達確認設定を変更できます。 詳しくは、 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">基本ワークフローを使用した詳細な配達確認の作成</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">自動ワークフローを使用した高度な配達確認の作成</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
