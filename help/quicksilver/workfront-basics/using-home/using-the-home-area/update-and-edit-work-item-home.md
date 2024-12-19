---
product-area: projects
navigation-topic: use-the-home-area
title: ホームエリアでの作業アイテムの更新または編集
description: Adobe Workfront の [!UICONTROL ホーム]エリア内の作業アイテムの更新を表示して追加できます。編集アクセス権がある場合は、作業アイテムに関連する他のデータを編集することもできます。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: db643781-4f52-4a8c-8c13-0bbc4c7056fd
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 35%

---

# [!UICONTROL ホーム]エリア内の作業アイテムを更新または編集する

<!--Audited: April 2024-->


<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

[!DNL Adobe Workfront] の [!UICONTROL ホーム]エリア内の作業アイテムの更新を表示して追加できます。編集アクセス権がある場合は、作業アイテムに関連する他のデータを編集することもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>新規：標準</p>
   または

<p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベルの設定</strong></td> 
   <td> <p>タスクとイシューに対する[!UICONTROL Edit]アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>作業が必要なタスクおよび問題に対するContribute以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

*ご利用のプラン、ライセンスタイプまたはアクセス権について詳しくは、[!DNL Workfront] 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--not sure if this  from the old UI: we don't have a Work List anymore - should this section come off? 

## View updates on a work item

You can view updates on any work item in the [!UICONTROL Work List]:

1. Click the **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the item where you want to view updates.\
   Updates are displayed in the right panel.

-->

## のホーム エリアでコメントを追加したり、項目を編集したりできるウィジェットの概要

「ホーム」領域の次のウィジェットにコメントを追加できます。

| ウィジェット | 説明 |
|--------------|---------------------------------------------------------------------------------------------------|
| ボード | 作成または招待したボードを表示します |
| 担当作業 | 自分に割り当てられているタスクおよび問題を表示します |
| マイプロジェクト | 所有しているプロジェクトまたは自分が参加しているプロジェクトを表示します |
| マイタスク | 自分に割り当てられているタスクを表示します |
| マイイシュー | 自分に割り当てられている問題を表示します |
| マイリクエスト | 送信したすべての要求を表示します |
| マイ承認 | 承認待ち、割り当て、委任、および送信済みのすべてを表示します |
| メンション | マイ更新ページと同様に、Workfront 全体で最近のコメントスレッドと、ウィジェット内で返信を作成できる返信ボタンを表示します。 |

ホーム領域にある次のウィジェットで作業項目を編集できます。

| ウィジェット | 説明 |
|--------------|---------------------------------------------------------------------------------------------------|
| ボード | 作成または招待したボードを表示します |
| 担当作業 | 自分に割り当てられているタスクおよび問題を表示します |
| マイプロジェクト | 所有しているプロジェクトまたは自分が参加しているプロジェクトを表示します |
| マイタスク | 自分に割り当てられているタスクを表示します |
| マイイシュー | 自分に割り当てられている問題を表示します |
| マイリクエスト | 送信したすべての要求を表示します |
| マイ承認 | 承認待ち、割り当て、委任、および送信済みのすべてを表示します |

## 担当作業ウィジェットの作業項目にコメントを追加

[!UICONTROL  担当作業 ] ウィジェットの任意の作業項目に対して更新を提供できます。

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png)、または可能であれば左上隅の&#x200B;**メインメニュー** ![](assets/lines-main-menu.png) をクリックし、「**[!UICONTROL ホーム]**」をクリックします。
1. （条件付き） **カスタマイズ** をクリックして [!UICONTROL **担当作業**] ウィジェットを追加します。

1. [!UICONTROL **担当作業**] ウィジェットで、更新する作業項目を見つけます。
1. 名前の上にマウスポインターを置き、「**新しい更新を追加** アイコンをクリックします。

   ![](assets/add-update-on-widget.png)

1. コメントを入力してください。
1. （任意）「**ユーザーまたはチームのタグ付け**」ボックスに、このコメントに含めるユーザーまたはチームの名前またはメールの入力を開始し、リストに表示されたら選択します。
1. （オプション） リッチテキストツールバーのオプションを使用してテキストの書式を設定したり、コメントに絵文字、リンクまたは画像を追加してコンテンツを充実させることができます。
1. 「**送信**」をクリックして、作業項目にコメントを追加します。

   >[!IMPORTANT]
   >
   >コメントの編集は、送信後 15 分以内に完了します。 コメントを編集するには、コメントの右上隅にある **詳細** メニューをクリックしてから、「**編集** をクリックします。

   更新の追加について詳しくは、[ 作業の更新 ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md) を参照してください。


## メンションウィジェットの項目にコメントを追加

1. **メンション** ウィジェットをホームエリアに追加します。

1. 更新に含めた項目と、返信先の項目を見つけます。

1. 「**返信**」をクリックします。

   <div class="preview">

   ![](assets/reply-to-comment-in-mentions-widget.png)

   </div>

1. コメントを入力してください。
1. （オプション）「<span class="preview">**ユーザーをタグ付け**</span>」ボックスに、このコメントに含めるユーザーまたはチームの名前の入力を開始し、リストに表示されたら選択します。
1. （オプション） リッチテキストツールバーのオプションを使用してテキストの書式を設定したり、コメントに絵文字、リンクまたは画像を追加してコンテンツを充実させることができます。
1. <span class="preview"> 「**送信**」をクリックして、作業項目にコメントを追加します。</span>

   >[!IMPORTANT]
   >
   ><span class="preview"> コメントの編集は、送信後 15 分以内に完了します。 コメントを編集するには、コメントの右上隅にある **詳細** メニューをクリックしてから、「**編集** をクリックします。</span>

   <span class="preview"> 更新の追加について詳しくは、「[ 作業の更新 ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md) を参照してください。</span>

## 作業アイテムを編集する

編集にアクセスできる任意の作業アイテムの任意のフィールドを編集できます。

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png)、または可能であれば左上隅の&#x200B;**メインメニュー** ![](assets/lines-main-menu.png) をクリックし、「**[!UICONTROL ホーム]**」をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **担当作業** ウィジェットを追加します。

1. 作業項目の上にマウスポインターを置き、「**概要** アイコンをクリックします。
   ![](assets/open-summary-new-home.png)

1. 概要パネルで、編集するフィールドの上にポインタを合わせます。
フィールドの編集権限がある場合は、フィールドにカーソルを合わせると、そのフィールドがハイライト表示されます。
1. 編集するフィールドをクリックして、必要な更新を行います。
1. フィールドの外側をクリックして、変更を保存します。
