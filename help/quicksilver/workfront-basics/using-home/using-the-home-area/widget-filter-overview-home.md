---
product-area: home
navigation-topic: new-home
title: ホームウィジェットフィルターの概要
description: 多数のウィジェットから選択して、ホームページに表示されるコンテンツをカスタマイズできます。これらのウィジェットは、ホームページ上でサイズ変更や配置が可能です。
author: Courtney
feature: Get Started with Workfront
exl-id: 58f79e81-df6b-456f-9e91-4e00a1c2a8a2
source-git-commit: 2d75f74c7281a3ea288c892db6895754a697e198
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 17%

---

# ホームウィジェットフィルターの概要

次のウィジェットに対してフィルターを使用し、作業を検索および整理できます。

* [マイプロジェクト](#my-projects)
* [マイタスク](#my-tasks)
* [マイイシュー](#my-issues)
* [担当作業](#my-work)
* [マイ承認](#my-approvals)

>[!IMPORTANT]
>
>* ホームウィジェットにタスクと問題を表示するには、その親プロジェクトが現在のステータスまたは現在と同じステータスである必要があります。
>* また、プロジェクトは、現在ステータス、または表示するのに等しいステータスである必要があります。

## マイプロジェクト

マイプロジェクトウィジェットでは以下のフィルターを使用できます。

<table>
  <tr>
    <td>アクティブ</td>
    <td>現在、予定、承認済みのステータスのプロジェクトが表示されます </td>
  </tr>
  <tr>
    <td>リスクあり</td>
    <td>「危険」ステータスのプロジェクトを表示 </td>
  </tr>
  <tr>
    <td>スケジュール遅れ</td>
    <td>「遅れているプロジェクト」ステータスを表示</td>
  </tr>
  <tr>
    <td>現在</td>
    <td>現在の状態のプロジェクトを表示します </td>
  </tr>
  <tr>
    <td>期限が今月中</td>
    <td>現在のカレンダー月に含まれる予定完了日があるプロジェクトを表示します</td>
  </tr>
  <tr>
    <td>遅延</td>
    <td>プロジェクトを遅延ステータスで表示</td>
  </tr>
  <tr>
    <td>マイプロジェクト</td>
    <td>自分または自分のプロジェクト チームに割り当てられているプロジェクトを現在の状態で表示します</td>
  </tr>
  <tr>
    <td>予定通り</td>
    <td>プロジェクトを予定通りに表示ステータス</td>
  </tr>
  <tr>
    <td>コスト予算超過</td>
    <td>実際のコストの値が予定コストの値よりも大きいプロジェクトを表示します</td>
  </tr>
  <tr>
    <td>作業予算超過</td>
    <td>[ 実績作業時間の必要条件 ] の値が [ 作業時間の必要条件 ] の値よりも大きいプロジェクトを表示します。</td>
  </tr>
  <tr>
    <td>キューのみ</td>
    <td>リクエストキューに指定されているプロジェクトを表示</td>
  </tr>
  <tr>
    <td>リクエスト日</td>
    <td>要求された状態のプロジェクトを表示します</td>
  </tr>
  <tr>
    <td>シナリオ プランナ プロジェクト</td>
    <td>シナリオ プランナで設定されたイニシアティブ ID を持つプロジェクトを表示します。</td>
  </tr>
</table>

## マイタスク

マイタスクウィジェットでは以下のフィルターを使用できます。

<table>
  <tr>
    <td>アクティブタスク</td>
    <td><p>ハンドオフ日またはハンドオフ日が今日以前のタスクを表示します。</p>
<ul>
  <li>100% 未満の完了率</li>
  <li>開始可能値は True に設定されています</li>
</ul>
</td>
  </tr>
   <!-- <tr>
    <td>All Unassigned Tasks</td>
    <td></td>
  </tr> -->
  <tr>
    <td>承認タスク</td>
    <td>タスクを承認待ち状態で表示します</td>
  </tr>
  <tr>
    <td>開始可能</td>
    <td><p>自分に割り当てられている、次のタスクを表示します</p>
<ul>
  <li>状態が完了ではありません</li>
  <li>「開始可能」の値が true の場合</li>
</ul>
</td>
  </tr>
  <tr>
    <td>クリティカルパス</td>
    <td>クリティカル タスクとして指定されたタスクを表示します</td>
  </tr>
  <tr>
    <td>未完了のタスク</td>
    <td>状態が [ 完了 ] 以外に設定されているタスクを表示します</td>
  </tr>
  <tr>
    <td>マイルストーンタスク</td>
    <td>マイルストーンに関連付けられているタスクを表示します。 詳しくは <a href="/help/quicksilver/manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md"> マイルストーンとタスクの関連付け </a> を参照してください。
</td>
  </tr>
  <tr>
    <td>マイプロジェクトタスク</td>
    <td>自分がプロジェクト チームのメンバであるタスクを [ 現在の状態 ] に表示します </td>
  </tr>
    <tr>
    <td>マイタスク</td>
    <td>自分に割り当てられているタスクを表示します</td>
  </tr>
  <tr>
    <td>反復に割り当てられていません</td>
    <td>反復に割り当てられていないタスクを表示します</td>
  </tr>
  <tr>
    <td>最近の話題</td>
    <td><p>過去 2 週間以内に最後の更新があったタスクを表示します。</p>
<ul>
  <li>コミット日が完了予定日より後です</li>
  または
  <li>プロジェクト期間が予定期間を超えています</li>
  または
  <li>状況は順調に進んでいるか、いくつかの懸念があります</li>
  または
  <li>プライマリタスクの担当者がタスクの作業を開始した</li>
</ul>
</td>
  </tr>
  <tr>
    <td>マイ役割の未割り当てタスク</td>
    <td><p>次のタスクを表示します</p>
<ul>
  <li>自分の役割に割り当てられた</li>
  <li>未完了</li>
</ul>
</td>
  </tr>
  <tr>
    <td>今後のタスク</td>
    <td><p>タスクを表示します</p>
<ul>
  <li>不完全である</li>
  <li>現在のステータスのプロジェクトに属している</li>
  <li>今日の日付から 2 週間以内に開始予定日を設定する</li>
</ul>
</td>
  </tr>
</table>

## マイイシュー

自分のイシューウィジェットでは次のフィルターを使用できます。

<table>
<tr>
    <td>すべて未割り当て</td>
    <td>未割り当てで、解決中のオブジェクトが添付されていないすべての問題を表示します </td>
  </tr>
  <tr>
    <td>自分に割り当てられている</td>
    <td>自分がプライマリ担当者である問題を表示します</td>
  </tr>
  <tr>
    <td>完了</td>
    <td>完了日に関する問題を表示 </td>
  </tr>
  <tr>
    <td>自分が入力した</td>
    <td>入力した問題を表示します</td>
  </tr>
  <tr>
    <td>マイプロジェクト問題</td>
    <td><p>問題を表示する条件</p>
<ul>
  <li>自分がプライマリ担当者です</li>
  <li>ステータスが不完全です</li>
  <li>解決するオブジェクトが添付されていません</li>
</ul>
</td>
  </tr>
    <tr>
    <td>最近送信したマイ問題</td>
    <td><p>次の問題を表示します</p>
<ul>
  <li>送信済み</li>
  <li>解決するオブジェクトが添付されていません</li>
  <li>ステータスが完了ではなく、完了日もありません</li>
  <li>今日の日付から 3 か月以内に提出されました</li>
</ul>
</td>
  </tr>
    </tr>
    <tr>
    <td>自分で送信したイシュー</td>
    <td>所有している問題を表示します</td>
  </tr>
  <tr>
    <td>開く</td>
    <td>完了日のない問題を表示します</td>
  </tr>
  <tr>
    <td>解決可能</td>
    <td>解決オブジェクトが添付されている問題を表示します</td>
  </tr>
  <tr>
    <td>マイ役割で未割り当て</td>
    <td>プライマリユーザーが割り当てられていないが、役割が割り当てられている問題をすべて表示します </td>
  </tr>
</table>

## 担当作業

自分の作業ウィジェットでは次のフィルターを使用できます。

<table>
  <tbody>
    <tr>
      <td>作業中</td>
      <td>現在作業中の項目を表示します</td>
    </tr>
    <tr>
      <td>開始準備完了</td>
      <td>項目を次で表示 
      <ul>
      <li>未完了の先行タスクまたはタスク制約はありません</li>
      <li>予定開始日が過去または最大 2 週間以内です</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>準備未完了</td>
      <td>次を持つ項目を表示
       <ul>
      <li>不完全な先行タスクまたはタスクの制約により、このアイテムは作業できません</li>
      または
      <li>予定開始日が 2 週間以上先の日付です</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>リクエスト日</td>
      <td>作業を開始していない問題を表示します</td>
    </tr>
    <tr>
      <td>私が委任済み</td>
      <td>他のユーザーに委任した項目を表示します</td>
    </tr>
    <tr>
      <td>私に委任済み</td>
      <td>ユーザーがあなたに委任した項目を表示します</td>
    </tr>
    <tr>
      <td>完了</td>
      <td>過去 2 週間以内に完了した作業を表示します。 このフィルターオプションには、承認は含まれません。</td>
    </tr>
  </tbody>
</table>

## マイ承認

自分の承認ウィジェットでは次のフィルターを使用できます。

<table>
  <tbody>
    <tr>
      <td>代理承認</td>
      <td>あなたに委任された承認が表示されます</td>
    </tr>
    <tr>
      <td>マイ承認</td>
      <td>承認が必要な項目を表示します
      </td>
    </tr>
    <tr>
      <td>送信済みの承認</td>
      <td>承認用に送信した項目を表示
       </td>
    </tr>
  </tbody>
</table>