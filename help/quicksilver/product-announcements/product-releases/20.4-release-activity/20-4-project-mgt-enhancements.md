---
title: 20.4 プロジェクト管理の機能強化
description: 20.4 プロジェクト管理の機能強化
author: Luke
draft: Probably
feature: Product Announcements
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1542'
ht-degree: 0%

---

# 20.4 プロジェクト管理の機能強化

このページでは、プレビュー環境の 20.4 リリースでおこなわれた、プロジェクト管理に関するすべての機能強化について説明します。 これらの機能強化は、2020 年 11 月 10 日の週に、実稼動環境で利用可能になる予定です。

20.4 リリースで使用可能なすべての変更点の一覧については、 [20.4 リリースの概要](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 管理者向けの新機能：カスタムフィールドの共有方法を制御する

作成したカスタムフィールドの編集、削除、使用をできるユーザーをより詳細に制御できるように、カスタムフィールドの共有方法を正確に設定する機能が追加されました。

これまで、カスタムフィールドを作成した場合、システムの全員が編集できました。 これは、カスタムフィールドのデフォルトの状態ですが、カスタムフィールドの共有を特定のユーザー、役割、チーム、グループおよび会社に制限できるようになりました。 また、受信者がカスタムフィールドの管理のみを行うか、カスタムフィールドのみを表示するかを指定できます。

また、この機能を身近に感じてもらうために、この機能のユーザーインターフェイスを、Workfront全体で共有される他のオブジェクト領域と同様のものにするように設計しました。

詳しくは、 [カスタムフィールドとウィジェットの共有を設定する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## 管理者向けの新機能：標準化されたカスタムフォーム共有

カスタムFormsの共有を標準化し、既に知っているのと同じWorkfrontオブジェクト共有プロセスを使用できるようにしました。 また、新しい共有エクスペリエンスにより、作成したカスタムFormsの編集、削除、使用を実行できるユーザーをより詳細に制御できます。 カスタムフォームの共有を、特定のユーザー、役割、チーム、グループおよび会社に制限できます。 また、これらの受信者がカスタムフォームを表示または管理できるかどうかを指定できます。

詳しくは、 [カスタムフォームの共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## プロジェクト、タスクまたは問題の詳細セクションからカスタムフォームおよび概要情報を書き出す

これで、カスタムフォーム情報を.pdf ファイルに書き出すことができます。 オブジェクトの「詳細」セクションでフォームにアクセスする際に、プロジェクト、タスクまたは問題からカスタムフォームを書き出すことができます。

プロジェクト、タスクおよび問題のカスタムフォームの書き出しに加えて、書き出した PDF に「概要」領域を含めることができるようになりました。

オブジェクトからカスタムフォームを書き出す方法について詳しくは、 [カスタムフォームとオブジェクトの詳細のエクスポート](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## 反復をすばやく追加

>[!NOTE]
>
>この機能は、実稼動環境から一時的に削除されました。 このページは、この機能が使用可能になると更新されます。

繰り返しの作成を簡単にするために、「繰り返し」タブから繰り返しを追加できる新しいボタンが追加されました。 ここでは、反復を作成し、後でタスクとイシューを追加できます。

バックログタグでは、以前と同様にイテレーションを作成できます。

詳しくは、 [反復を作成](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## プロジェクトで使用できる新しい指標セクション

時間を節約し、プロジェクトの全体的な正常性をより深く理解するために、プロジェクトに「指標」セクションが追加され、以下に関する情報が含まれるようになりました。

* 完了、未完了、期限切れ、および今後の作業
* ステータスまたは優先度別にグループ化されたタスクと発行金額
* 各ユーザーに割り当てられた作業量

グラフを選択して、プロジェクトのタスクや問題の様々な側面を表示し、特定の要素をクリックしてタスク情報を表示できます。

この機能は、 [プランナーの基本、第 3 部学習パス](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) Workfront・ワンで

## 管理者向けの新機能：ビジネスリーダーをグループに割り当て

グループの整理と定義を改善するために、ユーザーをグループ（またはサブグループ）のビジネスリーダーとして割り当てる機能が追加されました。 ビジネスリーダーとは、グループのビジネス上の意思決定をおこなうWorkfrontユーザーです。

新しい「ビジネスリーダー」フィールドは、レポートのフィルター、ビューおよびグループで使用できます。 例えば、特定のビジネスリーダーでフィルタリングして、その役割に割り当てられているグループのみをリストできます。

詳しくは、 [ビジネスリーダーの概要](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

この機能は、 [管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront・ワンで

## 管理者向けの新機能：ポートフォリオ、プログラム、会社とグループの関連付け

Workfront管理者がポートフォリオ、プログラムまたは会社を作成または編集する際に、ポートフォリオをグループに割り当てることができます。 グループがこれらのオブジェクトに割り当てられている場合、グループに対する責任を容易に特定できます。

例えば、組織のすべてのポートフォリオをレポートにリストし、「グループ」列を見て、グループが作業しているポートフォリオを確認できます。

詳細については、この記事の「グループとオブジェクトの関連付けについて」を参照してください。 [グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

この機能は、 [管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront・ワンで

## 管理者向けの新機能：会社に割り当てられたグループの管理者は、会社を管理できます

グループ管理者がWorkfrontでグループに関連付けられている会社を簡単に管理できるようになりました。 会社を管理するためのアクセスは、関連付けがおこなわれると自動的に使用可能になります。 これは、グループ管理者が会社に対する管理者アクセス権を持っていない場合に特に重要です。

詳しくは、 [会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

会社への管理アクセスについて詳しくは、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

この機能は、 [管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront・ワンで

## 「作業対象」ボタンを「開始」ボタンに置き換えます

作業項目で実際に開始する日時の作業を取り込むために、ユーザーは作業項目の状態と実際の開始日を自動的に更新する開始ボタンに置き換えることができます。

更新日：9 月 24 日[ タスクの開始 ] または [ タスクの開始 ] をクリックした後に、選択を元に戻すオプションが表示され、[ 元に戻す ] をクリックして作業項目の作業を開始する準備ができていない可能性が示されます。 作業項目は「新規」ステータスに戻り、「コミット日」と「実際の開始日」が削除されます。 「元に戻す」オプションは非常に短時間表示され、ページから移動したりページを更新した後はクリアされます。

このオプションの設定について詳しくは、 [「作業対象」ボタンを「開始」ボタンに置き換えます](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

この機能は、 [作業者の基本学習パス](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) そして [管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront・ワンで

## キュートピックに複数のドラフトを許可

リクエストを操作する際の自由度を高めるために、1 つのキュートピックに対して保存できるドラフトの数に制限がなくなりました。 新しいリクエストを作成する場合、同じキュートピックのドラフトのリストから既存のドラフトを選択し、上書きして新しいリクエストとして送信するか、新しいリクエストをゼロから作成できます。

この機能強化がおこなわれるまで、Workfrontはリクエストキュー内の各キュートピックに対して 1 つのドラフトのみを保存していました。

リクエストの送信について詳しくは、 [Workfront要求の作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## チームにグループを割り当てる

グループに関連付けられたチームの管理やレポートを簡単に行えるように、編集するアクセス権を持つチームに任意のグループを割り当てることができるようになりました。

グループにチームを割り当てると、そのグループ管理者は、チームのメンバーにならずにチームを管理できます。 チームの詳細ページで、管理するグループに割り当てられたチームを確認できます。 また、レポートを実行して、特定のグループに関連するすべてのチームを一覧表示できます。

詳しくは、 [チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

この機能は、 [管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront・ワンで

## 新しいフィールドでは、トップレベルのグループとそのサブグループのデータをレポートできます

トップレベルのグループとそのサブグループに関連付けられたデータを識別できるように、新しい「上位の親 ID」フィールドを追加しました。このフィールドは、グループオブジェクトに関するレポートを作成する際に、フィルタ、表示、グループで使用できます。

このフィールドは、複数のサブグループを含むグループを管理するグループ管理者に特に役立ちます。

例えば、Field Marketing と Digital Marketing のサブグループを持つ Marketing というグループを管理しているとします。 次のフィルター規則を持つ「プロジェクト」領域フィルターを作成すると、3 つすべてのグループに属するプロジェクトを一覧表示できます。
<pre>グループ：上位親名/次と等しい/マーケティング</pre>また、新しい「上位の親名」フィールドが追加され、（フィルターやグループではなく）ビューの最上位グループに関連付けられたデータを識別できるようになりました。

リストとレポートでのフィールドの使用について詳しくは、 [Adobe Workfrontの用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## 要求の下書きを破棄する際にアクションをキャンセルする新しいオプション

保存した下書きを破棄する際に、下書きが削除されることを通知する確認メッセージで「キャンセル」をクリックできるようになりました。 この方法では、破棄についての考えを変えた場合に、下書きを失うことはありません。

この機能は、新しいWorkfrontエクスペリエンスでのみ使用できます。 詳しくは、 [Workfront要求の作成と送信](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

