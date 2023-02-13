---
content-type: release-notes
keywords: メモ，四半期，更新，リリース
navigation-topic: 2021-2-release-activity
title: 21.2 管理者の機能強化
description: このページでは、プレビュー環境の 21.2 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、2021 年 5 月 10 日の週に実稼動環境で利用可能になる予定です。 21.2 リリースで使用できるすべての変更点の一覧については、 21.2 リリースの概要を参照してください。
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 7ae5a04a-a9bc-4a85-8651-2b912f7fd7e4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# 21.2 管理者の機能強化

このページでは、プレビュー環境の 21.2 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、2021 年 5 月 10 日の週に実稼動環境で利用可能になる予定です。 21.2 リリースで使用可能なすべての変更点の一覧については、 [21.2 リリースの概要](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 管理者向け：Workfrontのその他の多くの領域に関する監査ログ情報の表示

「監査ログ」領域で、Workfront全体の様々な領域で変更を追跡し、トラブルシューティングできるようになりました。 ユーザーが次のいずれかの操作を行うと、監査ログエントリが生成されるようになりました。

* カスタムフォームを作成、変更、削除、または共有します
* カスタムフィールドの作成、変更、削除、共有を行います
* カスタムセクションを作成、変更、または削除します
* 為替レートを作成、変更、または削除します
* ジョブの役割を作成、変更、または削除します
* 優先度を作成、変更、または削除します
* 重大度を作成、変更、または削除
* 条件の作成、変更、削除
* プロジェクトの環境設定を変更するか、カスタム四半期を作成または削除します
* タスクと問題の環境設定を変更します

詳しくは、 [監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

この機能は、 [新しいWorkfrontエクスペリエンスの管理の基本、パート 2:プロジェクト設定](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) Workfront One の学習パス

## グループ管理者の場合：サブグループと更新されたツールバーを移動するためのコントロールを改善

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

セットアップのサブグループ領域で次の改善を行いました。

* 管理するグループを簡単に整理するために、「サブグループを追加」ツールバーボタンを追加し、新しいサブグループを作成して既存のサブグループを移動できます。

   詳しくは、 [サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

* サブグループ領域のツールバーで、新しいWorkfrontエクスペリエンスで、リストが他の最新化されたリストと一致するようになりました。 グループを選択すると、ツールバーで使用可能な機能がアイコンで表されます。

## 管理者向けの新機能：タイムシートと時間の環境設定ページのルックアンドフィールを更新しました

タイムシートと時間の環境設定ページの操作性を向上させるために、ユーザーインターフェイスを更新し、Workfrontの他の場所で見つかる最新の外観と操作性に合わせました。

セクションと個々のオプションは、より縦のスペースで区切られているので、読みやすくなります。

2 つのラジオボタンオプションのラベルは、それほど長くはないように分割されます。各ラベルの 2 番目の部分は、別々の行の情報メッセージになります。

タイムシートと時間の優先順位の詳細については、 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## グループ管理者の場合：グループ領域のリストの改善

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

セットアップのグループ領域で次の 2 つの機能が強化され、新しいWorkfrontエクスペリエンスの他の最新化されたリストと一致するリストが作成されました。

* グループを選択すると、ツールバーで使用可能な機能がアイコンで表されます。
* グループ、列、並べ替え、階層のリストでは、他のリストに慣れている方が新しい外観と操作性を持ちます。 また、デフォルトでは、1 つのページに最大 2,000 個の項目が表示され、100 個の項目は表示されません。

Workfront全体で最新化されたリストについて詳しくは、 [リストの表示方法を変更する](../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md).

グループ領域について詳しくは、 [グループの管理](../../../administration-and-setup/manage-groups/manage-groups.md).

## グループ管理者の場合：セットアップのグループ領域からプログラムを作成および編集する

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

アドビでは、グループとその関連オブジェクトを 1 か所で容易に管理できるようにし続けています。 これで、セットアップの [ グループ ] 領域で、グループのプログラムを表示して操作できるようになりました。 これにより、グループのプログラムを管理するために [ プログラム ] 領域に移動する必要がなくなります。 また、使用しているグループプログラムのリストを、システム内の他のプログラムとは別に保持します。

詳しくは、 [グループのプログラムの作成、変更、表示](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## 管理者向け：セットアップ領域の更新されたヘッダー

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

Setup 領域の管理者の向きをよりよくし、Adobe Workfrontの一貫性を維持するために、Setup ヘッダーを次のように更新しました。

* 各設定ページとサブページを示す大きなカラフルなバッジ
* 各サブページの名前の上の階層情報（例：単一のグループのページ上）
* フォントのスタイルとサイズを最新化

   ![](assets/updated-headers-in-setup-02-29-21-350x214.png)

設定領域について詳しくは、 [管理と設定](../../../administration-and-setup/administration-and-setup.md).

## グループ管理者の場合：グループページで追加のグループオブジェクトを表示および管理します

>[!NOTE]
>
>この機能は、新しいAdobe Workfrontエクスペリエンスでのみ使用できます

アドビでは、グループとその関連オブジェクトを 1 か所で容易に管理できるようにし続けています。 これで、セットアップのグループ領域で、グループの会社、チームおよびポートフォリオを表示および操作できます。 これにより、これらのオブジェクトの様々なセットアップページに移動して、グループの管理を行う必要がなくなります。 見ているグループオブジェクトのリストをシステム内の他のグループのリストとは別に保持します

詳しくは、次の記事を参照してください。

* [グループの会社の作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md)
* [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md)
* [グループのチームの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)

## グループ管理者向けの新機能：グループタイムシートプロファイルを割り当て

管理するグループのタイムシートプロファイルを管理しやすくなりました。 タイムシートプロファイルを作成できるだけでなく、自分のグループに割り当てたり、自分のグループの個々のメンバに割り当てたりすることもできます。 これは、アクセスレベルで [ タイムシートと時間 ] オプションが有効になっていない場合でも当てはまります。

これまで、タイムシートプロファイルを割り当てるには、[ タイムシートと時間 ] オプションを有効にする必要がありました。 ただし、システム内のすべてのタイムシートと時間情報に対する表示と編集のアクセス権を付与するので、グループ管理者全員にとっては理想的ではない場合があります。 このレベルのアクセス権が必要ない場合は、グループのタイムシートプロファイルを管理できます。

詳しくは、 [タイムシートプロファイルの作成、編集、割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

アクセスレベルの [ タイムシートと時間 ] オプションの詳細については、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 管理者向け：ユーザーがオブジェクトリストに表示するフィルター、表示、グループ化を設定します

新しいWorkfrontエクスペリエンスのレイアウトテンプレートを使用すると、Workfront全体のオブジェクトリストにユーザーが表示するデフォルトのフィルター、表示、グループ化を設定できるようになりました。

たとえば、[ フィルタ一覧 ] のコントロールを [ すべて ] に設定したままにする代わりに、[ ホームチーム ] に変更することができます。 この方法では、ユーザーがオブジェクトのリストを表示すると、ユーザーのチームに関連付けられたオブジェクトのみが含まれます。

以前は、これらのデフォルトはカスタマイズできなかったので、フィルターの場合は常に「すべて」、ビューの場合は「標準」、グループの場合は「なし」に設定されていました。 新しい機能に加えて、これら 3 つの設定が不要な場合に、ユーザーに対して非表示にできる点が特に重要です。

詳しくは、 [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

この機能は、 [新しいWorkfront Experience の管理者向け基本、パート 3:コントロールとインターフェイスの操作](https://one.workfront.com/s/learningpath3/administrator-fundamentals-control-and-interface-experience-MCNCSSMXLPDFEERGVEM4EWL2I4LI) Workfront One の学習パス

## 管理者向けの新機能：現在カスタムフィールドを使用しているレポートを簡単にリスト

>[!NOTE]
>
>この機能は、2021 年 3 月 4 日に実稼動環境にリリースされました。

一部のAdobe Workfrontレポートに既に実装されているカスタムフィールドを編集または削除する必要がある場合は、変更後も正しく動作するために、それらのレポートに調整が必要かどうかを評価することが重要です。

カスタムForms領域にカスタムビューを追加し、特定のカスタムフィールドを使用しているレポートを示す新しい「レポート」列を追加できます。

以前は、この列がない場合、テキストモードでレポートを手動で作成するか、別の回避策を使用して、レポートでどのカスタムフィールドが使用されているかを調べる必要がありました。 組織で多くのカスタムフィールドを使用する場合は、これは困難で面倒です。

詳しくは、 [特定のカスタムフィールドまたはウィジェットを使用するすべてのレポートを表示する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).

## グループ管理者の場合：1 か所でグループとそのオブジェクトを表示、管理する

>[!NOTE]
>
>この機能は、新しいAdobe Workfrontエクスペリエンスでのみ使用できます

セットアップの [ グループ ] 領域でグループを表示すると、グループを管理しやすくなりました。 新しい「その他」メニューを使用すると、グループページに戻ることなく、グループの編集、コピー、削除をすばやくおこなうことができます。 詳しくは、 [グループの管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

また、グループのページから、グループのレイアウトテンプレート、集計表、タイムシートプロファイル、サブグループメンバを表示し、操作することもできます。 これにより、これらのオブジェクトの様々なセットアップページに移動して、グループの管理を行う必要がなくなります。 また、グループのオブジェクトのリストは、システム内の他のグループのリストとは別に保持されます。

詳しくは、次の記事を参照してください。

* [グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)
* [グループのスケジュールの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md)
* [グループのタイムシートプロファイルを作成および管理する](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)
* [サブグループメンバーの表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)

## 管理者向けの新機能：カスタムフォームフィールドで使用可能なその他のテキスト書式設定オプション

書式設定が可能なカスタムフォームフィールドに入力すると、太字、斜体、下線に加えて、箇条書き、段落番号、ハイパーリンク、ブロック引用符を使用してテキストを整理できるようになりました。

詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

