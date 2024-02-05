---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ドキュメント用のプルーフを作成する
description: ドキュメントをWorkfrontにアップロードする際に、そのドキュメントの配達確認を生成できます。 Adobe Workfront に既にアップロードされているドキュメントのプルーフや、既に Workfrontにある新しいバージョンのプルーフを生成することもできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 89%

---

# ドキュメント用のプルーフを作成する

<!-- Audited: 1/2024 -->

ドキュメントを Workfront にアップロードする際に、そのドキュメントのプルーフを生成できます。

Adobe Workfront に既にアップロードされているドキュメントのプルーフや、既に Workfrontにある新しいバージョンのプルーフを生成することもできます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>新規：任意 </p>
   <p>現在： Pro 以上</p> <p>従来のプラン：Select または Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在：作業またはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## ドキュメントのアップロードとプルーフの作成

1. 新しいプルーフを作成するプロジェクト、タスクまたはイシューに移動します。
1. 次をクリック： **ドキュメント** タブをクリックします。
1. 左側のパネルでドキュメント ![](assets/document-icon.png) をクリックします。
1. クリック **新規追加**&#x200B;を選択し、次に **配達確認** をクリックします。

   >[!TIP]
   >
   >ユーザープロファイルで「**ドキュメントのアップロード時にプルーフを自動生成**」を有効にして、この処理を自動化します。詳しくは、[個人設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)を参照してください。

1. 表示される&#x200B;**新規プルーフ**&#x200B;ページで、以下の操作を実行できます。

   * [基本ワークフローを使用した詳細なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## ドキュメントのアップロードとプルーフの新しいバージョンの作成

1. 既存のプルーフの新しいバージョンを作成するプロジェクト、タスクまたはイシューを開きます。
1. 次をクリック： **ドキュメント** タブをクリックします。
1. 新しいバージョンを追加するドキュメントを選択します。
1. クリック **新規追加** > **バージョン** > **配達確認**.
1. 表示される&#x200B;**新規プルーフバージョン**&#x200B;ページで、以下の操作を実行できます。

   * [基本ワークフローを使用した詳細なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## ドラッグ＆ドロップを使用した新しいバージョンの簡単なプルーフの生成

ファイルシステム（デスクトップなど）からドキュメントをドラッグ&amp;ドロップして、新しいプルーフまたは既存のプルーフの新しいバージョンを作成できます。プルーフには、プルーフを新規作成するか新しいバージョンを作成するかに応じて、次の設定が含まれます。

* **新規プルーフ**：自分とのみ共有される、簡単なプルーフを作成します。プルーフの作成後に共有設定を変更できます（[プルーフの設定を編集](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md)を参照）。

* **既存のプルーフの新しいバージョン**：以前のバージョンと同じプルーフ設定を持つ新しいバージョンが作成されます。

ドラッグ&amp;ドロップを使用して新しいプルーフまたは新しいプルーフバージョンを生成するには：

1. 説明に従って、プルーフが自動的に生成されるように設定されていることを確認します。
1.  [ファイルシステムからAdobe Workfrontにドキュメントを追加する](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)に進みます。これは、ドキュメントをドラッグ&amp;ドロップで追加する方法を説明します。

## 既存ドキュメントのプルーフの作成

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
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">自動ワークフローを使用した詳細プルーフの作成</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
