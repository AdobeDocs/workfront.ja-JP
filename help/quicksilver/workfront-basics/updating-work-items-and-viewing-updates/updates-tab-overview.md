---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: アップデートセクションの概要
description: 「更新」セクションには、過去 90 日以内におこなわれた最新の更新のうち、最大 200 個が表示されます。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# アップデートセクションの概要

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

オブジェクトの「更新」(Updates) セクションには、オブジェクトに対してユーザーが行ったコメント、またはオブジェクトの変更を追跡するシステム更新が表示されます。

## アップデートセクションの概要

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

オブジェクトの「更新」セクションには、過去 90 日以内におこなわれた最新の更新のうち、最大 200 個が表示されます。

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

「更新」セクションには、次の情報が表示されます。

* ユーザーが行ったコメントと、そのコメントへの返信。
* 特定のイベントをオブジェクトに記録するためにWorkfrontが作成する情報メッセージです。 例えば、システムの更新を含むステータス、名前、またはカスタムフィールドの変更を取り込むことができます。 Workfrontまたはグループ管理者が、オブジェクトのシステム更新を有効にすることができます。 詳しくは、 [システム更新の構成](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

次のオブジェクトの「更新」セクションが表示されます。

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

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## 上位のオブジェクトにも表示される更新

次の表に示すように、特定のオブジェクトに対して更新を行った返信も、上位のオブジェクトの [ 更新 ] セクションに表示されます。

たとえば、タスクに更新を追加すると、更新がタスクの [ 更新 ] セクションと、タスクを含むプロジェクトの [ 更新 ] セクションに表示されます。

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

## 更新の節の制限

### ユーザーおよびチームの制限

チームを更新することはできません。 チームの「更新」セクションには、次のオブジェクトに入力された更新が入力されます。

* ユーザー
* タイムシート
* ストーリー
* 反復

ユーザーおよびチームの「更新」セクションでは、過去 90 日間に入力された更新を表示できます。

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
