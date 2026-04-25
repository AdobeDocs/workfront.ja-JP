---
product-area: documents
navigation-topic: approvals
title: 新しいドキュメントバージョンのアップロードと承認のリクエスト
description: 新しいドキュメントのバージョンをアップロードして、Adobe Workfrontの他のユーザーに承認を依頼できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 16%

---

# 新しいドキュメントバージョンのアップロードと承認のリクエスト

以前のレビューで「作業が必要」とマークされたドキュメントの場合は、新しいバージョンを元のドキュメントにアップロードして、別の承認ラウンドを開始できます。 新しいバージョンのドキュメントをアップロードすると、以前のバージョンはロックされます。

新しいバージョンのファイル名が以前のバージョンのファイル名と異なる場合、Workfront は新しいファイル名を持つドキュメントを表示します。

未承認の文書に新しいバージョンを追加すると、以前のバージョンの承認は「撤回」と表示されます。 一部の参加者がまだ決定を下していない場合でも、以前の承認プロセスは終了します。

最新バージョンのドキュメントが削除された場合、以前のバージョンはロックされたままになります。 以前のバージョンを編集する必要がある場合は、手動でロックを解除する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>従来のWorkfrontストレージを使用して承認を管理する、あらゆるWorkfrontパッケージ</p>
<p>Adobeのエンタープライズストレージを使用して、承認を管理するあらゆるワークフローパッケージ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>リクエスト以上</p>
   <p>コントリビューター以上</p>
   <p>Frame.io統合を使用している場合は、承認ワークフローを作成するための標準ライセンスが必要です。</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントに関連付けられたオブジェクトへの編集アクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++



## ドラッグ&amp;ドロップを使用して、従来のドキュメント領域に新しいバージョンを追加します

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Workfront ストレージとAdobe エンタープライズストレージ &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)の比較を参照してください。

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。


ドキュメントのレビューと承認をもう1回行う必要がある場合は、Workfrontで新しいドキュメントのバージョンを作成できます。

以前の参加者、新しい参加者、またはその両方を追加できます。 以前のバージョンと参加者に関する情報は、ドキュメントの詳細ページで確認できます。

新しいバージョンを追加するには：

1. Workfrontでドキュメントに移動します。
1. 新しいファイルを前のドキュメントの上にドラッグ&amp;ドロップします。 これにより、自動的に新しいバージョンが作成されます。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択してドキュメント概要パネルを開きます。 ここでは、パネルの上部にバージョン番号が表示されます。
   ![&#x200B; ドキュメントの詳細ページを開く](assets/open-doc-details.png)


1. **承認** セクションまでスクロールします。

1. 「**ワークフローを作成**」をクリックし、次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、<em>初期審査</em>や<em>最終承認</em>などのより分かりやすいものに変更できます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1つの決定が必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期日（オプション）</strong></td>
   <td>承認の期日を設定します。 ユーザーとチームには、指定された期日の72時間、24時間前に電子メールで通知されます。</td>
   </tr>
   </table>

1. （オプション）前の手順を繰り返して、必要に応じてステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で進みます。 必要な決定がすべて行われると、次のステージが始まり、前のステージがロックされます。



1. （オプション）既存の承認テンプレートを追加するには、ダイアログの左側からテンプレートを選択します。

   >[!TIP]
   >
   >   標準ライセンスを持つユーザーは、設定領域から再利用可能な承認テンプレートを作成できます。 詳しくは、[&#x200B; ドキュメントの承認ワークフローテンプレートの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)を参照してください。



1. 必要なすべてのステージと参加者を追加したら、**承認を依頼**&#x200B;をクリックします。

   承認ワークフローが開始され、新しいドキュメントのバージョンで承認が必要であることを示す通知が承認者に届きます。 以前のバージョンのドキュメントはロックされ、以前のバージョンで未承認の承認は取り消されます。

   ![承認依頼](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->
