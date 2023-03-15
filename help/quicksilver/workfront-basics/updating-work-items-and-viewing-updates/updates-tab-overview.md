---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 「更新」タブの概要
description: 「更新」タブには、過去 90 日以内におこなわれた最新の更新のうち、最大 200 個が表示されます。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 19872953e847921c0fee6d383026641c05012ead
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 7%

---

# 「更新」タブの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

<!-- for preview commenting beta: at the release of commenting beta: change the title to: Updates section overview - also update ALL articles from which this is linked-->

「更新」タブには、過去 90 日以内におこなわれた最新の更新のうち、最大 200 個が表示されます。

次のオブジェクトに対してコメントを付けたり、更新に返信したりできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>ドキュメント</li> 
     <li>目標</li> 
     <li>問題</li> 
     <li>反復</li> 
     <li>プロジェクト</li> 
     <li>プログラム</li> 
     <li>ポートフォリオ</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>ストーリー</li> 
     <li>タスク</li> 
     <li>テンプレート</li> 
     <li>テンプレート タスク</li> 
     <li>タイムシート</li> 
     <li>ユーザー</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 上位のオブジェクトにも表示される更新

次の表に示すように、特定のオブジェクトに対して更新を行った返信も、上位のオブジェクトの [ 更新 ] タブに表示されます。

たとえば、タスクに更新を追加すると、更新がタスクの [ 更新 ] タブと、タスクを含むプロジェクトの [ 更新 ] タブに表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>元の更新が追加されたオブジェクト</strong> </th> 
   <th> <p><strong>元の更新も表示される上位のオブジェクト</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>問題</td> 
   <td>プロジェクト</td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>プロジェクト</td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>プログラム、Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ドキュメント </td> 
   <td>ドキュメントが添付されるオブジェクト、プロジェクト </td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>ポートフォリオ</td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>チーム</td> 
  </tr> 
  <tr> 
   <td>タイムシート</td> 
   <td>ユーザー、チーム</td> 
  </tr> 
  <tr> 
   <td>テンプレート タスク</td> 
   <td>テンプレート</td> 
  </tr> 
  <tr> 
   <td>ストーリー</td> 
   <td>反復、チーム</td> 
  </tr> 
  <tr> 
   <td>反復</td> 
   <td>チーム</td> 
  </tr>

<tr> 
   <td>目標</td> 
   <td>結果、アクティビティ</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>システム更新に追加された返信は、親オブジェクトにロールアップされません。 子オブジェクトに対する直接応答と、既存の更新に追加された返信のみが、親オブジェクトにロールアップされます。
>
>Adobe Workfrontのオブジェクト階層について詳しくは、 [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## 「更新」タブの制限事項

### ユーザーおよびチームの制限

チームを更新することはできません。 チームの「更新」タブには、次のオブジェクトに入力された更新が入力されます。

* ユーザー
* タイムシート
* ストーリー
* 反復

ユーザーおよびチームの「更新」タブでは、過去 90 日間に入力された更新を表示できます。

ユーザーまたはチームに対しておこなわれたすべての更新を 90 日の制限を超えて確認する場合は、メモに関するレポートを作成できます。 ユーザーまたはチームが行った更新をすべて表示する時間フィルターをレポートに含めないでください。 詳しくは、 [カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 別のユーザーの代わりにコメントを入力する際の制限

Adobe Workfrontの管理者とグループ管理者は、他のユーザーとしてログインし、Workfrontでコメントの入力などのアクションを実行できます。 ( 詳しくは、 [別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) 別のユーザーに代わって行われたコメントは、コメントに示されます。

グループ管理者は、別のユーザーの代わりにコメントを作成できますが、そのコメントは削除できません。 別のユーザーに代わって作成したコメントを削除できるのは、Adobe Workfront管理者のみです。

## 仕訳入力レポートを使用して作業項目のシステム更新を表示

仕訳レポートは、プロジェクト、タスクおよび問題の更新領域からシステムの更新を表示します。

このレポートでは、次の情報を確認できます。

* ステータスの変更が発生した回数
* タスクまたはイシューが削除されたとき
* 重要なカスタムフィールドの値がプロジェクトの過程でどのように変化したか
* プロジェクトの過程で変わった重要な日付
* プロジェクトの進行中に優先度が変更された場合
* プロジェクトの所有者が変更された場合

詳しくは、 [更新領域に関するレポート](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
