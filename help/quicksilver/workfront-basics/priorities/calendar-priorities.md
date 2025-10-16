---
navigation-topic: get-started-with-workfront
title: 優先度カレンダーでの作業の管理
description: わかりやすい視覚的なカレンダーで、作業を追跡します。
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: d24ad7d1-3a88-479e-beaf-69f8264c9a6b
source-git-commit: 0940e4c89de6cd3518cd98a1e06dc726f434846b
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 11%

---

# 優先度カレンダーでの作業の管理

わかりやすい視覚的なカレンダーで、作業を簡単に追跡できます。 優先度カレンダーでは、次のことができます

* フィルターを使用した作業の検索
* ステータスやフォーカスレベルなどのカスタムフィールドを適用して、優先度の高い作業を特定する
* 色を適用して素早く整理

>[!IMPORTANT]
>
>プロジェクトとその子タスクおよび問題を表示するには、プロジェクトが現在ステータスまたは現在と等しいステータスである必要があります。


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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>Reviewer 以上</p>
   <p>ライト以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>更新先のオブジェクトに対する表示または編集アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>オブジェクトに対する表示アクセス権</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 作業をカレンダーに表示します

優先度には、割り当てられた作業項目が表示されます。 チームに割り当てられた作業アイテムは優先度カレンダーに表示されません。

{{step1-to-priorities}}

1. 作業リストの上部にある **カレンダー** アイコンをクリックします。
   ![&#x200B; カレンダーアイコン &#x200B;](assets/calendar-tab.png)
1. 1 つ以上のフィルターを選択して、作業アイテムを絞り込みます。

   +++展開すると、使用可能なフィルターの詳細情報が表示されます
   <table>
    <tbody>
    <tr>
    <th>フィルター</th>
    <th>説明</th>
    </tr>
        <tr>
        <td>作業中</td>
        <td>現在作業中の項目を表示します。</td>
        </tr>
        <tr>
        <td>開始準備完了</td>
        <td>項目を次で表示 
        <ul>
        <li>未完了の先行タスクまたはタスク制約はありません</li>
        <p>and</p>
        <li>予定開始日が過去または最大 2 週間以内です</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>準備未完了</td>
        <td>次を持つ項目を表示
        <ul>
        <li>不完全な先行タスクまたはタスクの制約により、このアイテムは作業できません</li>
        <p>または</p>
        <li>予定開始日が 2 週間以上先の日付です。</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>リクエスト日</td>
        <td>作業を開始していない問題を表示します。</td>
        </tr>
        <td>完了</td>
        <td>過去 2 週間以内に完了した作業を表示します。 このフィルターオプションには、承認は含まれません。</td>
        </tr>
        <tr>
        <td>プロジェクト</td>
        <td>割り当てられたタスクまたは問題を含むプロジェクトを表示します。</td>
        </tr>
        <tr>
        <td>期日</td>
        <td>作業を完了予定日ごとに表示します。</td>
        </tr>
        <tr>
        <td>ステータス</td>
        <td>タスクまたは問題の状態（新規、進行中、完了）を表示します。</td>
        </tr>
        <tr>
        <td>マイフォーカス</td>
        <td>フォーカスレベルが割り当てられている内のタスクまたは問題を表示します。 フォーカスレベルの割り当てと管理は、個々のユーザーが行います。</td>
        </tr>
    </tbody>
    </table>

   +++

1. カレンダーの作業項目バーをクリックして、横の概要を開きます。 横の概要では、次のことができます

   * プロジェクトと作業項目の詳細の表示と編集
   * コメントの作成と表示
   * ドキュメントの表示とアップロード
   * プルーフを作成
   * Workfrontのプロジェクトページに移動します
   * 優先度の作業項目の詳細ページに移動します
   * 時間を記録
   * クイックリンクの追加

1. （オプション）「**新規作成**」をクリックして、新しい作業項目をカレンダーに追加します。 詳しくは、[&#x200B; 優先度で新しいタスクまたはイシューを作成する &#x200B;](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md) を参照してください。

## カレンダーの設定

{{step1-to-priorities}}

1. 作業リストの上部にある **カレンダー** アイコンをクリックします。
   ![&#x200B; カレンダーアイコン &#x200B;](assets/calendar-tab.png)
1. カレンダーの右隅にある **設定** アイコンをクリックします。

1. 「**バースタイル**」タブで、カレンダーの作業項目バーに表示するフィールドを最大 5 つ選択します。
   ![&#x200B; サンプルバー &#x200B;](assets/sample-task-for-field-config.png)

1. **カラー** タブで、作業項目の表示方法を選択します。 例えば、「**プロジェクト** を選択すると、作業リストのプロジェクトに割り当てられたカラーに従って作業項目が表示されます。
   ![&#x200B; サンプルカラープロジェクト &#x200B;](assets/sample-calendar-projects.png)
