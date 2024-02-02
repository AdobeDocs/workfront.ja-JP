---
title: 20.4 プロジェクト管理の機能強化
description: 20.4 プロジェクト管理の機能強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '1485'
ht-degree: 100%

---

# 20.4 プロジェクト管理の機能強化

このページでは、プレビュー環境の 20.4 リリースで行われた、プロジェクト管理に関するすべての機能強化について説明します。これらの機能強化は、2020年11月9日（PT）の週に実稼動環境で利用可能になる予定です。

20.4 リリースで利用可能なすべての変更点の一覧については、[20.4 リリースの概要](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md)を参照してください。

## 管理者向けの新機能：カスタムフィールドの共有方法を制御

作成したカスタムフィールドの編集、削除および使用が可能なユーザーをよりきめ細かく制御できるように、カスタムフィールドの共有方法を正確に設定する機能が追加されました。

これまでは、カスタムフィールドを作成した場合、システムのすべてのユーザーがそれを編集できました。カスタムフィールドは、デフォルトの状態ではやはりそうなっていますが、カスタムフィールドの共有を特定のユーザー、役割、チーム、グループおよび会社に限定できるようになりました。また、カスタムフィールドを受信者が管理できるようにするか、表示のみ可能にするかを指定できます。

また、これをなじみのあるエクスペリエンスにするために、この機能のユーザーインターフェイスを、Workfront 全体で共有される他のオブジェクト領域と同様のものになるように設計しました。

詳しくは、[カスタムフィールドとウィジェットの共有を設定](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md)を参照してください。

## 管理者向けの新機能：標準化されたカスタムフォームを共有

カスタムフォームの共有を標準化したので、既にご存知のものと同じ Workfront オブジェクト共有プロセスを使用できます。また、新しい共有エクスペリエンスでは、作成したカスタムフォームの編集、削除および使用が可能なユーザーをよりきめ細かく制御できます。カスタムフォームの共有を、特定のユーザー、役割、チーム、グループおよび会社に限定できます。また、これらの受信者がカスタムフォームの表示のみ可能か管理も可能かを指定できます。

詳しくは、[カスタムフォームを共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)を参照してください。

## プロジェクト、タスクまたはイシューの詳細セクションからのカスタムフォームおよび概要情報を書き出し

これで、カスタムフォーム情報を .pdf ファイルに書き出すことができます。オブジェクトの「詳細」セクションでフォームにアクセスする際に、プロジェクト、タスクまたはイシューからカスタムフォームを書き出すことができます。

プロジェクト、タスクおよびイシューのカスタムフォームの書き出しに加えて、書き出した PDF に「概要」エリアを含められるようになりました。

オブジェクトからカスタムフォームを書き出す方法について詳しくは、[カスタムフォームとオブジェクトの詳細を書き出し](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)を参照してください。

## 迅速なイテレーションを追加

>[!NOTE]
>
>この機能は、実稼動環境から一時的に削除されました。このページは、この機能が使用可能になると更新されます。

イテレーションの作成を容易にするために、「イテレーション」タブからイテレーションを追加できる新しいボタンが追加されました。ここでは、イテレーションを作成し、後でタスクとイシューを追加できます。

バックログタグでは、以前と同様にイテレーションを作成できます。

詳しくは、[イテレーションを作成](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)を参照してください。

## プロジェクトで使用できる新しい指標セクション

時間を節約し、プロジェクトの全体的な正常性をより深く理解するために、次のような情報を含む「指標」セクションをプロジェクトで使用できるようになりました。

* 完了、未完了、期限切れ、および今後の作業
* ステータスまたは優先度ごとにグループ化されたタスクとイシューの量
* 各ユーザーに割り当てられた作業量

グラフを選択して、プロジェクトのタスクやイシューの様々な側面を表示し、特定の要素をクリックしてタスクの情報を表示できます。

この機能は、Workfront One の[プランナーの基本、第 3 部学習パス](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA)を含みます。

## 管理者向けの新規：ビジネスリーダーをグループに割り当て

グループの整理と定義を改善するために、ユーザーをグループ（またはサブグループ）のビジネスリーダーとして割り当てる機能が追加されました。ビジネスリーダーとは、グループのビジネス上の意思決定を行う Workfront ユーザーです。

新しいビジネスリーダーフィールドは、レポートのフィルター、表示およびグループ化で使用できます。例えば、特定のビジネスリーダーでフィルタリングして、その人物がその役割に割り当てられているグループのみをリストすることができます。

詳しくは、[ビジネスリーダーの概要](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md)を参照してください。

この機能は現在、Workfront One の[管理者の基本、第 1 部　学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)に含まれています。

## 管理者向けの新機能：ポートフォリオ、プログラム、会社とグループの関連付け

