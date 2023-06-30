---
title: 23.3 アジャイルの強化
description: 23.3 アジャイルの強化
author: Lisa
feature: Product Announcements
source-git-commit: 3aa19652024cd6df1c9560aad6e982e4b615569c
workflow-type: tm+mt
source-wordcount: '1305'
ht-degree: 0%

---

# 23.3 アジャイルの強化

このページでは、プレビュー環境の 23.3 リリースでおこなわれたすべてのアジャイル機能の強化について説明します。 これらの機能強化は、23.3 リリースで実稼動環境で利用できるようになります。

23.3 リリースサイクルのこの時点で使用可能なすべての変更点のリストについては、 [23.3 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

四半期リリース前の新しいボード機能をオプトインする方法について詳しくは、 [Adobe Workfrontボードの初期機能のオプトイン](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

## プロジェクトの「アジャイル・ビュー」には、かんばんボードが表示されます

プロジェクトの「アジャイルビュー」には、かんばんボード内の作業をフィルタリング、グループ化、並べ替える機能が追加されました。 新しい柔軟なビューデザインには、堅牢な検索機能と、ボードから直接プロジェクトに新しいタスクを追加する機能が含まれています。

>[!NOTE]
>
>「アジャイルビュー」は、プロジェクトの代替表示であり、ボードダッシュボードなどWorkfrontの他の領域からはアクセスできないので、単一のプロジェクトにのみ存在します。

ボードにいる間、レガシー Agile View に切り替えることができます。

詳しくは、 [アジャイルビューでのプロジェクト管理](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3421283/){target=_blank}

## ボード列で並べ替え

ボード上の列のカードを並べ替える機能が追加されました。 並べ替えの基準となるオプションを選択すると、すべての列が並べ替えられます。 1 つの列を並べ替えることはできません。また、backlog 列または intake 列は並べ替えられません。

カード名、期限、見積もり、ステータスまたは接続（プロジェクト名）で、昇順または降順に並べ替えることができます。 接続は、接続されたカードにのみ適用され、その他のオプションは、列内の接続されたカードとアドホックカードの両方を並べ替えます。

「ユーザーの順序」オプションは、他の並べ替えオプションが適用される前に、手動で設定された順序にカードを返します。 列のデフォルトの並べ替えです。

詳しくは、 [ボードでのフィルターと検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3420932/){target=_blank}

## Adobe Workfrontボードでダークモードが利用可能

これで、すべてのボードとワークストリームをダークモードで表示できます。 新しい設定は、ボードダッシュボードの環境設定で利用できます。

>[!NOTE]
>
>組織のWorkfrontインスタンスがAdobeUnified Experience にオンボーディングされている場合は、環境設定メニュー（プロフィールの画像）ですべてのAdobe Experience Cloudのダークテーマの書式設定を有効にできます。Workfrontボードにはダークモードオプションは別に表示されません。

詳しくは、 [電子メール通知と環境設定をボード](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

## Adobe Workfrontボードのワークストリーム反復で使用可能な目標

カードに目標をリストする必要なく、目標をイテレーションに追加する機能を追加しました。 目標はチェックリスト形式で追加され、完了とマークできます。 反復の右上にある指標領域には、目標の数と完了数が表示されます。

また、「次の反復」(Next Iteration) 列がイテレーションボードで使用できるようになりました。 この列にカードを配置すると、そのカードは次の反復に自動的に持ち込まれ、バックログには戻りません。 次の反復では、カードのステータスに対応する列にカードが表示されます。

詳しくは、 [ワークストリームでの反復の作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

## ボードのカードにコメントを追加する

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ボード上のアドホックカードと接続されたカードの両方にコメントを追加し、そのコメントで他のユーザーにタグ付けできるようになりました。 コメントはカードの詳細で確認できます。 ボードのコメント機能は、新しいAdobe Workfrontのコメント機能を使用します。

詳しくは、 [ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) および [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3420832/){target=_blank}

## Boards タグマネージャーの機能強化

タグマネージャーのインターフェイスが改善され、新しいタグをすばやく作成して、カードに適用できるようになりました。 また、ワークストリーム用のタグを作成することもできます。

詳しくは、 [タグを追加](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

## ボードの取り込み口列で使用可能な単純なフィルタ

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

インテーク列の設定にシンプル化されたフィルターが追加され、インテーク列をより迅速に定義できるようになりました。 使用可能なフィルターは、Workfrontプロジェクトと、チームまたはユーザーによる割り当てです。 必要に応じて、詳細フィルターに切り替えることができます。

詳しくは、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3419420/){target=_blank}

## ダイナミックボードテンプレートに追加されたシンプルなフィルター

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

ダイナミックボードテンプレート上のフィルターが簡素化され、ボードをより迅速に作成できるようになりました。 使用可能なフィルターは、Workfrontプロジェクトと、チームまたはユーザーによる割り当てです。 必要に応じて、詳細フィルターに切り替えることができます。 これらのフィルターオプションは、ダイナミックボードの設定パネルにも表示されます。

詳しくは、 [ボードの作成または編集](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## ダイナミックボードテンプレート

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

新しいテンプレートであるダイナミックボードがスタンドアロンボードで使用できるようになりました。 このテンプレートは、ワークストリーム内のボードでは使用できません。

動的ボードを使用すると、Workfrontプロジェクトに基づいて、ボードにカードを自動的に挿入できます。 フィルターを使用すると、カードはステータスに基づいて列に追加されます。

詳しくは、 [ボードの作成または編集](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3418600/){target=_blank}

## アジャイルチームかんばんカードをボードに移行

新しい **ボードに追加** アジャイルチームのボタンアジャイルチームかんばんボードを使用すると、かんばんボードからWorkfrontボードにすべてのカードを追加できます。 新しいWorkfrontボードを作成するか、既存のボードにカードを追加するかを選択できます。

Workfrontボードでのカードの配置は、列ポリシーに基づいています。 （例えば、ポリシーは、ステータスが「処理中」のすべてのカードを特定の列に移動できます）。 ポリシーがない場合や、カードがポリシーと一致しない場合、カードは一番左の列に配置されます。 現時点では、レガシーボードの「バックログ」列のカードはWorkfrontボードに追加されません。

カードはアジャイルチームかんばんボードからは削除されず、カードの状態の変更は両方のボードに同期します。 Workfrontボードに切り替える準備が整うまで、両方のボードをアクティブにしておくことができます。

詳しくは、 [アジャイルチームかんばんカードをWorkfrontボードに移行](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3420425/){target=_blank}

## ボードのカードの詳細に左側のナビゲーションが追加されました

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。

Workfrontボードのカードにフィールドオプションが追加されるにつれ、カードの詳細は長くなっています。 カードの詳細の左側にある新しいナビゲーションパネルを使用すると、セクションを選択して、そのフィールドグループに自動的に移動できます。

また、「説明」フィールドに URL を追加できるようになりました。URL は、カードの詳細を保存する際に、クリック可能なリンクになります。 これらの更新は、アドホックカードと接続されたカードの両方に適用されます。

詳しくは、 [ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) および [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3418598/){target=_blank}

## 電子メール通知と環境設定をボード

>[!NOTE]
>
>この機能は、Workfront Boards の初期の機能オプトインでのみ利用できます。 通常、電子メール通知はプレビューでは使用されないので、この機能は（初期の機能のオプトインのお客様のみ）プレビューと実稼動に同時にリリースされました。

Adobe Workfrontボードで電子メール通知を利用できるようになりました。 通知はデフォルトでオンになっており、環境設定で受信する電子メールを選択できます。 ボードに追加されたときや、カードが割り当てられたときに、電子メールが送信されます。

詳しくは、 [電子メール通知と環境設定をボード](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3418597/){target=_blank}
