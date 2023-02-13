---
content-type: release-notes
keywords: メモ，四半期，更新，リリース
navigation-topic: 2021-2-release-activity
title: 21.2 要求の機能強化
description: このページでは、プレビュー環境の 21.2 リリースでおこなわれたすべての要求の機能強化について説明します。 これらの機能強化は、2021 年 5 月 10 日の週に実稼動環境で利用可能になる予定です。 21.2 リリースで使用できるすべての変更点の一覧については、 21.2 リリースの概要を参照してください。
author: Luke
feature: Product Announcements
exl-id: af9c801f-ae40-439a-8749-ae8d178040ae
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# 21.2 要求の機能強化

このページでは、プレビュー環境の 21.2 リリースでおこなわれたすべての要求の機能強化について説明します。 これらの機能強化は、2021 年 5 月 10 日の週に実稼動環境で利用可能になる予定です。 21.2 リリースで使用可能なすべての変更点の一覧については、 [21.2 リリースの概要](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 新しいリクエストに対して実行する割り当てのタイプを制御する

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

一貫性を保つために新しいリクエストを作成する際の「割り当て」フィールドの機能を変更し、ユーザーが入力できる割り当ての種類に関係なく、常に同じフィールドを表示するようにしました。

リクエストキューの設定時に、「割り当て先」、「ジョブロール」、または「チーム」の各フィールドを表示すると、リクエスターには、これら 3 つの割り当てタイプのすべてまたはいずれかに対応する同じ「割り当て」フィールドが表示されます。

[ 割り当て ] フィールドには、許可される割り当ての種類を示すメッセージが表示されます。 例えば、リクエストキューを設定する際に「割り当て先」フィールドと「チーム」フィールドを有効にすると、「担当者、役割またはチームを検索」ではなく「担当者またはチームを検索」するよう求められます。

詳しくは、次の記事を参照してください。

* [Adobe Workfront要求の作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## リクエストの作成とドラフトの管理の改善

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

新しいWorkfrontエクスペリエンスにリクエストの作成に関するフィードバックを取り入れ続ける中で、新しいリクエストワークフローに対していくつかの改善を行いました。 これには次が含まれます。

* 「オプションを表示」アイコンを使用して、「要求タイプ」、「トピックグループ」、「キュートピック」の各フィールドが、以前に定義したオプションを選択できるドロップダウンリストであることを明確に示します。
* 「X」アイコンを使用して、リクエストの種類、トピックグループ、またはキュートピックの選択肢が選択された後に削除できることを明確に示します。
* 新しいリクエストを作成する際に、下書きを失うことなくリクエストを終了するための「閉じる」ボタンを指定します。 この変更に加え、「破棄」ボタンの名前が「下書きの破棄」に変更されました。

新しいリクエストの作成について詳しくは、 [Adobe Workfront要求の作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

この機能は、 [新しいWorkfront Experience の共同作業者の基本](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One の学習パス

## リクエストワークフローの改善

>[!NOTE]
>
>この機能は、新しいAdobe Workfrontエクスペリエンスでのみ使用できます

アドビでは、お客様のフィードバックを引き続き聞き、取り込む際に、新しいリクエストワークフローにいくつかの改善を加え、Adobe Workfrontとのインタラクションをより簡単かつ直感的にできるようにしました。 次の機能強化がおこなわれました。

* キュー設定の定義時に、要求キューを作成する際に、ファイルのアップロード用の「ドキュメント」セクションを配置する場所を選択できます。 このセクションは、リクエストフォームのカスタムフィールドの前または後に配置できます。 詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 「送信済みのリクエスト」リストをいずれかの列で並べ替えても、ページから移動しても保持されるようになりました。 詳しくは、 [送信された要求の場所](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
* 新しいリクエストを作成する際に、「送信」ボタンと「キャンセル」ボタンが新しいリクエストフォームの下部に表示されるようになりました。 詳しくは、 [Workfront要求の作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

この機能は、 [新しいWorkfront Experience の共同作業者の基本](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One の学習パス

## リクエスト領域の「Submitted」セクションで Summary パネルを開きます。

>[!NOTE]
>
>この機能は、新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

Adobe Workfrontのすべての領域でエクスペリエンスの一貫性を保つために、リクエスト領域の「送信済み」セクションに概要を開くアイコンを追加しました。 送信された問題の概要パネルを開き、問題に関する詳細を表示したり、問題を割り当てたり、ドキュメントやコメントを追加したりできます。

送信されたリクエストについて詳しくは、 [送信された要求の場所](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

この機能は、 [新しいWorkfront Experience の共同作業者の基本](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One の学習パス

## 削除した新しい問題フィールドを新しいリクエストフォームに戻す

>[!NOTE]
>
>この機能は、新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

以前のリリースで開始した新しいリクエストフォームのデザインを変更した際に、新しいリクエストを送信する際に、プロジェクトの「Queue Details」セクションの「New Issue Fields」領域に表示される複数のフィールドを非表示にしました。 フィードバックを取り込んだ後、フィールドを取り戻し、すべてのフィールドを新しいリクエストフォームに表示できるようにすることにしました。

詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## リクエスト領域でリクエストを送信する際の新しいエクスペリエンス

>[!NOTE]
>
>21.1 リリースで Preview に追加されましたが、21.2 の実稼動環境へのリリースに含まれる予定です。

新しいWorkfrontエクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエスト領域の新しいリクエストボックスのデザインを変更しました。 改善点を以下に示します。

* は、他の新しいWorkfrontエクスペリエンスと構成されたユーザーインターフェイスです
* 新しいリクエスト領域を排除し、より簡単で直感的なエクスペリエンスを実現
* リクエストにドキュメントを添付する新しい、より効率的な方法

リクエストを入力する際に、リクエストキュー、トピックグループまたはキュートピックへのリンクを共有できます。

リクエストの送信について詳しくは、 [Workfront要求の作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

この機能は、 [新しいWorkfront Experience の共同作業者の基本](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One の学習パス

## リクエスト送信時のリクエストキューへのリンクの共有

>[!NOTE]
>
>21.1 リリースで Preview に追加されましたが、21.2 の実稼動環境へのリリースに含まれる予定です。

リクエストの作成時に、リクエストキュー、トピックグループ、またはキュートピックへのリンクを共有できるようになりました。

新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループまたはキュートピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。

リクエスト送信時のリクエストキューへのリンクの共有について詳しくは、 [リクエストキューへのリンクの共有](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

この機能は、 [新しいWorkfront Experience の共同作業者の基本](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront One の学習パス
