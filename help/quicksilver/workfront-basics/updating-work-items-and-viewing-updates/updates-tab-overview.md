---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: アップデートセクションの概要
description: オブジェクトの「更新」(Updates) セクションには、オブジェクトに対してユーザーが行ったコメント、またはオブジェクトの変更を追跡するシステム更新が表示されます。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 3%

---


# アップデートセクションの概要

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->


>[!IMPORTANT]
>
>現在、Adobe Workfrontでのコメント作成エクスペリエンスの再設計中です。
>
>どのオブジェクトに対してコメント作成機能にアクセスするかに応じて、「更新」セクションに次の機能が表示されます。
>* 新しいエクスペリエンス
>* 従来のエクスペリエンス
>* 新しいエクスペリエンスと従来のエクスペリエンス
>
>この記事では、更新の新しいバージョンと従来のバージョンに関する情報を説明します。
>
>新しいコメントエクスペリエンスとその可用性について詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新しいコメントエクスペリエンスは、Workfrontオブジェクトの「更新」セクションでのみ使用でき、次の領域からオブジェクトにアクセスする場合は使用できません。
>
> * ホーム
> * リスト内の概要パネル
> * タイムシートの [ 概要 ] パネル
> * ワークロードバランサーの概要パネル

## アップデートセクションの概要

オブジェクトの「更新」セクションには、システムの更新と、過去 90 日以内にユーザーが行った最新の更新のうち、最大 200 個が表示されます。

![](assets/updates-tab-after-unified-experience-for-issues.png)

どのオブジェクトに対してコメント作成機能にアクセスするかに応じて、「更新」セクションに次のような操作が表示されます。

