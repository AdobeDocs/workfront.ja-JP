---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals での目標コメントの管理
description: Adobe Workfront Goals で表示できるすべての目標にコメントを追加できます。
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 72%

---

# Adobe Workfront Goals での目標コメントの管理

<!--Audited: 01/2024-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

Adobe Workfront Goals で表示できるすべての目標にコメントを追加できます。

## アクセス要件

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront プラン</td>
 <td>
 <p>任意</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront ライセンス*</td>
 <td>
 <p>新しいライセンス：寄稿者以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p> </td>
 </tr>
 <tr>
 <td role="rowheader">製品*</td>
 <td>
 <p> 新しい製品要件： Adobe Workfront Select または Prime のプランをお持ちの場合は、Adobe Workfront Goals ライセンスも追加で購入する必要があります。 Workfront目標は、Ultimate Workfrontプランに含まれます。</p>
 または
 <p>現在の製品要件：この記事で説明する機能にアクセスするには、 Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベルの設定</td>
 <td> <p>Goals に対する表示以上のアクセス権</p> <p><b>メモ</b><p>アクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 詳しくは、 <span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront目標へのアクセス権の付与</a></span></td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標に対する権限を表示またはそれ以上設定します</p>
  <p>デフォルトでは、ユーザーは目標にアクセスできません </p>
 <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
  </div> </td>
 </tr>
</tbody>
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの Workfront Goals 領域を含んだレイアウトテンプレート。

## 目標のコメントを管理

目標に対するコメントは、目標のページの「更新」セクションで追加できます。

このエリアに追加したコメントに対して、自分または他のユーザーが返信したり、「いいね！」をしたりできます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) を右上に配置するか、 **メインメニュー** アイコン ![](assets/lines-main-menu.png) 左上隅にある場合は、「 **目標**.
これにより、目標リストが開きます。
1. コメントを追加する目標を探し、その名前をクリックして目標ページを開きます。
1. 左側のパネルの「**更新**」をクリックします。
1. （オプション）既存のコメントを検索するには、キーワードの入力を開始します <!--or a user's name--> （内） **検索** ボックス **コメント** タブをクリックします。

   ![](assets/search-field-in-updates-tab-goals.png)

   キーワード <!--or user--> 検索した項目がハイライト表示され、それを含むコメントが「更新」セクションの上部に表示されます。

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >   コメントまたは返信に含まれる単語を検索する必要があります。 タグ付きユーザーまたはチームは検索できません。


   詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)

1. 次をクリック： **x** アイコンを使用して検索結果を消去し、完了時に戻ることができます。
1. 更新エリアの左上隅にある「**コメント**」タブをクリックします。
1. 「**新規コメント**」ボックスにコメントを入力し始めます。

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >コメント入力を完了して送信する前に更新セクションから移動すると、ログオフしてログオンし直した後でも、ページ上のコメントがドラフトモードのままになっています。コメントに追加された画像も下書きに保存されます。ドラフトは 7 日間保存され、その後は破棄され、復元できません。下書きのコメントは、入力したユーザーのみに表示されます。

1. （オプション）変更の取り消しまたはやり直しを行うには、以下のショートカットキーを使用します。
   * Ctrl + Z（Mac の場合は ⌘+z）で、変更を元に戻します
   * Ctrl + Y（Mac の場合は ⌘+y）で、変更をやり直します
1. （オプション）更新、ハイパーリンク、画像にリッチテキスト書式を追加するには、リッチテキストツールバーまたはその横にあるアイコンの任意のオプションを使用します。詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。
1. （オプション）**担当者またはチームのタグ付け**&#x200B;エリアで、このコメントに含めるユーザーまたはチームの名前やメールを入力して、リストに表示されたら選択します。
1. コメントが社内の担当者にのみ表示されるようにするには、「**社外秘**」切り替えスイッチを選択します。

   >[!TIP]
   >
   >このオプションを更新エリアで使用するには、プロファイルで「会社」を指定する必要があります。

1. 「**送信**」をクリックします。

   >[!TIP]
   >
   >あなたが更新している同じ項目に別のユーザーがコメントを送信すると、新しいコメントを知らせる「新規」指標が付いた赤い線が表示され、画面の下部に 新しいコメントの数を示す青い通知が表示されます。
   >
   >指標は、コメントが項目に送信された後にのみ表示され、コメントの構成中には表示されません。
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. （オプション）コメントを編集するには、「いいね！」アイコンの右側にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-icon.png) 、「**編集**」の順にクリックします。
1. コメント内の情報の編集、画像の追加や削除、タグ付きユーザーの削除を行います。
コメントは送信後 15 分間は編集できます。コメントが更新された際に表示される日付スタンプの左側に、「編集済み」のインジケーターが追加されます。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * 元の更新を送信した場合にのみ、ユーザーに更新を通知するメールが生成されます。更新を編集した後は、メールは生成されません。
   >
   > * 日付スタンプは、最新の更新日ではなく、元のコメントの日付です。

1. （オプション） **その他** メニュー ![](assets/more-icon.png)次に、次のいずれかのオプションをクリックして、コメントからクリップボードに情報をコピーするか、新しい返信に情報をコピーします。

   * **リンクをコピー**：返信を含めずに、更新のリンクをコピーします。
   * **本文をコピー**：更新のテキストをコピーします。
   * **見積もりの返信** ：新しいコメントボックスを開き、元のコメントが新しい返信で引用され、ブロック引用符としてマークされます。

     詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

1. コメントの右側にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-icon.png)、「**削除**」の順にクリックして追加したコメントを削除します。詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。
1. （オプション）「**返信**」をクリックして既存のコメントに返信し、上記の手順 5～9 に従います。更新情報の返信について詳しくは、[更新情報に返信する](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md)を参照してください。<!--insure this stays accurate-->
1. （条件付きおよびオプション）「更新」セクションの表示エリアの外側に表示されるコメントを他のユーザーが追加した場合は、画面下部の青い「**新しいコメントバナー**」内の「**表示**」をクリックして、これらのコメントを表示します。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   追加のコメントが画面の下部に表示されます。
1. （オプション）**次に類似**&#x200B;アイコン ![](assets/like-icon.png) をクリックして、他のユーザー追加したコメントに「いいね！」します。アイコンは「いいね！」の数に応じて更新されます。

1. （オプション）「**システムアクティビティ**」タブをクリックして、システムによって記録された更新を表示します。目標が更新されると、Workfront はその更新に関するメモを生成し、「システムアクティビティ」タブに表示します。Workfront は、結果、アクティビティ、またはプロジェクトが目標に追加されたときや、結果が更新されたときに、システムアップデートも記録します。<!--ensure the casing on the tab has not changed-->

