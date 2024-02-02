---
title: 23.1 アジャイルの機能強化
description: 23.1 アジャイルの機能強化
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '889'
ht-degree: 100%

---

# 23.1 アジャイルの機能強化

このページでは、23.1 リリースでプレビュー環境に対して行われたすべてのアジャイル機能強化について説明します。これらの機能強化は、2023年1月16日の週に実稼動環境で利用可能になる予定です。

23.1 リリースで使用可能なすべての変更点の一覧について詳しく、[23.1 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md)を参照してください。

## Workfront Boards のスクラム計画

Adobe Workfront ボードの新しいスクラム計画機能は、アジャイルなプロセスを管理する柔軟なオプションを提供します。これらのツールを使用して、次の操作を実行できます。

* イテレーションまたはスプリントでの作業をトラック
* 速度を利用してチームのコミットメントを導く
* バーンダウンと完了率を追跡

スクラム計画機能は、23.1 リリース以降、「迅速フォロー」になります。

## カードの期限は、Workfront オブジェクトの予定完了日にマッピング

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

Workfront ボードの接続されたカードの期限が、関連する Workfront オブジェクトの予定完了日にマッピングされるようになりました。カードの期限を更新すると、タスクまたはイシューの予定完了日が更新されます。予定完了日を変更すると、カードの期限も変更されます。以前は、カードの期限は手動で入力されたもので、タスクやイシューの日付にはマッピングされていませんでした。

日付マッピングは、サブタスクに同期される接続済みのチェックリスト項目にも適用されます。

接続されたカードとアドホックカードの両方で、期限に時間フィールドが含まれるようになりました。

詳しくは、[ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)を参照してください。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3411952/){target=_blank}

## ボードのチェックリスト項目と Workfront のサブタスクがリンクされました

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

接続されたカードを Workfront タスクのボードに追加すると、サブタスクはカードのチェックリスト項目として読み込まれます。また、接続したカードでチェックリスト項目を作成すると、サブタスクが Workfront タスクに追加されます。イシューに関するチェックリスト項目は、どの Workfront オブジェクトにも未接続です。

以前は、チェックリスト項目とサブタスクはリンクされていませんでした。サブタスクをボードに含めたい場合は、別の接続カードとして読み込むか、手動でチェックリスト項目をカードに追加します。

詳しくは、[ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)および[カードのチェックリスト項目を管理](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md)を参照してください。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3411951/){target=_blank}

## ボード列のカードカウンター

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

新しい設定では、ボード上のすべての列のカードカウンターをオンにできます。ある列に WIP 制限を使用している場合、別のカードカウンターは追加されません。

詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。

## ボードダッシュボードでの検索と並べ替え

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

ボードダッシュボードをボード名や日付で並べ替え、リスト内の特定のボードを検索できるようになりました。

詳しくは、[ボードダッシュボードの使用](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)を参照してください。

## カードに表示されたステータス

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

ボード上のカードにステータスが割り当てられた場合、そのステータスがカードに表示されるので、カードを開いてステータスを確認する必要はありません。この機能強化は、アドホックカードと接続カードの両方に適用されます。

詳しくは、[ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)および[ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)を参照してください。

![カードのステータス](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## ボードでリンク可能なカードが利用可能になりました

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

特定のカードへのリンクを別のボードユーザーに送信できるようになりました。ユーザーがリンクを開くには、そのユーザーにボードを表示するアクセス権必要です。

ボードでカードを開くと、ブラウザーの URL は次のようになります。

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

完全な URL をコピーして他のユーザーに送信できます。リンクにアクセスすると、開いたカードに直接移動します。

以前は、ボードではリンクが使用できましたが、特定のカードでは使用できませんでした。

カードについて詳しくは、[ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)および[ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)を参照してください。

## ボードの接続でフィルター

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

ボード上のフィルターのリストに、接続によってフィルタリングするオプションが追加され、特定のプロジェクトに接続されているカードがすべて表示されます。また、未接続のカードでフィルタリングすることもできます。

詳しくは、[ボード内でのフィルターと検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)を参照してください。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3412381/){target=_blank}

## スケジュールに従ってボードからカードをアーカイブ

>[!NOTE]
>
>この機能は、Workfront ボードの初期の機能オプトインでのみ利用できます。

カードをスケジュールに従ってアーカイブしたり、ボードから「フォールオフ」したりするようにボードを設定できます。特定の列にカードを設定して、特定の日数または週数でアーカイブするオプションが使用できます。例えば、フォールオフを定義して、完了列のカードを 2 週間後にアーカイブすることができます。

ボードから消えた後に再度カードを表示する場合は、アーカイブしたカードを表示するようにボードフィルターを設定できます。

詳しくは、[カードのフォールオフを設定](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md)を参照してください。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3412323/){target=_blank}
