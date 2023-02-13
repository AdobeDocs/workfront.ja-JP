---
title: 22.4 アジャイルの強化
description: 22.4 アジャイルの強化
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5d954537-5ee4-43b5-b1ab-d62433496e35
source-git-commit: 87d0b668185c4185646bfa1622eb37337844bcbc
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 22.4 アジャイルの強化

このページでは、プレビュー環境の 22.4 リリースでおこなわれたすべてのアジャイルの機能強化について説明します。 これらの機能強化は、2022 年 10 月 3 日の週に提供されます。

22.4 リリースで使用可能なすべての変更点の一覧については、 [22.4 リリースの概要](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 取り込みカラムはボードで利用可能

注意：この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

これで、ボードに取り込みカラムを追加できます。 この列は、定義したフィルターに基づいて、Workfrontに追加されたタスクとイシューを自動的にボードに取り込みます。

取り入れ列は、かんばんチームのバックログ列、サポートチームの取り入れ場所として、要求キューに追加された問題を確認するための取り入れ場所、または必要なその他の目的に使用できます。

1 つのボード上で許可される吸気カラムは 1 つだけです。

詳しくは、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412867/){target=_blank}

## ボードのフィルターパネルを更新しました

注意：この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボード上のフィルターアイコンと検索アイコンが、画面の左側に移動しました。 フィルターアイコンをクリックすると、左側のパネルが開き、すべてのフィルターオプションが表示されます。 以前は、フィルターは、ボードの右側のドロップダウンに表示されていました。

詳しくは、 [ボードでのフィルターと検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412868/){target=_blank}

## ボード上でグループを使用してスイムレーンを作成する

担当者別またはタグ別に、ボード上のカードをグループ化できるようになりました。 グループ化するオプションを選択すると、カードはスイムレーン形式で表示されます。 未割り当てのカードやタグのないカードは、独自のスイムレーンに表示されます。

また、カードをグループ間で移動した場合の動作を定義することもできます。 カードを移動するグループ内の担当者またはタグは、既存の担当者またはタグに追加したり、カード上の他の担当者またはタグを上書きしたりできます。

取り込みカラム内のカードはグループに含まれません。

詳しくは、 [ボードでのグループの使用](/help/quicksilver/agile/use-boards-agile-planning-tools/group-cards-on-board.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412869/){target=_blank}

## ボードのチェックリスト項目の強化

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ使用できます。

カードでチェックリスト項目を開くと、説明、期限、担当者、推定など、項目に関する詳細情報を追加できるようになりました。 以前は使用できなかったチェックリスト項目をコピーすることもできます。

詳しくは、 [カードのチェックリスト項目を管理](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

## ボードまたはカードにチームを追加する

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ使用できます。

これで、チームをボードのメンバーとして追加できます。 すべてのチームメンバーがボードにアクセスできますが、個々のチームメンバーは、ボードにチームを追加する際に追加されなくなります。

チームをボードに追加した後、チームをカードに割り当てることができます。 接続されたカードでは、1 つのチーム割り当てのみが許可されます。 アドホックカードでは、複数のチームを割り当てることができます。

詳しくは、 [ボードに対するメンバーの追加または削除](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412870/){target=_blank}

## ボード列で作業中の制限が使用できるようになりました

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボード上の任意の列に対して WIP(Work In Progress) 制限を設定できるようになりました。 WIP 制限を有効にすると、カード数と制限を含むカウンターが列に表示されます。 列に制限を超えるカードが含まれている場合、カウンターが赤に変わります。 これは単に視覚的な警告であり、制限を超えるカードの追加を停止することはありません。

詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412871/){target=_blank}

## カードに追加された推定フィールド

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ使用できます。

アドホックカードと接続カードの両方にある新しい「推定」フィールドを使用すると、カードが完了する推定時間数を入力できます。 これは、計算値ではなく手動の入力です。値は 99 以下にする必要があります。 見積もりは、ボード上のカードとカードの詳細に表示されます。

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412872/){target=_blank}