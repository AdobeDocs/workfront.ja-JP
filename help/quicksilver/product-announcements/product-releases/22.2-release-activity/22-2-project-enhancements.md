---
title: 22.2 プロジェクトの機能強化
description: 22.2 プロジェクトの機能強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 100%

---

# 22.2 プロジェクトの機能強化

このページでは、22.2 リリースのプレビュー環境で行われたすべてのプロジェクトの機能強化について説明します。これらの機能強化は、

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日（PT）の週に実稼動環境で公開されます。22.2 リリースで利用可能なすべての変更点の一覧については、[22.2 リリースの概要](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)を参照してください。

## Adobe Workfront のボードを利用できるようになりました。

ボードは、列やカードを含む共有ボードにアクセスできる、チームコラボレーションを可能にする柔軟なツールです。

ボードを使用してできること：

* 複数の列を持つタスクボードをすばやく設定する
* ステータスまたはカテゴリを表示する列を設定する
* 他のユーザーをボードに追加し、カードに割り当てる
* 自由形式のカードとチェックリストをすばやく追加

ボード上のカードは、Adobe Workfront のオブジェクトや作業アイテムには接続されません。

このオプションをすべてのユーザーが利用できるようにするには、システム管理者がメインメニューのレイアウトテンプレートのボードを有効にする必要があります。

詳しくは、[ボードの概要](../../../agile/boards-overview.md)を参照してください。

## Workfront ボードのその他の機能強化

Workfront ボードで、次の機能強化が行われました。

* ボードでのカードのタグ付け

  これで、ボード上のカードを色分けしたタグで分類できるようになりました。タグを使用すると、カードをすばやく識別できます。適用したタグに基づいてボードを並べ替えることもできます。

* ボードでのカードの管理

  ボード上のカードの管理に役立つ次の機能が追加されました。

   * カードのコピー：ボード上に既存のカードのコピーを作成します。
   * カードの移動：新しい「列の一番上」と「列の一番下」メニューオプションを使用して、ボードの一番上または一番下にカードをすばやく移動できます。

* ボードでの検索

  ボード上のすべてのカードを検索するのに役立つ検索バーが追加されました。

* ボードでカードの期限を設定する

  ボード上の個々のカードに期限を設定できるようになりました。

詳しくは、[Adobe Workfront でのボードの概要](../../../agile/get-started-with-boards/get-started-with-boards.md)を参照してください。

## 「投稿を更新」の取り消しオプション

更新を投稿する際の間違いを容易に発見できるようになりました。オブジェクトの「更新」タブでコメントを確定した後、ポップアップウィンドウが7秒間表示されるようになり、システムがタイムスタンプを付けたり、メールやアプリ内通知を送信する前に、投稿をキャンセルして編集に戻ることができるようになりました。ポップアップウィンドウを閉じるか、ページを離れるか、ウィンドウがタイムアウトするまで 7 秒待つと、投稿は通常どおり行われます。

