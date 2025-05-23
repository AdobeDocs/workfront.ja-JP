---
content-type: release-notes
keywords: メモ、四半期、更新
navigation-topic: product-releases
title: 21.1 プロジェクト管理の機能強化
description: このページでは、プレビュー環境の 21.1 リリースで行われたプロジェクト管理のすべての機能強化について説明します。これらの機能強化は、2021年2月15日（PT）の週に実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 99%

---

# 21.1 プロジェクト管理の機能強化

このページでは、プレビュー環境の 21.1 リリースで行われたプロジェクト管理のすべての機能強化について説明します。これらの機能強化は、2021年2月15日（PT）の週に実稼動環境で利用可能になる予定です。

21.1 リリースで使用可能なすべての変更点の一覧については、[21.1 リリースの概要](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)を参照してください。

## プロジェクトの「指標」セクションで書き出しが利用可能に

プロジェクトのステータスと進行状況をより簡単に共有できるように、プロジェクトの「指標」セクションにあるダッシュボード全体を .png ファイルに書き出しできるようになりました。

詳しくは、[プロジェクト指標の概要](../../../manage-work/projects/manage-projects/project-metrics.md)を参照してください。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスにおける計画担当者の基礎、パート 3：プロジェクトの管理](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/home)に含まれるようになりました。

## イシューの更新からプロジェクトまたはタスクに変換された際のイシューの完了率をアップデート

プロジェクトまたはタスクに変換されたイシューにおけるイシューの完了率の仕組みをアップデートしました。新しい機能では、イシューがタスクまたはプロジェクトに変換されると、「解決オブジェクトの状態が変わると、解決可能問題の状態を自動的に更新します」が設定で有効になっている場合、イシューの完了率が解決タスクまたは解決プロジェクトの完了率と同期して更新されます。

イシューの変換について詳しくは、[オブジェクトの解決と解決可能なオブジェクトの概要](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)を参照してください。

## 新しく送信されたリクエストのリスト

より簡単で一貫性の高い方法で送信済みリクエストを管理できるように、リクエストエリアの「送信済みの要求」セクションと「すべての要求」セクションを削除し、新しく「送信済み」リストに置き換えました。リストは、システムの他のリストとマッチする使い慣れたルックアンドフィールになっており、送信済みリクエストの様々なカテゴリをフィルタリングし、見つけにくいリクエストを素早く検索できます。

送信済みリクエストを見つける方法について詳しくは、[送信済みリクエストを見つける](../../../manage-work/requests/create-requests/locate-submitted-requests.md)を参照してください。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスにおける共同作業者の基礎](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)に含まれるようになりました。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスのリクエスト](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/understand-request-queues)に含まれるようになりました。

## 新しいリクエストページから削除されたフィールド

>[!NOTE]
>
>リリースから削除されました。

新しいリクエストページの再設計の一環として、プロジェクトの「キューの設定」セクションで設定された新しいイシューフィールドを更新しました。

次の新しいイシューフィールドは、プロジェクトの「イシュー」セクションからイシューを作成する場合にのみ表示されます。リクエストエリアのリクエストキューを使用してイシューを送信する際に、次のような情報は表示されません。

* 重大度
* 予定時間数
* 予定開始日
* URL
* 割り当て先
* 担当業務
* チーム

新しいリクエストを送信する際に、共通のフィールドにユーザー、担当業務、チームを効率的に指定できるように、「割り当て先」「担当業務」「チーム」の各フィールドは新規リクエストページで新しい「割り当て」フィールドに置き換えられました。

プロジェクトでの新しいイシューフィールドの定義について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

## リクエストエリアでリクエストを送信する際の新しいエクスペリエンス

>[!NOTE]
>
>リリースから削除されました。21.2 では、プレビューおよび実稼動版リリースに残されます。

新しい Workfront エクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエストエリアの「新規リクエスト」ボックスのデザインを変更しました。改善点のいくつかを次に示します。

* 新しい Workfront Experience の他の部分と一貫性のあるユーザーインターフェイス
* 新しい要求エリアを削除し、より簡単で直感的なエクスペリエンスを実現
* リクエストにドキュメントを添付するさらに効率的で新しい方法

リクエストを入力する際に、リクエストキュー、トピックのグループまたはキューのトピックへのリンクを共有できます。

リクエストの送信について詳しくは、[Workfront リクエストの作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

## リクエスト送信時のリクエストキューへのリンクの共有

>[!NOTE]
>
>リリースから削除されました。21.2 では、プレビューおよび実稼動版リリースに残されます。

リクエストの作成時に、リクエストキュー、トピックグループ、またはキューのトピックへのリンクを共有できるようになりました。

新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループ、またはキューのトピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。

リクエスト送信時のリクエストキューへのリンク共有について詳しくは、[リクエストキューへのリンクの共有](../../../manage-work/requests/create-requests/share-link-to-request-queue.md)を参照してください。

## プロジェクトに割り当てるグループを検索し、その詳細を表示する

プロジェクトにグループを割り当てる際に、適切なグループを識別しやすくなりました。「グループ」ボックスに表示されるグループ名の上にポインタを合わせて、名前の横に表示される情報アイコンをクリックして、グループの詳細のツールチップを表示します。

このツールチップには、グループの上のグループ（存在する場合）とグループの管理者の階層が含まれます。

グループに設定された詳細に応じて、グループのビジネスリーダーと説明も表示されます。

この情報を使用すると、プロジェクトに割り当てる適切なグループを選択できます。

詳しくは、[プロジェクトの概要エリアで情報を管理する](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)を参照してください。

## 新しくなったユーザーのデリゲーションレポート

以前は、タスク、イシュー、プロジェクトの承認のデリゲーションに関する情報は、デリゲートのホームエリアにのみ表示されていました。他のユーザーにこの情報の表示を許可するために、プランユーザーはユーザーのデリゲーションレポートを作成できます。このレポートは、次の内容を示します。

* 他のユーザーにこれらの承認をデリゲートしたユーザー
* これらの承認がデリゲートされたユーザー
* これらのデリゲーションの開始日と終了日

詳しくは、[ユーザーのデリゲーションレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md)を参照してください。
