---
product-area: reporting
navigation-topic: using-built-in-reports
title: Adobe Workfront の組み込みレポートを使用する
description: Adobe Workfrontには、すぐに使用できるビルトインレポートの広範なリストが用意されています。 Workfront 管理者は、組み込みのレポートを非表示にして、ユーザーがアクセスできないようにすることができます。
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '2986'
ht-degree: 56%

---

# Adobe Workfront の組み込みレポートを使用する

<!--Audited: 11/2024-->

Adobe Workfront には、ユーザーが使用できる組み込みレポートの大量のリストが用意されています。

Workfront管理者は、ビルトインレポートを非表示にして、ユーザーがアクセスできないようにすることができます。 組み込みレポートを非表示にする方法について詳しくは、[組み込みレポートを非表示にする](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>投稿者以上</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>リクエスト以上</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>報告書、ダッシュボード、カレンダーへの表示以上のアクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理し、レポートに対するフィルターを追加または編集</p> <p>フィルターに対する権限を管理し、リストで編集</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 組み込みレポートの概要 {#overview-of-built-in-reports}

組み込みレポートのコピーを作成して、新しいレポートとして保存できます。 組み込みレポートのコピーを作成する方法の詳細については、「[ レポートのコピーを作成する ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#create-a-new-version-of-a-report)」の [ 新しいバージョンのレポートを作成する ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md) を参照してください。

Workfront パッケージには、次のレポートが付属しています。これらのレポートは、最低でもアクセスレベルで組み込みレポートの表示権限を持つすべてのユーザーが利用可能です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>レポート名</strong> </th> 
   <th><strong>レポートの説明</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ポートフォリオ実コスト（プログラム別）</td> 
   <td>プロジェクトの予定コストと実際のコストを表示するプロジェクト報告書。 レポートは、プログラム名（ポートフォリオ名でプロンプトが表示されます）でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ実コスト（プロジェクト別）</td> 
   <td>プロジェクトの予定コストと実際のコストを表示するプロジェクト報告書。 レポートは、プロジェクト名（ポートフォリオ名でプロンプトが表示されます）でグループ化され、グラフを含みます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ実収益（プログラム別）</td> 
   <td>プロジェクトの予定収益と実収益を表示するプロジェクト報告書。 レポートは、プログラム名（ポートフォリオ名でプロンプトが表示されます）でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ実収益（プロジェクト別）</td> 
   <td>プロジェクトの予定収益と実収益を表示するプロジェクト報告書。 レポートは、プロジェクト名（ポートフォリオ名でプロンプトが表示されます）でグループ化され、グラフを含みます。</td> 
  </tr> 
  <tr> 
   <td>実収益 (会社)</td> 
   <td>プロジェクトの実収益と会社を表示するプロジェクト報告書。 レポートは会社名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>実収益（グループ別）</td> 
   <td>プロジェクトの実収益とグループを表示するプロジェクト報告書。 レポートはグループ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>すべてのオープン タイムシート</td> 
   <td>オープン タイムシートを表示するタイムシート報告書。 レポートには、タイムシートの日付範囲、所有者の名前、合計時間数、時間外、承認者の名前、ステータスの各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>承認タイムシート (確認)</td> 
   <td>承認者付きの送信済みタイムシートまたは拒否されたタイムシートを表示するタイムシート報告書。 レポートには、タイムシートの日付範囲、所有者、合計時間数、残業、承認者名およびステータスの各フィールドが表示されます。レポートは、タイムシート開始日、タイムシート終了日、タイムシート承認者名およびユーザー名によって要求されます。</td> 
  </tr> 
  <tr> 
   <td>危険プロジェクト</td> 
   <td>状況が [ 危険あり ] または [ トラブル発生中 ] である、現在および計画中のプロジェクトを表示するプロジェクト報告書。 レポートには、プロジェクトの説明、予定完了日、完了見込日、完了率、ステータスおよび優先度の各フィールドが表示されます。レポートはポートフォリオ名でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>請求収益（会社別）</td> 
   <td>プロジェクトの会社と請求収益を表示するプロジェクト報告書。 レポートは会社名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>請求収益（グループ別）</td> 
   <td>プロジェクトの請求収益とグループを表示するプロジェクト報告書。 レポートはグループ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>請求収益（月別）</td> 
   <td>請求記録のプロジェクト名、プロジェクト請求収益、および請求日を表示する請求記録報告書。 このレポートは、請求レコードの請求日の月ごとにグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>完了したイシュー（週別）</td> 
   <td>問題の実際の完了日を表示する問題報告書。 レポートは、イシューの実際の完了日の週ごとにグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>完了したイシュー（週別ユーザー別）</td> 
   <td>問題の実際の完了日と割り当てを表示する問題報告書。 レポートは、プライマリ担当者別およびイシューの実際の完了日の週別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>進行中のプロジェクト</td> 
   <td>現在のすべてのプロジェクトを表示するプロジェクト報告書。 レポートには、プロジェクトの説明、予定完了日、完了見込日、完了率、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>時間コスト（ユーザーおよび月別）</td> 
   <td>ログ時間数とその実際のコストを表示するマトリックス時間報告書。 レポートは、所有者名とその時間のエントリ日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>時間数（ユーザー別）</td> 
   <td>ログ時間数を表示する時間報告書。 レポートは所有者名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>時間数（ユーザー別週別）</td> 
   <td>過去 4 週間のログ時間数とその時間のエントリ日を表示するマトリックス時間報告書。 レポートは、その時間のエントリ日によってプロンプトが表示され、所有者名と、その時間のエントリ日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>イシュー（ステータス別）</td> 
   <td>問題の状態を表示する問題報告書。 レポートは、イシューのステータス別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>イシュー（ステータスおよびプロジェクト別）</td> 
   <td>現在のプロジェクトに含まれている問題の状態とプロジェクト名を表示するマトリックス問題報告書。 レポートは、イシューのプロジェクト名およびステータス別にグループ化されています。</td> 
  </tr> 
  <tr> 
   <td>労力コスト対費用コスト（ポートフォリオ別）</td> 
   <td>プロジェクトの予定労力コスト、実際の労力コスト、予定費用コスト、および実際の費用コストを表示するプロジェクト報告書。 レポートはポートフォリオ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>労力コスト対費用コスト（プログラム別）</td> 
   <td>プロジェクトの予定労力コスト、実際の労力コスト、予定費用コスト、および実際の費用コストを表示するプロジェクト報告書。 レポートは、ポートフォリオ名とプログラム名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>月次ポートフォリオ予定コスト対実コスト（プロジェクト別）</td> 
   <td>プロジェクトの配分日、予定コストの合計、実際のコストの合計、およびコスト差異の合計を表示するマトリックス プロジェクト （財務データ）報告書。 レポートは、プロジェクト名、四半期および配分日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>月次ポートフォリオ予定収益対実収益（プロジェクト別）</td> 
   <td>プロジェクトの配分日、予定収益の合計、実収益の合計、および収益差異の合計を表示するマトリックス プロジェクト （財務データ）報告書。 レポートは、プロジェクト名、四半期および配分日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>月次プロジェクト予定コスト対実コスト</td> 
   <td>プロジェクトの配分日、予定コストの合計、実際のコストの合計、およびコスト差異の合計を表示するマトリックス プロジェクト （財務データ）報告書。 レポートは、プロジェクト名、四半期、配分日の月でグループ化され、プロジェクト名でプロンプトが表示されます。</td> 
  </tr> 
  <tr> 
   <td>月次プロジェクト予定収益対実収益</td> 
   <td>プロジェクトの配分日、予定収益の合計、実収益の合計、および収益差異の合計を表示するマトリックス プロジェクト （財務データ）報告書。 レポートは、プロジェクト名、四半期、配分日の月でグループ化され、プロジェクト名でプロンプトが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイドキュメント</td> 
   <td>ログイン ユーザーがアップロードしたドキュメントを表示するドキュメント報告書。 レポートには、ドキュメントの所有者名、変更日、サイズ、バージョン数、ソースおよびタイプの各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>お気に入り</td> 
   <td>ログイン ユーザーがお気に入りとしてマークしたオブジェクトの一覧を表示するお気に入り報告書。 レポートには、オブジェクトタイプおよびお気に入りの名前の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイイシュー</td> 
   <td>ログインしたユーザーに割り当てられた、未完了の問題を表示する問題報告書。 レポートには、イシューのソース名、イシュータイプ、プライマリ担当者、エントリ日、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイポートフォリオ</td> 
   <td>ログイン ユーザーがPortfolio Manager である、アクティブなポートフォリオを表示するPortfolio報告書。</td> 
  </tr> 
  <tr> 
   <td>マイプログラム</td> 
   <td>ログイン ユーザーがプログラム マネージャーであるプログラムとその説明を表示するプログラム報告書。</td> 
  </tr> 
  <tr> 
   <td>マイプロジェクトのオープンイシュー</td> 
   <td>ログイン ユーザーが含まれているプロジェクト チームのプロジェクトで未完了の問題を表示する問題報告書。 レポートには、イシューのソース名、イシュータイプ、プライマリ担当者、エントリ日、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイプロジェクト</td> 
   <td>ログイン ユーザーが含まれているプロジェクト チームの現在のプロジェクトを表示するプロジェクト報告書。 レポートには、プロジェクトの説明、予定完了日、完了見込日、完了率、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>自分で送信したイシュー</td> 
   <td>ログイン ユーザーが送信した問題で、過去 3 か月間にクローズしたものか現在もオープンであるものを表示する問題報告書。 レポートには、イシューのソース名、イシュータイプ、エントリ日、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイタスク</td> 
   <td>ログイン ユーザーに割り当てられた、現在のプロジェクトで未完了タスクを表示するタスク報告書。 レポートには、タスクの予定期間、プロジェクト名、プライマリ担当者、開始予定、完了予定、完了率、優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイタイムシート</td> 
   <td>ログイン ユーザーのタイムシートをすべて表示するタイムシート報告書。 レポートには、タイムシートの日付範囲、所有者の名前、合計時間数、時間外、承認者の名前、ステータスの各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイ未割り当てイシュー</td> 
   <td>ログイン ユーザーの担当業務のいずれかに割り当てられているが、このユーザーには割り当てられていないオープンな問題を表示する問題報告書。 レポートには、イシューのソース名、イシュータイプ、エントリ日、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイ未割り当てタスク</td> 
   <td>ログイン ユーザーの担当業務のいずれかに割り当てられているが、このユーザーには割り当てられていない未完了タスクを表示するタスク報告書。 レポートには、タスクの予定期間、プロジェクト名、プライマリ担当者、予定開始日、予定完了日、完了率および優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>マイ予定タスク</td> 
   <td>今後 2 週間以内に開始する見込みで、現在のプロジェクトに含まれており、ログイン ユーザーに割り当てられている、未完了タスクを表示するタスク報告書。 このレポートには、タスクのプロジェクト名、予定完了日、見込み完了日、完了率およびステータスの各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>オープンタイムシート（確認）</td> 
   <td>オープン タイムシートを表示するタイムシート報告書。 レポートには、タイムシートの日付範囲、所有者、合計時間数、残業、承認者名およびステータスの各フィールドが表示されます。レポートは、タイムシート開始日、タイムシート終了日、タイムシート承認者名およびユーザー名によって要求されます。</td> 
  </tr> 
  <tr> 
   <td>予算超過プロジェクト（ポートフォリオ別）</td> 
   <td>プロジェクトの予定コストと実際のコストを表示するプロジェクト報告書。 レポートはポートフォリオ名でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ予定コスト（プログラム別）</td> 
   <td>プロジェクトの予定コストと実際のコストを表示するプロジェクト報告書。 レポートには、ポートフォリオ名、プログラム名でグループ化されたグラフが表示されます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ計画コスト（プロジェクト別）</td> 
   <td>プロジェクトの予定コストと実際のコストを表示するプロジェクト報告書。 レポートには、ポートフォリオ名、プロジェクト名でグループ化されたグラフが表示されます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ予定収益（プログラム別）</td> 
   <td>プロジェクトの予定収益と実収益を表示するプロジェクト報告書。 レポートには、ポートフォリオ名、プログラム名でグループ化されたグラフが表示されます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ予定収益（プロジェクト別）</td> 
   <td>プロジェクトの予定収益と実収益を表示するプロジェクト報告書。 レポートには、ポートフォリオ名、プロジェクト名でグループ化されたグラフが表示されます。</td> 
  </tr> 
  <tr> 
   <td>予定コスト対実コスト（ポートフォリオ別）</td> 
   <td>プロジェクトの予定コストと実際のコストをPortfolio別に表示するプロジェクト報告書。 レポートはポートフォリオ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>予定コスト対実コスト（プログラム別）</td> 
   <td>プロジェクトの予定コストと実際のコストをプログラム別に表示するプロジェクト報告書。 レポートはポートフォリオ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>予定収益対実収益（ポートフォリオ別）</td> 
   <td>プロジェクトの予定収益と実収益を表示するプロジェクト報告書。 レポートはポートフォリオ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>予定収益対実収益（プログラム別）</td> 
   <td>プロジェクトの予定収益と実収益を表示するプロジェクト報告書。 レポートはプログラム名でグループ化され、グラフも含まれます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオコスト（プログラム別月別）</td> 
   <td>プロジェクトの予定コスト、予算計上コスト、および実際のコストを表示するマトリックス プロジェクト報告書。 このレポートは、ポートフォリオ名、プログラム名およびプロジェクトの予定開始日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト（プログラム別およびステータス別にグループ化）</td> 
   <td>プロジェクトの状態を表示するプロジェクト報告書。 レポートは、プログラム名とプロジェクトステータスでグループ化され、グラフも含まれます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオプロジェクト（ステータスおよびポートフォリオ別にグループ化）</td> 
   <td>プロジェクトのPortfolio名と状態を表示するプロジェクト報告書。 レポートは、プロジェクトのポートフォリオ名とステータスでグループ化され、グラフも含まれます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ収益（プログラム別）</td> 
   <td>プロジェクトのPortfolio名、プログラム名、予定収益、および実収益を表示するプロジェクト報告書。 レポートは、ポートフォリオ名とプログラム名でグループ化され、グラフも含まれます。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ売上高（プログラム別および月別にグループ化）</td> 
   <td>予定収益、実収益、Portfolio名、およびプログラム名を表示するマトリックス プロジェクト報告書。 このレポートは、ポートフォリオ名、プログラム名およびプロジェクトの予定開始日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトコストと売上高（タスクステータス別）</td> 
   <td>タスクの予定コスト、実際のコスト、予定収益、実収益、およびプロジェクト名を表示するマトリックス タスク報告書。 レポートは、タスクのプロジェクト名とステータスでグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトコストと売上高の比較（ポートフォリオ別）</td> 
   <td>プロジェクトのPortfolio名、実際のコスト、および実収益を表示するプロジェクト報告書。 レポートはポートフォリオ名でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト費用８月および四半期別）</td> 
   <td>費用のエントリ日、予定金額、実際の金額、およびプロジェクトを表示するマトリックス費用報告書。 レポートは、プロジェクト名、四半期、費用のエントリ日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトの時間コスト（時間タイプおよび月別）</td> 
   <td>次のフィールドを表示するマトリックス時間報告書：時間、エントリ日、プロジェクトの実際のコスト、時間タイプ、プロジェクト名。 レポートは、プロジェクト名、時間のエントリ日の月および時間タイプでグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト労力コストと費用コスト（月および四半期別)</td> 
   <td>プロジェクトの予定労力コスト、実際の労力コスト、予定費用コスト、および実際の費用コストを表示するマトリックス プロジェクト報告書。 このレポートは、プロジェクト名、プロジェクトの四半期、実際の開始日の月でグループ化されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトパフォーマンス</td> 
   <td>現在のプロジェクトの次のフィールドを表示するプロジェクト報告書。プロジェクトの期日、CPI、SPI、CSI、予定コスト、予算、EAC、および費用。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトリクエスト</td> 
   <td>要求されたプロジェクトを表示するプロジェクト報告書。 レポートには、プロジェクトの説明、予定完了日、完了見込日、完了率、ステータスおよび優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト（状況別）</td> 
   <td>プロジェクトの状態を表示するプロジェクト報告書。 レポートは状況別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト（状況およびグループ別）</td> 
   <td>プロジェクトの進捗状態とグループを表示するプロジェクト報告書。 レポートは、グループ名と進捗ステータス別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト（優先度別）</td> 
   <td>プロジェクトの優先度を表示するプロジェクト報告書。 レポートは、優先度でグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト（進捗ステータス別）</td> 
   <td>プロジェクトの進捗状態を表示するプロジェクト報告書。 レポートは、進捗ステータス別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>タスク（進捗ステータス別）</td> 
   <td>現在のプロジェクトに含まれる全タスクの進捗状態を表示するタスク報告書。 レポートは、進捗ステータス別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>タスク（ステータス別）</td> 
   <td>すべてのタスクの状態を表示するタスク報告書。 レポートは、ステータス別にグループ化され、グラフが含まれます。</td> 
  </tr> 
  <tr> 
   <td>確認用タイムシート</td> 
   <td>ログイン ユーザーが承認者である、送信済みタイムシートおよび拒否されたタイムシートを表示するタイムシート報告書。 レポートには、タイムシートの日付範囲、所有者、合計時間数、残業、承認者名およびステータスの各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>問題タスク</td> 
   <td>進捗状態が「遅延」または「遅れ」の未完了タスク、ハンドオフ日が明日より前で、ログイン ユーザーがタスクが含まれているプロジェクトのプロジェクト チームの一員であるものを表示するタスク報告書。 レポートには、タスクの予定期間、プロジェクト名、プライマリ担当者、予定開始日、予定完了日、完了率および優先度の各フィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td>ユーザーログイン</td> 
   <td>ユーザーの一意の ID、ログイン回数（Workfrontで始まって以降にログインした回数）、最終ログイン日のフィールドを表示するユーザーレポート。 レポートは、ユーザーのアクセスレベル別にグループ化されます。</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## ビルトインレポートにアクセス

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. 「**レポート**」をクリックします。
1. 「**すべてのレポート**」をクリックします。
1. **フィルター** ドロップダウンメニューを展開し、「**新しいフィルター**」を選択します。

1. 「**フィルタールールを追加**」をクリックします。
1. 「**フィールド名の入力を開始**」フィールドで「**グローバル ID**」の入力を開始します。

1. 「**レポート**」オブジェクトの下で、「**グローバル ID**」を選択します。

1. フィルター修飾子のドロップダウンメニューで、「**空白でない**」を選択します。\
   ![ システムレポートのグローバル ID フィルター ](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. 「**フィルターを保存**」をクリックします。\
   レポートリストには、ビルトインレポートのみが表示されます。\
   使用可能なビルトインレポートの詳細については、この記事の「[ ビルトインレポートの概要 ](#overview-of-built-in-reports) を参照してください。
