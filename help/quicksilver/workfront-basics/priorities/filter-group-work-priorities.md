---
navigation-topic: get-started-with-workfront
title: 優先度を使用した作業のフィルタリングとグループ化
description: フィルターを使用して作業を検索し、グループ化を適用して整理することができます。
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 75396c3f066abc6070ae2a89c2ded0255dbc0751
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 18%

---


# 優先度を使用した作業のフィルタリングとグループ化

フィルターを使用して探している作業を見つけ、グループ化を適用して整理することができます。

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
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> 
   <p>現在：Request 以上</p>
   <p>新規：Contributor 以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>更新先のオブジェクトに対する表示または編集アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトに対する表示アクセス権</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 作業をフィルター

自分に割り当てられたタスクやイシューをフィルタリングできます。

{{step1-to-priorities}}

1. ワークリストの右上にある「**フィルター**」をクリックします。
1. 1 つまたは複数のフィルターを選択して、作業アイテムを絞り込みます。
   ![](assets/filters.png)

+++展開すると、使用可能なフィルターの詳細情報が表示されます
<table>
  <tbody>
   <tr>
   <th>フィルター</th>
   <th>説明</th>
   </tr>
    <tr>
      <td>作業中</td>
      <td>現在作業中の項目を表示します</td>
    </tr>
    <tr>
      <td>開始準備完了</td>
      <td>項目を次で表示 
      <ul>
      <li>未完了の先行タスクまたはタスク制約はありません</li>
      <p>および</p>
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
      <li>予定開始日が 2 週間以上先の日付です</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>リクエスト日</td>
      <td>作業を開始していない問題を表示します</td>
    </tr>
      <td>完了</td>
      <td>過去 2 週間以内に完了した作業を表示します。 このフィルターオプションには、承認は含まれません。</td>
    </tr>
    <tr>
    <td>プロジェクト</td>
    <td>割り当てられたタスクまたは問題を含むプロジェクトを表示します</td>
    </tr>
    <tr>
    <td>期限日</td>
    <td>作業を予定完了日別に表示</td>
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

1. （任意）「**デフォルトに戻る**」をクリックして、選択をリセットします。

## 作業のグループ化

{{step1-to-priorities}}

1. ワークリストの右上にある「**グループ**」をクリックします。
1. 作業リストを整理するグループを選択
   ![](assets/groups.png)

+++展開すると、利用可能なグループの詳細情報が表示されます

| グループ | 説明 |
|-----------|-------------|
| なし | これにより、ワークリストからグループ化が削除されます。 |
| マイフォーカス | これにより、割り当てたフォーカスレベルに基づいて項目がグループ化されます。 |
| 期限の週 | これにより、期限の週に基づいて項目がグループ化されます。 期限は予定完了日によって決定されます。 |
| ステータス | これは、新規、処理中、完了のステータスで項目をグループ化します。 <br> メモ：現時点では、優先度でカスタムステータスを使用することはできません。 |
| プロジェクト | これにより、プロジェクトごとに項目がグループ化されます。 |

+++

## 作業の並べ替え

作業を並べ替えるには、**グループ** を開き、**昇順で並べ替え** または **降順で並べ替え** をクリックします。

![](assets/expand-sort-groups.png)

>[!IMPORTANT]
>
>グループを適用している場合、並べ替えオプションは一時的に使用できません。



## すべてのセクションを展開または折りたたむ

すべてのセクションを展開または折りたたむには、**グループ** を開いて **すべて展開** または **すべて折りたたむ** をクリックします。

![](assets/expand-sort-groups.png)

