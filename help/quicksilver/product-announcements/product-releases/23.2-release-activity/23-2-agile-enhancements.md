---
title: 23.2 アジャイルの強化
description: 23.2 アジャイルの強化
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 8a209bbe64b7b69b41cd9e4d2f603ff58491ba30
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 23.2 アジャイルの強化

このページでは、プレビュー環境の 23.2 リリースでおこなわれたすべてのアジャイルの機能強化について説明します。 これらの機能強化は、23.2 リリースで実稼動環境で利用できるようになります。

23.2 リリースサイクルのこの時点で使用可能なすべての変更点のリストについては、 [23.2 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

<!--

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Second two articles will not be available in Main until I publish my branch.

## Add tasks and issues to Boards workstreams from lists and reports

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

-->

## ボード上の接続されたカードのログ時間

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

タスクやイシューと同じ方法で、接続されたカードに時間を記録できるようになりました。 時刻を記録するには、タスクまたはイシューに対する適切な権限が必要です。

デフォルトでは、接続されたカードにタイムログフィールドが表示されません。 有効にする必要があります **時間** をクリックします。

詳しくは、 [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## カードでのフィールド表示のカスタマイズ

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。


カードを開いたときのフルビューと、ボード上の縮小されたカード表示の両方で、どのフィールドをカードに表示するかを設定できるようになりました。 無効にしたフィールドは、どちらのビューにも表示されません。 また、フルビューでフィールドを有効にして、縮小表示で非表示にすることもできます。

詳しくは、 [カードに表示するフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3415710/){target=_blank}

## ボード列に移動されたカードのデフォルトのステータスを定義する

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

列ポリシーでカスタムステータスとシステムステータスを選択することで、特定の列に移動したカードに適用するデフォルトのステータスを設定できるようになりました。 カードを列に移動すると、Workfrontは最初にカスタムステータス（フィードバック待ちなど）の適用を試みます。 そのカードでカスタムステータスが使用できない場合、Workfrontは代わりにシステムステータスを適用します（保留中など）。 また、接続されたタスクまたは問題のステータスが列ポリシーで設定されたカスタムまたはシステムのステータスに変更された場合、カードは自動的に列に移動されます。

以前は、複数のステータスがある場合、列に移動するすべてのカードのステータスを選択するよう求めるプロンプトが表示されていました。

詳しくは、 [列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3415711/){target=_blank}

## コレクションがAdobe Workfrontボードで利用可能に

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボードダッシュボードでコレクションを作成できるようになりました。 コレクションは、作業での共同作業用のボードのグループです。 コレクションに名前を付けたら、列名などの事前定義済みの設定を提供する一連のテンプレートを使用して、コレクションにボードを追加できます。 スタンドアロンボードをコレクションに移動することもできます。 ボードがコレクションに含まれると、別のコレクションに移動できますが、スタンドアロンボードにすることはできません。

コレクションへのメンバーの追加は、ボードへのメンバーの追加と同じように機能します。 個人またはチームは、コレクション内のボードにメンバーとして追加する前に、コレクションのメンバーである必要があります。

詳しくは、 [コレクションの管理](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3415609/){target=_blank}

## 接続されたカードの推定フィールドは、Workfrontオブジェクトの「ストーリーポイント」フィールドにマッピングされます

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

Workfrontボードの接続されたカードの「推定」フィールドが、関連するWorkfrontオブジェクトの「ストーリーポイント」フィールドにマッピングされるようになりました。

新しい [ ストーリーポイント ] フィールドは、編集可能で自由形式のフィールドで、タスクやタスクに関するリストやレポートのビューに追加できます。 予定時間やチームの割り当てには縛られません。

以前は、カード見積もりは手動入力で、タスクやイシューのフィールドにはマッピングされませんでした。

また、アドホックカードと接続カードの「推定」フィールドに文字制限がなくなりました。 以前は、最大文字数は 99 文字でした。

詳しくは、 [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## インテーク列でカードをプレビュー

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

これで、インテーク列で接続されたカードをクリックして、その内容を表示専用バージョンで表示できるようになりました。 カードが取り込みカラムからボード上の別のカラムに移動するまで、カードの内容を編集することはできません。
