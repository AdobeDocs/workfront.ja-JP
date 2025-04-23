---
product-area: requests
navigation-topic: create-requests
title: リクエストの作成と送信
description: 予定作業は、Adobe Workfront ではプロジェクトとタスクで表されます。ただし、予定外の作業が（ランダムなリクエストの形で）いつでも発生する可能性がある環境で作業する場合もあります。Workfront には、リクエストキューを使用してこのタイプの環境に対応するワークフローが用意されています。
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '2680'
ht-degree: 82%

---

# リクエストの作成と送信

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

予定作業は、Adobe Workfront ではプロジェクトとタスクで表されます。ただし、予定外の作業が要求という形で突然舞い込んでくる環境で働いているかもしれません。Workfront には、リクエストキューを使用してこのタイプの環境に対応するワークフローが用意されています。

リクエストキューにリクエストを作成したら、担当者に割り当てて完了させるか、タスクまたはプロジェクトに変換することができます。\
タスクまたはプロジェクトにイシューを変換する方法について詳しくは、[Adobe Workfront におけるイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

Workfront リクエストを作成するには、次の方法があります。

* 最初から（この記事ではこの場合について説明しています）。
* ドラフトから。詳しくは、[ドラフトからのリクエストの作成](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)を参照してください。
* 既存のリクエストから（コピーの送信によります）。詳しくは、[リクエストのコピーと送信](../../../manage-work/requests/create-requests/copy-and-submit-requests.md)を参照してください。

Workfront Planning でレコードを作成するには、次の方法で、Workfront Planning のリクエストをゼロから作成します。

* リンクからWorkfront計画リクエストフォームへ。

* Workfrontの「リクエスト」領域のWorkfront Planning リクエストフォームから。

  Workfront Planning パッケージを購入する必要があります。 詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：Contributor 以上</p>
   または
   <p>現在：Request 以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストキューの使用上の前提条件

この機能を使用するには、まず Workfront 管理者がリクエストキューを作成して、ユーザーが使用できるようにする必要があります。プランナーライセンスを持ち、プロジェクトへの編集アクセス権と特定のプロジェクトの管理権限を持つユーザーも、リクエストキューを作成できます。

リクエストキューの作成方法については、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

Workfront 管理者は、リクエストキューの次のコンポーネントを作成する必要があります。

* ステータスが「進行中」のプロジェクト。ヘルプリクエストキューとして公開されます。
* キュートピック\
  詳しくは、[キュートピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

* ルーティング規則\
  詳しくは、[ルーティング規則の作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)を参照してください。

* （オプション）トピックグループ\
  詳しくは、[トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)を参照してください。

* （オプション）リクエストのカスタムフォーム。\
  詳しくは、「カスタムフォームの作成 [ を参照してください ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

* （オプション）リクエストの承認プロセス。\
  詳しくは、[作業アイテムの承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)を参照してください。

## Workfront web アプリでのリクエストの作成とドラフトの生成

Workfront web アプリでリクエストを作成すると、Workfront はリクエストをドラフトとして保存してから送信します。リクエストキューを選択し、その情報の入力を開始するとすぐに、Workfront がドラフトを作成します。

引き続きリクエストを送信することもできますし、入手できる限りの情報を入力し、いったん作業を離れて後でリクエストを完了することもできます。Workfront は、開始されたドラフトリクエストをドラフトフォルダーに保存します。

>[!IMPORTANT]
>
>ドラフトを使用する際は、次の点に注意してください。
>
>* Workfront では、サードパーティのアプリケーションからリクエストを送信する際（Workfront へのメール送信や、別のアプリケーションを使用してリクエストを作成する場合など）に、ドラフトリクエストは作成されません。Workfront web アプリの外部からリクエストを送信すると、リクエストは「送信済み」セクションに保存されます。
>* リクエストキューの構造が変更されると、既存のドラフトにアクセスできなくなります。例えば、キューのトピックが削除された場合や、トピックグループが追加された場合、保存されたドラフトにはアクセスできなくなります。
>

既存のドラフトからのリクエストの作成について詳しくは、[ドラフトからリクエストを作成](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)を参照してください。リクエストドラフトの削除について詳しくは、[リクエストドラフトを削除](../../../manage-work/requests/create-requests/delete-request-draft.md)を参照してください。

Workfront web アプリでリクエストを作成するには：

{{step1-to-requests}}

1. （オプションおよび条件付き）以下の項目が組織とWorkfront インスタンスに当てはまる場合は、画面の右上にある「**新しいエクスペリエンスに切り替え**」設定を選択してください。

   * Workfront パッケージを購入している
   * 組織がAdobe統合エクスペリエンスにオンボーディングされました。
   * 管理者から、Workfront Planning へのアクセス権を付与されています
   * Workfront Planning Workspace に対して少なくとも表示権限がある

   詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください

1. ページの右上隅にある「**新規リクエスト**」をクリックします。

   >[!TIP]
   >
   >* 「新しいリクエスト」オプションには、リクエスト エリアの任意のセクションからアクセスできます。
   >* イシューを作成するためのアクセス権がない場合、「新規リクエスト」オプションはグレー表示されます。

   **新しいリクエスト** ボックスが開きます。

1. （条件付き）Workfront Planning を含む新しいエクスペリエンスに切り替えた場合、「**新規リクエスト**」ボックスに次が表示されます。</span>

   * 最近アクセスした 6 つのWorkfront リクエストキューおよび Planning リクエストフォームが「最近」セクションに表示されます。
   * 50 個の追加のWorkfront リクエストキューおよび Planning のリクエストフォームが、「すべてのリクエストフォーム **セクションにアルファベット順に表示され** す。 デフォルトで表示されないリクエストキューを検索できます。

   ![ 計画リクエスト用の統合ワークフローを備えた新しいリクエストボックス ](assets/new-request-box-with-unified-workflow-for-planning-requests.png)

   Workfront リクエストキューカードの 1 つをクリックするか、1 つを検索して、リストに表示されたらクリックします。
1. （条件付き）Workfront Planning を含む新しいエクスペリエンスに切り替えた場合は、トピックグループとキューのトピックを選択して、フォームの更新を続行します。

   それ以外の場合は、「**リクエストタイプ**」フィールド内をクリックし、次のいずれかの操作を行います。

   * 「**最近使用したパス**」セクションで、リクエストキューを開くために最近使用したパスを選択します。パスには、リクエストキュー、トピックグループ、最近送信したキューのトピックが含まれます。デフォルトでは、最後の 3 つのパスが表示されます。

     >[!NOTE]
     >
     >Workfront は、実際にリクエストを送信した場合にのみパスを保存します。ドラフトリクエストのパスは作成されません。

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * 「**リクエストキュー**」セクションで、リクエストキューを選択します。
   * 以前にアクセスしたパスに属するキーワードを入力して、リクエストキューを検索します。

     例えば、「Location」という名前のトピックグループと「Remote」という名前のキューのトピックを含む「Help Desk」という名前のリクエストキューがある場合、「remote」と入力すると、パスの要素に「remote」を含むすべてのリクエストキューが表示されます。

     >[!TIP]
     >
     >特殊文字を含む名前を入力すると、入力を省略した場合でも、リクエストキュー、キューのトピック、またはトピックグループが表示されます。

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     使用可能なリクエストキューと最近のパスのリストは、結果でハイライト表示されたキーワードを含むパスのみが含まれるように動的に更新されます。

     検索結果は、次のエリアに表示されます。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">リクエストキュー</td> 
        <td>名前にキーワードが含まれるリクエストキュー</td> 
       </tr> 
       <tr> 
        <td role="rowheader">リクエストパス</td> 
        <td> <p>要素の名前にキーワードが含まれるパス（リクエストキュー、トピックグループ、キューのトピックを含む）</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* デフォルトでは、最初の 200 件のリクエストキューがアルファベット順に表示されます。
   >* リクエストキューの名前は、ヘルプリクエストキューとして公開されたプロジェクトの名前です。
   >* 選択したリクエストキューとして設定されたプロジェクトの説明が、リクエストキュー名の右側に表示されます。
   >   
   >プロジェクトをヘルプリクエストキューとして公開する方法について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)の記事を参照してください。

1. **新しいリクエスト**&#x200B;フォームで、次のいずれかの操作を行います。

   * （条件付き）「リクエストタイプ」フィールドに表示される通知メッセージから、使用可能なドラフトを選択します。

     このエリアは、以前にドラフトを送信せずに保存したことがある場合にのみ表示されます。

     デフォルトでは、3 つの異なるキューのトピックからの 3 つの最新のドラフトが表示されます。

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * 選択したキューに新しいリクエストの入力を開始します。

     新しいリクエストの情報の入力を開始し、「件名」フィールドにリクエストに名前を付けると、新しいドラフトが「ドラフト」セクションに自動的に保存されます。

1. （オプション）リクエストキューにトピックグループが含まれる場合、最初のドロップダウンフィールドでトピックグループの名前を選択します。それ以外の場合は、キュートピックを選択します。

   >[!TIP]
   >
   >トピックグループまたはキュートピックの上にポインタを合わせると、右側に「説明」フィールドが表示されます。トピックグループまたはキューのトピックに関する追加情報が含まれます。
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >
   >

   リクエストキューには、最大 10 個のトピックグループを組み込むことができます。\
   トピックグループの作成方法について詳しくは、[トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)の記事を参照してください。キュートピックの作成について詳しくは、[キューのトピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

   >[!TIP]
   >
   >ドラフトまたは前のパスを選択した場合、トピックグループとキューのトピックは既に選択されています。必要に応じて、別のものを選択できます。

1. Workfront 管理者がプロジェクトの「**キューの詳細**」サブタブの「**新規問題フィールド**」セクションで有効にしたフィールドに応じて、新しいリクエストを送信すると、次のフィールドのいずれかが表示されることがあります。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>件名</strong> </td> 
      <td>リクエストの名前を指定します。これは必須フィールドです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>リクエストの説明を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>リクエストに関連する URL を指定します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p>リクエストの優先度を指定します。優先度は、このリクエストをどの程度の速度で解決すべきかを定義する必要があります。デフォルトのオプションは次のとおりです。 </p> 
       <ul> 
        <li>なし</li> 
        <li>低 </li> 
        <li>標準</li> 
        <li>高</li> 
        <li>緊急</li> 
       </ul> <p>優先事項の名前は、システム管理者が変更できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>重大度</strong> </td> 
      <td> <p>リクエストの重大度を指定します。重大度は、時間内に解決されない場合に、このリクエストが作業に与える影響を定義する必要があります。デフォルトのオプションは次のとおりです。</p> 
       <ul> 
        <li>一時回避</li> 
        <li>混乱を招く</li> 
        <li>対処策のあるバグ</li> 
        <li>対処策のないバグ</li> 
        <li>致命的なエラー</li> 
       </ul> <p>重大度の名前は、システム管理者が変更できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プライマリ連絡先</strong> </td> 
      <td>リクエストのプライマリ連絡先は、リクエストに関する質問に対処する時点の担当者なので、デフォルトでユーザーに設定されます。ただし、これを他の Workfront ユーザーに変更することはできます。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>割り当て</strong> </td> 
      <td> <p><span>リクエストを割り当てる必要があるアクティブなユーザー、担当業務、またはチームの名前を指定します。</span> </p> <p>1 つのチームのみを指定できます。</p>

   <p> リクエストキューの設定方法によっては、リクエストに 3 つすべてではなく、1 つまたは 2 つのタイプのリソースを割り当てることのみ可能です（例えば、リクエストをユーザーに割り当てることのみ可能です）。</p>

   <p>ルーティングルールもリクエストキューに関連付けられ、異なるタイプのリソース（チームなど）に自動的にルーティングする場合、リクエスト（ユーザー）の送信時に手動で指定したエンティティとルーティングルール（チーム）で指定したリソースの両方にリクエストが割り当てられます。 </p>

   <p> 詳しくは、次の記事を参照してください。</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">ルーティングルールの作成</a><br> </p> </li> 
      </ul> </p>

   <p><span>リクエストキューを適切なリソースに自動的にルーティングできるように、ルーティングルールをリクエストキューに使用することをお勧めします。</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>予定時間数</strong> </td> 
      <td> <p>このリクエストの完了に要する時間を見積もります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定開始日</strong> </td> 
      <td> <p>このリクエストでの作業を開始する日付を指定します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定完了日</strong> </td> 
      <td>このリクエストを解決する日付を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ステータス</strong> </td> 
      <td>新しいリクエストのデフォルトのステータスは「新規」です。システム管理者がこのステータスの名前を変更した可能性があります。このドロップダウンメニューからステータスを別のものに変更することもできます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ドキュメント</strong> </td> 
      <td> <p>リクエストにドキュメントを追加します。 </p> <p> リクエストキューの設定に応じて、カスタムフィールドの前後に「ドキュメント」セクションが表示される場合があります。 </p> <p>Workfront にアップロードしたドキュメントは、ドラフトのリクエストに 24 時間保存されます。その後、ドラフトの編集と送信に戻ったときに、それらを再添付する必要があります。他のドライブからリンクされたドキュメントは、永久にドラフトに保存されます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）Workfront 管理者がカスタムフォームをリクエストキューまたはキューのトピックに関連付けた場合、カスタムフォーム内のフィールドを指定します。\
   カスタムフォームは、Workfront インスタンスごとに異なります。
1. （オプションおよび条件付き）リクエストの入力中の任意の時点で、自動的に作成されたドラフトを削除する場合、「[!UICONTROL **ドラフトの破棄**]」をクリックします。これにより、復元できない下書きが削除されます。ドラフトの削除を確認する確認メッセージが表示されます。

1. （オプション）アクションを元に戻してドラフトを保持したい場合は、確認メッセージで「[!UICONTROL **取り消し**]」をクリックします。

1. 次のいずれかの操作を行います。

   * リクエストを送信する準備ができたら、「**送信**」をクリックします。リクエストは「送信済み」セクションに保存されます。リクエストキューのルーティングルールに応じて、このリクエストはリクエストキューとして指定されたリクエストとは異なるプロジェクトにルーティングされる場合があります。ルーティングルールについて詳しくは、[ルーティングルールの作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)を参照してください。

     または

     送信する準備がまだ整っておらず、後で戻って完了する場合は、「**閉じる**」をクリックします。リクエストは「ドラフト」セクションに保存され、次回このリクエストキューのリクエストを送信する際に利用できます。

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   リクエストを送信すると、ドラフトが自動的に削除され、復元できなくなります。

   送信されたリクエストは、リクエスト エリアの **送信済み** セクションに一覧表示されます。 Workfront Planning を含む新しいエクスペリエンスを使用している場合、Workfrontから送信されたリクエストがリクエスト エリアの **Workfront** タブに表示されます。

   受信リクエストの処理について詳しくは、[作業とチームのリクエストを管理](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)の記事を参照してください。

   送信またはドラフトのリクエストの検索について詳しくは、[送信された要求を見つける](../../../manage-work/requests/create-requests/locate-submitted-requests.md)を参照してください。

## Workfront 以外からのリクエストを作成する

新しいリクエストを送信し、他のアプリケーションに埋め込む際に、リクエストキューへの直接リンクを共有できます。Web または他のアプリケーションからこのリンクにアクセスするユーザーも、このキューにアクセスしてリクエストを送信できるように、アクティブな Workfront アカウントでログインする必要があります。詳しくは、[リクエストキューへのリンクの共有](../../../manage-work/requests/create-requests/share-link-to-request-queue.md)を参照してください。

## Workfront にメールでリクエストを作成する

リクエストキューでメールによるリクエストを受け取ることを有効にしている場合、リクエストキューに関連付けられたメールにリクエストを直接メールで送信できます。

メールの本文テキストがリクエストの説明として追加されます。

>[!NOTE]
>
>HTML の形式は、リクエストが Workfront に入ると削除されますが、署名と既存の返信先スレッドの内容は削除されず、リクエストの説明に表示されます。

リクエストキューがメールでリクエストを受け取れるようにする方法について詳しくは、[ユーザーがイシューをリクエストキュープロジェクトにメールで送信できるようにする](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md)を参照してください。

## Outlook クライアントを使用してリクエストを作成する

Outlook クライアントを使用してリクエストを送信できます。新しいリクエストを作成するか、メールをリクエストに変換することができます。

Outlook クライアントを使用してリクエストを送信する方法について詳しくは、[Outlook メールから Adobe Workfront リクエストを作成](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md)の記事を参照してください。

## Workfront モバイルアプリを使用したリクエストの作成

スマートフォンのモバイルアプリを使用してリクエストを送信できます。新しいリクエストを作成し、web アプリケーションで表示するためのアクセス権があるリクエストキューに送信できます。

モバイルアプリを使用してリクエストを送信する方法について詳しくは、この記事のリクエストの節を参照してください。

* [Android 用 Adobe Workfront](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [iOS 用 Adobe Workfront](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## 他のアプリケーションからリクエストを作成する

Workfront と統合されている任意のアプリケーションを使用して、リクエストを送信できます。

* Workfront と別のアプリケーションとの間のカスタム統合を構築し、他のアプリケーションから Workfront にリクエストを送信できます。\
  カスタム Workfront の統合について詳しくは、[Adobe Workfront 統合](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md)を参照してください。

* Salesforce 用 Workfront アプリをインストール済みの場合は、Salesforce からリクエストを送信できます。\
  Salesforce 用 Workfront アプリを使用して Salesforce からリクエストを送信する方法について詳しくは、[Salesforce オブジェクトから Adobe Workfront リクエストを送信](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)の記事を参照してください。

## Workfront計画リクエストフォームを使用したリクエストの作成

Planning リクエスト・フォームを使用して、Workfrontの Planning リクエストを追加できます。 Workfront Planning 要求を追加すると、要求フォームが承認されている場合、または承認を必要としない場合に、計画レコードが作成されることがあります。

Planning 要求を発行するには、Workfront Planning パッケージを購入する必要があります。

詳しくは、次の記事を参照してください。

* [Adobe Workfront Planning でリクエストフォームを作成および管理します ](/help/quicksilver/planning/requests/create-request-form.md)。
* [ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md)。

## 送信されたリクエストを見つける

送信またはドラフトのリクエストの検索について詳しくは、[送信されたリクエストを見つける](../../../manage-work/requests/create-requests/locate-submitted-requests.md)を参照してください。