Workfront 管理者がポートフォリオ、プログラムまたは会社を作成または編集する際に、ポートフォリオをグループに割り当てることができます。グループがこれらのオブジェクトに割り当てられている場合、彼らに対するグループの責任を容易に特定できます。

例えば、組織のすべてのポートフォリオをレポートにリストし、グループ列を見て、グループが作業しているポートフォリオを確認することができます。

詳しくは、[グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md)の記事の「グループとオブジェクトの関連付けについて」を参照してください。

この機能は現在、Workfront One の[管理者の基本、第 1 部　学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)に含まれています。

## 管理者向けの新機能：会社に割り当てられたグループの管理者は、会社を管理できます

グループ管理者が Workfront でグループに関連付けられている会社を、簡単に管理できるようになりました。会社を管理するためのアクセスは、関連付けられると自動的に使用可能になります。これは、グループ管理者に会社への管理者アクセスがない場合に特に重要です。

詳しくは、[会社を作成および編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。

会社への管理アクセスに関する詳細情報は、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

この機能は現在、Workfront One の[管理者の基本、第 1 部 学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)に含まれています。

## 「作業をする」ボタンを「開始」ボタンに置き換えます

作業アイテムで実際に作業が始まる日時を取り込むために、ユーザーは「作業をする」ボタンを「開始」ボタンに置き換えて、作業アイテムの状態と実際の開始日を自動的に更新することができます。

9月24日（PT）更新：タスク開始またはイシュー開始をクリックした後、選択を元に戻すオプションが追加され、「元に戻す」をクリックすると、作業アイテムの作業を開始する準備ができていないことを示すことができるようになりました。作業アイテムは「新規」ステータスに戻り、「コミット日」と「実際の開始日」が削除されます。「元に戻す」オプションは非常に短時間表示され、ページから移動するかページを更新した後はクリアされます。

このオプションの設定に関して詳しくは、[「作業をする」ボタンを「開始」ボタンに置き換え](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)を参照してください。

この機能は現在、[作業者の基本の学習パス](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA)および Workfront One の[管理者の基本、第 1 部　学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)に含まれています。

## キュートのピックに複数のドラフトを許可する

リクエストを操作する際の自由度を高めるために、1 つのキューのトピックに対して保存できる下書き数の制限をなくしました。新しいリクエストを作成する場合、同じキューのトピックに対する下書きの一覧から既存の下書きを選択し、上書きして新しいリクエストとして送信するか、新しいリクエストをゼロから作成できます。

この機能強化が行われるまで、Workfront でリクエストキュー内の各キューのトピックに対して保存できる下書きは 1 つのみでした。

リクエストの送信に関する詳細情報は、[Workfront リクエストの作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

## チームにグループを割り当てる

グループに関連付けられたチームの管理やレポートを簡単に行えるように、編集するアクセス権を持つチームに、任意のグループを割り当てることができるようになりました。

グループにチームを割り当てると、そのグループ管理者は、チームのメンバーにならずにチームを管理することができます。チームの詳細ページで、管理するグループに割り当てられたチームを確認できます。またレポートを実行して、特定のグループに関連付けられているすべてのチームをリストすることもできます。

詳しくは、[チームを作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)を参照してください。

この機能は現在、Workfront One の[管理者の基本、第 1 部　学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)に含まれています。

## 新しいフィールドで、トップレベルのグループとそのすべてのサブグループのデータをレポートできます

トップレベルのグループとそのサブグループに関連付けられたデータを識別できるように、「最上位の親 ID」フィールドを新しく追加しました。このフィールドは、グループオブジェクトに関するレポートを作成する際に、フィルター、ビュー、グループで使用できます。

このフィールドは、複数のサブグループを含むグループを管理するグループ管理者に特に役立ちます。

例えば、フィールドマーケティングとデジタルマーケティングというサブグループを持つマーケティングというというグループを管理しているとします。以下のフィルタールールを持つプロジェクトエリアフィルターを作成すると、3 つすべてのグループに属するプロジェクトを一覧表示できます。
<pre>グループ：最上位の親名／次と等しい／マーケティング</pre>また、新しい最上位の親名フィールドが追加され、（フィルターやグループ内でではなく）表示の最上位グループに関連付けられたデータを識別できるようになりました。

リストとレポートでのフィールドの使用に関する詳細情報は、[Adobe Workfront の用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

## リクエストの下書きを破棄する際にアクションをキャンセルできる新しいオプション

保存済みの下書きを破棄する際に、下書きが削除されることを通知する確認メッセージで「キャンセル」をクリックできるようになりました。これにより、破棄を止めた場合でも、下書きが失われることはありません。

この機能は、新しい Workfront エクスペリエンスでのみ使用できます。詳しくは、[Workfront リクエストの作成および送信](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html?lang=ja)を参照してください。