* 次のオブジェクトの新しいコメントエクスペリエンスと従来のコメントエクスペリエンスの両方：

   * プロジェクト
   * タスク（ストーリーを含む）
   * 問題
   * ドキュメント

     >[!TIP]
     >
     >「新しいコメント」オプションを使用して、新しいコメントエクスペリエンス（有効にした場合）または従来のコメントエクスペリエンス（無効にした場合）を表示します。 新しいコメントエクスペリエンスがデフォルトです。 詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* 以下に示すオブジェクトの新しいコメントエクスペリエンスのみ。 これらのオブジェクトに対して従来のコメント作成機能を有効にするオプションはありません。

   * 目標

     >[!NOTE]
     >
     >Workfrontのこの領域にアクセスするには、Adobe Workfront Goals に対する追加のライセンスが必要です。 詳しくは、 [Workfront目標の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * ボード上のカード
   * チーム
   * テンプレート
   * テンプレート タスク
   * タイムシート
   * プログラム
   * ポートフォリオ
   * ユーザー

* 次のオブジェクトに対する従来のコメントエクスペリエンスのみ：

   * イテレーション

     繰り返しの新しいコメントエクスペリエンスを有効にするオプションはありません。

### 新しいコメントエクスペリエンスの更新の節の概要

![](assets/updates-tab-after-unified-experience-for-tasks.png)

>[!NOTE]
>
>新しいコメントエクスペリエンスは、繰り返しでは使用できません。


* 「更新」セクションには、新しいコメントエクスペリエンスの次のタブに情報が表示されます。


   * **コメント**：ユーザーが行ったコメントと、そのコメントに対する返信を表示します。 「コメント」タブを使用して、新しいコメントを追加したり、既存のコメントに返信したりします。 新しいコメントエクスペリエンスでのオブジェクトの更新について詳しくは、 [作業を更新](../updating-work-items-and-viewing-updates/update-work.md).
   * **システムアクティビティ**：特定のイベントをオブジェクトに記録するためにWorkfrontが作成する情報メッセージであるシステムアップデートを表示します。 例えば、ステータス、名前、またはカスタムフィールドの変更は、システムの更新によって取り込まれます。 Workfrontまたはグループ管理者が、オブジェクトのシステム更新を有効にすることができます。 詳しくは、 [システム更新の構成](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 次のオブジェクトには「システムアクティビティ」タブはありません。

   * チーム
   * テンプレート
   * テンプレート タスク
   * アドホックカード


### 従来のアップデートの節の概要

<!--when we remove legacy, make this section an "Iterations-only" section-->

![](assets/updates-tab-before-unified-experience-for-tasks.png)

「従来の更新」セクションには、次の情報が表示されます。

* **ユーザーの更新**：ユーザーがおこなったコメント、およびそれらのコメントに対する返信。
* **システムの更新**：オブジェクトに特定のイベントを記録するためにWorkfrontが作成する情報メッセージ。 例えば、システムの更新を含むステータス、名前、またはカスタムフィールドの変更を取り込むことができます。 Workfrontまたはグループ管理者が、オブジェクトのシステム更新を有効にすることができます。 詳しくは、 [システム更新の構成](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

次のオブジェクトは、システムの更新を記録しません。

* チーム
* テンプレート
* テンプレート タスク
* イテレーション


## 上位のオブジェクトにも表示される更新

特定のオブジェクトに対するコメント、返信、またはシステム更新も、上位のオブジェクトの [ 更新 ] セクションに表示されます。

たとえば、タスクに更新を追加すると、更新がタスクの [ 更新 ] セクションと、タスクを含むプロジェクトの [ 更新 ] セクションに表示されます。

次の表に、コメントが上位のオブジェクトにも表示されるオブジェクトを示します。

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
   <td><p>ユーザー、チーム</p>
   <p><b>メモ</b></p>
   <p>タイムシートのコメントは、コメントを作成したユーザーの [ 更新 ] セクションと、ホームチームの [ 更新 ] セクションに表示されます。</p>
   </td> 
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
   <td>結果</td> 
   <td>目標</td> 
  </tr> 
  <tr> 
   <td>アクティビティ</td> 
   <td>目標</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>システム更新に追加された返信は、親オブジェクトにロールアップされません。 子オブジェクトに対する直接応答と、既存の更新に追加された返信のみが、親オブジェクトにロールアップされます。
>
>Adobe Workfrontのオブジェクト階層について詳しくは、 [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> 新しいコメントエクスペリエンスでは、システムの更新に返信できません。 詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## 更新の節の制限事項

チームの「更新」セクションでは、他のユーザーに代わって更新を入力する場合の制限事項がいくつかあります。

### ユーザーおよびチームの制限

ユーザーおよびチームの更新を表示する際は、次の点を考慮してください。

* チームの「更新」セクションで新しいコメントを追加することはできません。

* チームで表示する更新に返信を追加できます。 返信は、チームの更新セクションに表示され、返信が属するオブジェクトの更新セクションにも表示されます。

* チームの「更新」セクションには、次のオブジェクトに入力された更新が入力されます。

   * ユーザー
   * タイムシート*
   * ストーリー
   * 反復*

  *新しいコメントエクスペリエンスでは使用できません。

* ユーザーおよびチームの「更新」セクションでは、過去 90 日間に入力された更新を表示できます。

  ユーザーまたはチームに対しておこなわれたすべての更新を 90 日の制限を超えて確認する場合は、メモに関するレポートを作成できます。 ユーザーまたはチームが行った更新をすべて表示する時間フィルターをレポートに含めないでください。 詳しくは、 [カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 別のユーザーの代わりにコメントを入力する際の制限

Adobe Workfrontの管理者とグループ管理者は、他のユーザーとしてログインし、Workfrontでコメントの入力などのアクションを実行できます。

詳しくは、 [別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

別のユーザーとしてログインし、コメントを追加する際は、次の点を考慮してください。

* 別のユーザーに代わって行われたコメントは、コメントに示されます。

* グループ管理者は、別のユーザーの代わりにコメントを作成できますが、そのコメントは削除できません。 別のユーザーに代わって作成したコメントを削除できるのは、Adobe Workfront管理者のみです。

* Workfrontまたはグループ管理者は、別のユーザーとしてログアウトし、自分自身として再度ログインした場合にのみ、自分が追加したコメントを編集できます。 別のユーザーに代わってコメントを削除することはできません。

## 仕訳入力レポートを使用して作業項目のシステム更新を表示します

仕訳レポートは、プロジェクト、タスクおよび問題の更新領域からシステムの更新を表示します。

このレポートでは、次の情報を確認できます。

* ステータスの変更が発生した回数
* タスクまたはイシューが削除されたとき
* 重要なカスタムフィールドの値がプロジェクトの過程でどのように変化したか
* プロジェクトの過程で変わった重要な日付
* プロジェクトの進行中に優先度が変更された場合
* プロジェクトの所有者が変更された場合

詳しくは、 [更新領域に関するレポート](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
