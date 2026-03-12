---
product-area: documents
navigation-topic: approvals
title: 新しいドキュメントバージョンのアップロードと承認のリクエスト
description: 新しいドキュメントバージョンをアップロードし、Adobe Workfrontの他のユーザーの承認をリクエストできます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 15%

---

# 新しいドキュメントバージョンのアップロードと承認のリクエスト

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

以前のレビューでドキュメントに「作業が必要」とマークされた場合、元のドキュメントに新しいバージョンをアップロードし、別の承認を開始できます。 新しいバージョンのドキュメントをアップロードすると、以前のバージョンがロックされます。

新しいバージョンのファイル名が以前のバージョンのファイル名と異なる場合、Workfront は新しいファイル名を持つドキュメントを表示します。

承認が未処理のドキュメントに新しいバージョンが追加されると、以前のバージョンの承認は「撤回済み」と表示されます。 一部の参加者がまだ決定を行っていない場合でも、前回の承認プロセスが終了します。

最新バージョンのドキュメントを削除しても、以前のバージョンはロックされたままになります。 旧バージョンを編集する必要がある場合は、手動でロックを解除する必要があります。

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
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>リクエスト以上</p>
   <p>コントリビューター以上</p>
   <p>Frame.io 統合を使用している場合、承認ワークフローを作成するには Standard ライセンスが必要です。</p>
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


## ドラッグ&amp;ドロップを使用して、実稼動環境に新しいバージョンを追加します

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。


ドキュメントに対する別のラウンドのレビューと承認が必要な場合は、Workfrontで新しいドキュメントバージョンを作成できます。

以前の参加者、新しい参加者または両方を追加できます。 以前のバージョンと参加者に関する情報は、「ドキュメントの詳細」 ページで表示できます。

新しいバージョンを追加するには：

1. Workfrontのドキュメントに移動します。
1. 新しいファイルを前のドキュメントの上にドラッグ&amp;ドロップします。 これにより、新しいバージョンが自動的に作成されます。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択し、「**ドキュメントの詳細**」をクリックします。
   ![ ドキュメントの詳細ページを開く ](assets/open-doc-details.png)


1. 左側のパネルで「**承認**」をクリックし、「**追加**」をクリックします。

1. 以前の参加者をすべて追加するには、「**すべてを追加**」をクリックします。 必要に応じて、新しい参加者を追加したり、以前の参加者を削除したりすることもできます。


1. 既存の承認テンプレートを追加するには、「テンプレート」ボタンをクリックしてテンプレート名の入力を開始します。

   >[!TIP]
   >
   >   Standard ライセンスを持つユーザーは、設定領域から再利用可能な承認テンプレートを作成できます。 詳しくは、[ ドキュメント用の承認ワークフローテンプレートの作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) を参照してください。


1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. すべてのレビュー担当者と承認者を追加したら、「**リクエストを送信**」をクリックします。 参加者には、メールで通知されます。

   ![ 承認用に新しいバージョンを送信 ](assets/add-previous-participants.png)





<div class="preview">

## プレビュー環境のレガシードキュメント領域に新しいバージョンを追加するには、ドラッグ&amp;ドロップを使用します

組織がWorkfront ストレージ上にある場合、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Workfront ストレージとAdobe エンタープライズストレージの比較 ](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage) を参照してください。

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。


ドキュメントに対する別のラウンドのレビューと承認が必要な場合は、Workfrontで新しいドキュメントバージョンを作成できます。

以前の参加者、新しい参加者または両方を追加できます。 以前のバージョンと参加者に関する情報は、「ドキュメントの詳細」 ページで表示できます。

新しいバージョンを追加するには：

1. Workfrontのドキュメントに移動します。
1. 新しいファイルを前のドキュメントの上にドラッグ&amp;ドロップします。 これにより、新しいバージョンが自動的に作成されます。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択してドキュメントの概要パネルを開きます。 ここでは、パネルの上部にバージョン番号が表示されます。
   ![ ドキュメントの詳細ページを開く ](assets/open-doc-details.png)


1. 「**承認** セクションまでスクロールします。

1. **ワークフローを作成** をクリックし、次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、「最初のレビュー」や「<em> 最終承認 </em> など、よりわかりやすい名前 <em> 変更 </em> きます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>ユーザー名またはチーム名の入力を開始して、承認者またはレビュアーとして追加します。 レビュー担当者のみが存在する場合、レビュー担当者に通知され、レビューを完了するオプションが提供されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1 つの決定が必要（オプション）</strong></td>
   <td>最初に決定を行ったユーザーがステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>承認期限を設定します。 ユーザーとチームには、指定した期日の 72 時間前、つまり 24 時間前にメールで通知が届きます。</td>
   </tr>
   </table>

1. （オプション）必要に応じて、前の手順を繰り返して追加のステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で続行されます。 必要な決定がすべて行われると、次のステージが開始され、前のステージがロックされます。



1. （オプション）既存の承認テンプレートを追加するには、ダイアログの左側からテンプレートを選択します。

   >[!TIP]
   >
   >   Standard ライセンスを持つユーザーは、設定領域から再利用可能な承認テンプレートを作成できます。 詳しくは、[ ドキュメント用の承認ワークフローテンプレートの作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) を参照してください。



1. 必要なすべてのステージと参加者を追加したら、「**承認をリクエスト**」をクリックします。

   承認ワークフローが開始し、新しいドキュメントバージョンで承認が必要であるという通知が承認者に届きます。 以前のドキュメントバージョンがロックされ、以前のバージョンに対する未処理の承認が取り消されます。

   ![ リクエストの承認 ](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->



</div>