詳しくは、[作業を更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

## イシューをコピーおよび移動する際のエクスペリエンスのアップデート

Workfront の使用を新しい Adobe Workfront エクスペリエンスと一致させるため、イシューのコピーと移動のためのインターフェイスを再設計しました。これは、現在、単一のイシューをコピーまたは移動する場合や、リストまたはレポートから一括してイシューをコピーまたは移動する場合に使用できます。

この新しく再設計されたインターフェイスの改善点には次のようなものがあります。

* 移動前に更新する必要があるすべての情報が、連続した 1 ページに表示されます。
* Workfront は、プロジェクトを選択した直後に、宛先プロジェクトにアクセスできるかどうかを確認します。この機能強化が行われる前、Workfront では、移動を確認した後に正しいアクセス権がないという警告が表示され、余分な手順が発生して移動が許可されませんでした。
* 「タスクの移動」ボックスを離れることなく、タスクを移動するプロジェクトへのアクセスを要求する機能。
* イシューを別の場所に移動したときに、イシューから項目（割り当て、進捗、ドキュメント、権限、更新）を削除する機能。以前は、この機能はイシューのコピーに対してのみ使用できました。
* イシューをコピーする際に、コピー先のプロジェクトの選択に加えて、コピー先のタスクを選択する機能。

イシューの移動またはコピーについて詳しくは、次の記事を参照してください。

* [イシューをコピー](../../../manage-work/issues/manage-issues/copy-issues.md)
* [イシューを移動](../../../manage-work/issues/manage-issues/move-issues.md)

## プロジェクトをコピーする際の新しいエクスペリエンス

Workfront の使用と新しい Adobe Workfront エクスペリエンスの一貫性を保つため、プロジェクトをコピーするためのインターフェイスのデザインを変更しました。これは、現在、プロジェクトページからプロジェクトをコピーする場合、またはリストやレポートからプロジェクトをコピーする場合に使用できます。この更新以前は、プロジェクトページからのみプロジェクトをコピーできました。

詳しくは、[プロジェクトのコピー](../../../manage-work/projects/manage-projects/copy-project.md)を参照してください。

## 新しい詳細メニューのリストやレポートからプロジェクトを管理できる機能

プロジェクトリストとレポートに新しいその他メニューが追加され、これらの領域から次の操作を実行できるようになりました。

* 一度に複数のプロジェクトを扱う場合
* タイムラインを再計算
* 財務を再計算
* カスタム式を再計算
* 単一のプロジェクトの場合
* テンプレートを添付
* MS Project にエクスポートする
* 登録

詳しくは、次の記事を参照してください。

* [プロジェクトタイムラインの再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [プロジェクトの財務を再計算](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [カスタムフォームフィールドの情報の編集](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [プロジェクトへのテンプレートの添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [プロジェクトを Microsoft Project に書き出し](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Adobe Workfront の項目を購読](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## イシューをプロジェクトに変換した後に、ダッシュボード、リストまたはレポート上でユーザーを保持

効率を高め、クリック数を減らすために、イシューをリスト、レポート、またはダッシュボードからプロジェクトに変換する際の改善点をリリースしました。

イシューをプロジェクトに変換した後、プロジェクトのページにリダイレクトされるのではなく、ユーザーがリスト、レポート、またはダッシュボードにとどまります。変換処理の完了後、プロジェクトへのリンクが付いた成功通知が表示され、必要に応じて簡単にプロジェクトに移動できます。

詳しくは、[イシューを Adobe Workfront のプロジェクトに変換](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)を参照してください。

## 割り当てに変更を加える際に、配分時間が削除されなくなります

>[!NOTE]
>
>この機能は、もともと 22.2 リリースで発表される予定でした。2022年4月21日（PT）に実稼動環境へリリースされます。

データの正確性を確保するため、割り当て時間を保持し、タスクの割り当てを変更する際にタスクの計画時間を変更しないように変更しました。

シンプルな期間タイプのタスクに対して、次の変更が加えられました。

* すべての担当者を削除しても、予定時間数は保持されます。
* ユーザーとロールを置き換える際に、個々の割り当ての割り当てが保持されます。
* ユーザーを削除しても、個別に付与された割り当ては役割に対して保持されます。（リリースから削除されました。すべての担当者を削除した後、予定時間数が 0 に設定されるようになりました。)

予定時間について詳しくは、[予定時間の概要](../../../manage-work/tasks/task-information/planned-hours.md)を参照してください。

## フォルダー階層の上位 5 レベルのみでフォルダーを共有

>[!NOTE]
>
>この機能は一時的に利用できません。この機能が実稼動で使用可能になったら、このリリースノートを更新します。

フォルダーを共有するユーザーにとって最高のパフォーマンスを確保するため、現在、共有は 1 つのオブジェクト上のフォルダー階層の上位 5 レベルに制限されています。

6 番目以下のフォルダーは、そのすぐ上のフォルダーから共有設定を継承します。

フォルダーの共有について詳しくは、[ドキュメントフォルダーを共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)を参照してください。

