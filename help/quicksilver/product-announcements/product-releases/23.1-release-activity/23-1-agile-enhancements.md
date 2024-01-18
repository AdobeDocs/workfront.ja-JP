---
title: 23.1 アジャイルの強化
description: 23.1 アジャイルの強化
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 23.1 アジャイルの強化

このページでは、プレビュー環境の 23.1 リリースでおこなわれたすべてのアジャイルの機能強化について説明します。 これらの機能強化は、2023 年 1 月 17 日の週に実稼動環境で利用可能になる予定です。

23.1 リリースで使用可能なすべての変更点の一覧については、 [23.1 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Workfront Boards のスクラム計画

Adobe Workfrontボードの新しいスクラム計画機能は、アジャイルなプロセスを管理する柔軟なオプションを提供します。 これらのツールを使用して、次の操作を実行できます。

* 繰り返しまたはスプリントでの作業の追跡
* Velocity を使用してチームのコミットメントをガイド
* バーンダウンと完了率を追跡する

Scrum の計画機能は、23.1 リリース以降、「高速フォロー」になります。

## カードの期限は、Workfrontオブジェクトの予定完了日にマッピングされます

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

Workfrontボードで、接続されたカードの期限が、関連するWorkfrontオブジェクトの予定完了日にマッピングされるようになりました。 カードの期限を更新すると、タスクまたはイシューの予定完了日が更新されます。 計画完了日を変更すると、カードの期限も変更されます。 以前は、カードの期限は手動で入力されたもので、タスクやイシューの日付にはマッピングされていませんでした。

日付マッピングは、サブタスクに同期される接続済みのチェックリスト項目にも適用されます。

接続されたカードとアドホックカードの両方で、期限に時間フィールドが含まれるようになりました。

詳しくは、 [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3411952/){target=_blank}

## ボードのチェックリスト項目とWorkfrontのサブタスクがリンクされました

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

接続されたカードをWorkfrontタスクのボードに追加すると、サブタスクはカードのチェックリスト項目として読み込まれます。 また、接続したカードでチェックリスト項目を作成すると、サブタスクがWorkfrontタスクに追加されます。 問題に関するチェックリスト項目は、どのWorkfrontオブジェクトにも接続されていません。

以前は、チェックリスト項目とサブタスクはリンクされていませんでした。 サブタスクをボードに含めたい場合は、別の接続カードとして読み込むか、手動でチェックリスト項目をカードに追加します。

詳しくは、 [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) および [カードのチェックリスト項目を管理](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3411951/){target=_blank}

## ボード列のカードカウンター

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

新しい設定では、ボード上のすべての列のカードカウンターをオンにできます。 ある列に WIP 制限を使用している場合、別のカードカウンターは追加されません。

詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## ボードダッシュボードでの検索と並べ替え

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボードダッシュボードをボード名や日付で並べ替え、リスト内の特定のボードを検索できるようになりました。

詳しくは、 [ボードダッシュボードの使用](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## カードにステータスが表示されます

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボード上のカードにステータスが割り当てられた場合、そのステータスがカードに表示されるので、カードを開いてステータスを確認する必要はありません。 この強化は、アドホックカードと接続カードの両方に適用されます。

詳しくは、 [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) および [ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![カードのステータス](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## ボードでリンク可能なカードが利用可能になりました

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

特定のカードへのリンクを別のボードユーザに送信できるようになりました。 ユーザーがリンクを開くには、そのユーザーがボードを表示するアクセス権を持っている必要があります。

ボードでカードを開くと、ブラウザーの URL は次のようになります。

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

完全な URL をコピーして他のユーザーに送信できます。 リンクにアクセスすると、開いたカードに直接アクセスします。

以前は、ボードではリンクが使用できましたが、特定のカードでは使用できませんでした。

カードについて詳しくは、 [ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) および [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## ボードの接続でフィルタリング

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボード上のフィルターのリストに、接続でフィルターするオプションが追加され、特定のプロジェクトに接続されているカードがすべて表示されます。 また、接続されていないカードでフィルタリングすることもできます。

詳しくは、 [ボード内でのフィルターと検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412381/){target=_blank}

## スケジュールに従ってボードからカードをアーカイブ

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

カードをスケジュールに従ってアーカイブしたり、ボードから「フォールオフ」したりするようにボードを設定できます。 特定の列にカードを設定して、特定の日数または週数でアーカイブするオプションが使用できます。 たとえば、フォールオフを定義して、完了 (Complete) 列のカードを 2 週間後にアーカイブすることができます。

ボードから落ちた後に再度カードを表示する場合は、アーカイブしたカードを表示するようにボードフィルターを設定できます。

詳しくは、 [カードのフォールオフを設定](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412323/){target=_blank}
