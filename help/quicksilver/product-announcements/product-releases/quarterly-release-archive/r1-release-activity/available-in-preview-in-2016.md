---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2016 年のプレビューで使用可能になった機能
description: 2016 年のプレビュー環境では、次の機能が使用可能になりました。 これらの機能は、R1 リリースで実稼動環境にリリースされる予定です。
author: Luke
feature: Product Announcements
exl-id: 08e0bd72-5979-449e-9fb2-c4d45f51119e
source-git-commit: aa1bf796982fa91ff9096d92fef1fb95c2e29778
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# 2016 年のプレビューで使用可能になった機能

2016 年のプレビュー環境では、次の機能が使用可能になりました。 これらの機能は、R1 リリースで実稼動環境にリリースされる予定です。

## リソーススケジュールの改善

これで、リソースマネージャーであるプロジェクトのすべてのタスクが表示され、スケジュールに関する決定を行う際に、より詳細な情報を得ることができます。 

リソースのスケジュール設定に使用できるツールの一般情報については、 [リソーススケジュールの概要](../../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md)

スケジュールタイムラインに表示される情報を調整するには、 [スケジュール領域の情報のフィルタリング](../../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

自分が担当するプロジェクトのタスクの表示に加えて、スケジューリングタイムラインを使用して、リソース割り当てを変更できます。 スケジューリングタイムラインでユーザーの割り当てを管理する方法について詳しくは、 [スケジュール領域で未割り当てタスクとタスクを手動で割り当てる](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md)

## スケジューリングタイムラインでのユーザー割り当ての管理

新しいリソーススケジュールツールを使用してリソースをスケジュールする場合、タスクまたは問題の予定時間をユーザーに割り当てる方法を指定できるようになりました。 時間は、タスクの期間内および割り当てられたユーザー間で日数で割ることができます。

詳しくは、 [スケジューリング領域でユーザー割り当てを管理します](../../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md)

## ユーザーの割り当てはデフォルトで無効になっています

リソーススケジュール時のスケジュールタイムラインのユーザー割り当ての網掛けが、デフォルトで無効になりました。

以前は、配分の網掛けがデフォルトで表示されており、無効にできませんでした。

ユーザー割り当てオプションを有効にする方法について詳しくは、 [スケジューリング領域でユーザー割り当てを管理します](../../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) in  [スケジューリング領域でユーザー割り当てを管理します](../../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md)

## レイアウトテンプレートは、新しいカレンダーとレガシーカレンダーのどちらを作業領域に表示するかを決定します

**サンドボックスをプレビュー：2016 年 12 月 7 日；早期アクセス：2016 年 12 月 15 日** 

レイアウトテンプレートが適用されていない場合は、新しいカレンダーが [ 作業 ] 領域にデフォルトで表示されます。

選択した場合、タスクと問題に関するコミット日のみを表示するように設定された [ 作業用 ] 領域にレイアウトテンプレートを適用することで、[ 作業用 ] 領域に従来のカレンダーを表示するように構成できます。

[ 作業 ] 領域でレガシーカレンダーを使用する場合は、コミットした作業のみが表示されます。

レイアウトテンプレートの適用時にWorkfrontで新しいカレンダーを [ 作業 ] 領域に表示するように設定するには、レイアウトテンプレートを設定してタスクと問題に対する計画完了日を表示し、そのレイアウトテンプレートを適切なユーザーに割り当てます。

レイアウトテンプレートの設定について詳しくは、 [レイアウトテンプレートの作成と管理](../../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md#customizing-my-work) in [レイアウトテンプレートの作成と管理](../../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Outlook 365 ベータ版

**ベータ版：未定；パブリック可用性：未定**

次のセクションで説明するように、Outlook for Office 365 のWorkfrontを使用できます。

* [Outlook 用のAdobe Workfrontのセットアップ](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)
* &quot;Outlook 365 でのメールからの既存の項目の更新&quot;

## 任意のリスト内の列をドラッグ&amp;ドロップで並べ替える

**早期アクセス：2016 年 2 月 21 日**

リスト内の列の順序を変更するには、列をある場所から別の場所にドラッグ&amp;ドロップします。

これは、ガントチャートとリスト表示を同時に表示し、表示する列がページの左側に表示されない場合に特に便利です。 

詳しくは、 [列の幅と順序を変更する](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)

## ダッシュボードリストのルックアンドフィールを更新しました。

現在は、ダッシュボードのリストを表示する際のルックアンドフィールがより近代的で拡張性が高くなっています。

ダッシュボードについて詳しくは、 [ダッシュボードの作成](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)

## カスタムFormsへのアクセスの制御

**サンドボックスをプレビュー：2016 年 1 月 24 日**

個々のユーザー、チーム、役割、グループまたは会社にアクセス権を付与することで、カスタムフォームへのアクセス権を持つユーザーを制御できるようになりました。 

この変更を行う前は、グループに対してのみアクセス権を付与することができました。

詳しくは、 [カスタムフォームの作成または編集](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Adobe Creative Cloudとの統合

**アドオンは次の場所からダウンロードできます。2016 年 4 月**

Workfront Extension for Adobe Creative Cloudは、Creative Cloudで作成したアセットをWorkfrontに保存および書き出して、承認とレビューのプロセスを高速化できるように設計されています。
