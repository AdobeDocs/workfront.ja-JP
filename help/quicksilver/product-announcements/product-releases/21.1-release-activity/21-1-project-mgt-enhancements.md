---
content-type: release-notes
keywords: メモ，四半期，更新
navigation-topic: product-releases
title: 21.1 プロジェクト管理の強化
description: このページでは、プレビュー環境の 21.1 リリースでおこなわれたプロジェクト管理のすべての機能強化について説明します。 これらの機能強化は、2021 年 2 月 15 日の週に実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 21.1 プロジェクト管理の強化

このページでは、プレビュー環境の 21.1 リリースでおこなわれたプロジェクト管理のすべての機能強化について説明します。 これらの機能強化は、2021 年 2 月 15 日の週に実稼動環境で利用可能になる予定です。

21.1 リリースで使用可能なすべての変更点の一覧については、 [21.1 リリースの概要](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## プロジェクトの指標セクションでエクスポートが利用できるようになりました

プロジェクトのステータスと進行状況をより簡単に共有できるように、プロジェクトの「指標」セクションにあるダッシュボード全体を.png ファイルにエクスポートできるようになりました。

詳しくは、 [プロジェクト指標の概要](../../../manage-work/projects/manage-projects/project-metrics.md).

この機能は、 [新しいWorkfrontエクスペリエンスのプランナーの基本、第 3 部：プロジェクトの管理](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) Workfront One の学習パス

## 問題の更新から変換されたプロジェクトまたはタスクで、問題の完了率を更新します

プロジェクトまたはタスクに変換された問題に対する、問題の完了率の仕組みを更新しました。 新機能では、問題がタスクまたはプロジェクトに変換されると、[ 解決可能な問題の状態が変更された場合に自動的に解決可能な問題の状態を更新する ] 設定が設定から有効になると、問題の完了率が解決タスクまたはプロジェクトの完了率と同期して更新されます。

問題の変換について詳しくは、 [オブジェクトの解決と解決の概要](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## 新しく送信されたリクエストリスト

より一貫性の高い簡単な方法で送信済みリクエストを管理できるように、「リクエスト」領域の「送信済みリクエスト」と「すべてのリクエスト」セクションを削除し、新しい送信済みリストに置き換えました。 リストは、システム内の他のすべてのリストと一致する使い慣れたルックアンドフィールを持ち、送信されたリクエストの様々なカテゴリをフィルタリングし、見つけにくいリクエストをすばやく検索できます。

送信されたリクエストの見つけ方について詳しくは、 [送信された要求を見つける](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

この機能は、 [新しいWorkfront Experience の共同作業者の基本](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One の学習パス

この機能は、 [新しいWorkfrontエクスペリエンスのリクエスト](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) Workfront One の学習パス

## 新しいリクエストページから削除されたフィールド

>[!NOTE]
>
>リリースから削除されました。

新しいリクエストページの再設計の一環として、プロジェクトのキュー設定セクションで設定された新しい問題フィールドを更新しました。

次の「新しい問題」フィールドは、プロジェクトの「問題」セクションから問題を作成する場合にのみ表示されます。 リクエスト領域のリクエストキューを使用して問題を送信する際に、次のような情報は表示されません。

* 重大度
* 予定時間数
* 予定開始日
* URL
* 割り当て先
* 担当業務
* チーム

新しいリクエストを送信する際に、共通のフィールドにユーザー、ジョブの役割、またはチームを効率的に指定するために、「割り当て先」、「ジョブの役割」、「チーム」の各フィールドは「新規リクエスト」ページで新しい「割り当て」フィールドに置き換えました。

プロジェクトでの新しい問題フィールドの定義について詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## リクエスト領域でリクエストを送信する際の新しいエクスペリエンス

>[!NOTE]
>
>リリースから削除されました。21.2 では、プレビューに残り、実稼動環境へのリリースになります。

新しいWorkfrontエクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエスト領域の新しいリクエストボックスのデザインを変更しました。 次に、改善点を示します。

* は、他の新しいWorkfrontエクスペリエンスと構成されたユーザーインターフェイスです
* 新しいリクエスト領域を排除し、より簡単で直感的なエクスペリエンスを実現
* リクエストにドキュメントを添付する新しい、より効率的な方法

リクエストを入力する際に、リクエストキュー、トピックグループまたはキュートピックへのリンクを共有できます。

リクエストの送信について詳しくは、 [Workfront要求の作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## リクエスト送信時のリクエストキューへのリンクの共有

>[!NOTE]
>
>リリースから削除されました。21.2 では、プレビューに残り、実稼動環境へのリリースになります。

リクエストの作成時に、リクエストキュー、トピックグループ、またはキュートピックへのリンクを共有できるようになりました。

新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループまたはキュートピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。

リクエスト送信時のリクエストキューへのリンクの共有について詳しくは、 [リクエストキューへのリンクの共有](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## プロジェクトに割り当てるグループを検索し、その詳細を表示します

プロジェクトにグループを割り当てる際に、適切なグループを識別しやすくなりました。 「グループ」ボックスに表示されるグループ名の上にマウスポインターを置き、名前の横に表示される情報アイコンをクリックして、グループの詳細のツールチップを表示します。

このツールチップには、グループの上のグループ（存在する場合）とグループの管理者の階層が含まれます。

グループに設定された詳細に応じて、グループのビジネスリーダーと説明も表示されます。

この情報を使用すると、プロジェクトに割り当てる適切なグループを選択できます。

詳しくは、 [プロジェクトの概要領域で情報を管理します。](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## 新しいユーザーの委任レポート

以前は、タスク、問題、プロジェクトの承認の委任に関する情報は、委任者のホーム領域にのみ表示されていました。 他のユーザーにこの情報の表示を許可するために、プランユーザーはユーザー委任レポートを作成できます。このレポートは、次の内容を示します。

* 他のユーザーにこれらの承認を委任したユーザー
* これらの承認が委任されたユーザー
* これらの委任の開始日と終了日

詳しくは、 [ユーザー委任レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
