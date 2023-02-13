---
title: 22.1 管理者の機能強化
description: 22.1 管理者の機能強化
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# 22.1 管理者の機能強化

このページでは、プレビュー環境の 2.1 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、実稼動環境で利用できるようになります

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022 年 1 月 17 日の週。

22.1 リリースで使用可能なすべての変更点の一覧については、 [22.1 リリースの概要](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 「更新」領域にログインしたドキュメントのダウンロード

ユーザーがWorkfrontに保存しているドキュメントのダウンロード数を追跡できるように、ユーザーがドキュメントをダウンロードしたときに、そのドキュメントの更新領域にエントリが記録されるようになりました。

>[!NOTE]
>
>この機能は、新しくアップロードしたドキュメントのプレビューでテストすることをお勧めします。

オブジェクトに対するWorkfrontの自動更新の記録方法について詳しくは、 [システムで追跡された更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## アクセスレベルを使用したチームへのアクセス権の付与

「アクセスレベル」領域の新しいセクションでは、チームに対するユーザーのアクセスを管理するためのより詳細なコントロールを提供します。 チームを作成、編集および表示できるユーザーを決定できます。

これによって、ユーザのチームへの既存のアクセスが変更されることはありません。

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## グループマッピングがブループリントで使用できるようになりました

一部のブループリントにグループが含まれるようになり、ブループリントをインストールする前にカスタマイズできます。 ブループリント内のグループをWorkfrontインスタンス内の既存のグループにマッピングしたり、必要に応じて新しいグループを作成したりできます。

詳しくは、 [ブループリントの設定](../../../administration-and-setup/blueprints/configure-template-package.md).

## カスタムForms領域でのスタイル設定の更新

カスタムForms領域は、新しいWorkfrontエクスペリエンスの他の多くの領域と最新の状態にするための新しいルックアンドフィールを備えています。

カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 計算カスタムフィールドを作成するための多くの機能強化

新しい計算エディタで、次の追加を使用すると、計算カスタムフィールドをより簡単に作成できるようになりました。

* 計算の式の上にマウスポインターを置くと、説明、使用例、ヘルプ記事の詳細情報へのリンクなど、式に関する情報が表示されます。
* 追加する各式は、タイプに応じて色分けされます。 これにより、式を見つけやすくなり、式の種類をすぐに認識できます。
* 行番号は、長い計算で関数を識別し、参照するのに役立ちます。
* 式またはフィールド名の入力を開始すると、使用可能な項目のリストが表示され、必要な項目を選択できます。 また、開き丸括弧を入力すると、閉じ丸括弧が自動的に追加されます。
* 計算エディターを離れることなく、既存のオブジェクトを使用して計算結果をプレビューできます。

また、カスタマイズ可能な「説明」で、計算済みカスタムフィールドのテキストにカーソルを合わせると、フィールドの数式の表示と非表示を切り替えることができます。 これは、カスタムフォームに入力するユーザーがその情報を必要としないと考える場合に役立ちます。

計算カスタムフィールドの作成について詳しくは、 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## ステータスと会社に関する監査ログ情報の表示

設定の監査ログ領域でステータスや会社に関するインシデントの情報を表示すると、それらのインシデントのトラブルシューティングをより簡単におこなうことができます。

例：

* ステータスの名前変更、ロック、非表示のユーザー、および変更日時を確認できます。
* 会社から一部のメンバーやジョブの役割を削除したユーザーと削除したタイミングを確認できます。

監査ログ情報の表示については、 [監査ログの表示と書き出し](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## ブループリント会社のマッピングおよびその他の機能強化

次のブループリントの機能強化が利用できます。

* 一部のブループリントに会社が含まれるようになり、ブループリントをインストールする前にカスタマイズできます。 ブループリント内の会社をWorkfrontインスタンス内の既存の会社にマッピングしたり、必要に応じて新しい会社を作成したりできます。
* 新しいブループリントタイプ「組織構造」を使用できるようになりました。 一部のブループリントには、複数のタイプの要素（プロジェクトテンプレートや組織構造など）が含まれます。 カタログページでブループリントタイプでフィルタリングできます。
* 設定ページの「Install Preferences」と「Template Ownership」の各セクションが、簡単にするために「Template Preferences」に組み合わされました。

詳しくは、 [ブループリントの設定](../../../administration-and-setup/blueprints/configure-template-package.md).

## 会社メンバーシップをより簡単に管理

会社領域では、更新されたツールバーを使用すると、既存のWorkfrontユーザーを会社に簡単に追加したり、会社メンバーを削除したりできます。

以前は、これらの操作は「会社を編集」ボックスでのみ使用できました。

更新されたツールバーには、メンバーのユーザープロファイル情報の編集やシステムでの非アクティブ化など、前のツールバーで使用できたすべてのアクションも含まれています。

詳しくは、 [会社メンバーシップの管理](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 新しい計算フィールドウィンドウで式とフィールドを選択する

カスタムフォームでの計算フィールドの作成が、引き続き容易になります。 次に、[ 最大化 ] をクリックして新しい計算エディタを開くと、必要な式やフィールドを検索して選択できます。

詳しくは、 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## グループは、独自のタイムシートと時間の基本設定を構成できます

>[!NOTE]
>
>この機能は、最初は、21.4 リリースの一部として、Cluster 4 のお客様のみが段階的にロールアウトの一部として使用できました。 この機能は、2021 年 11 月 8 日に実稼動環境の残りのすべてのクラスタで使用できるようになります。

大規模な組織では、管理者がシステムレベルで設定した基本設定を継承するのではなく、固有のワークフローに合わせてタイムシートと時間の基本設定を個別に構成する必要がある場合があります。 Workfrontの管理者は、システム内のすべてのグループのタイムシートと時間の優先順位をロック解除して、自分で構成できるようになりました。

この機能は、最近、プロジェクトの環境設定や、タスクおよび問題の環境設定に追加されました。

Workfront管理者がタイムシートと時間の優先順位のロックを解除する方法の詳細については、「 [グループのタイムシートと時間の基本設定をロック解除](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 記事内 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

グループ管理者がグループのロック解除されたタスクと問題の環境設定を構成する方法について詳しくは、 [グループのタイムシートと時間の基本設定を構成する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## グループのロックを解除または再ロックする複数の通知を選択します

グループの電子メール通知のロック解除や再ロックがより速く、簡単になりました。 複数の通知を選択し、選択内容が正しいことを確認した後、ツールバーに表示される新しい「ロック解除」または「ロック」ボタンをクリックします。

以前は、通知のロックを解除し、一度に 1 つずつ再ロックする必要がありました。 Workfrontには現在 95 の通知があるので、すべてまたは多くの通知に対しておこなう必要がある場合は時間がかかりました。

詳しくは、 [すべてのグループのイベント通知の設定をロック解除またはロックします](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## グループ管理者の場合：グループの削除時に置き換えグループを簡単に選択できる

グループを削除する場合は、[ グループの削除 ] ボックスに 2 つの改善点があり、削除したグループのユーザー、作業項目、サブグループを保持する置換グループを簡単に選択できます。

* グループの名前を入力すると、すばやく見つけることができます。 以前は、入力できないドロップダウンリストしかありませんでした。 多数のグループを持つ組織では、必要なグループを見つけるためにリストをスクロールする必要があるので、この問題が発生していました。 また、ドロップダウンリストに項目数の制限があるので、必要なグループが表示されない可能性がありました。
* 新しい情報アイコンを使用して、必要な置換グループを選択していることを確認できます。 アイコンの上にマウスポインターを置くと、グループの上位のグループの階層や管理者の名前など、グループに関する情報が一覧表示されるツールチップが表示されます。

詳しくは、 [グループの削除](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## 集計フィールドを作成する領域が大きい

これで、カスタムフォームで複雑な計算フィールドを簡単に作成できます。 新しい「最大化」ボタンをクリックして、計算を作成するための大きな編集ウィンドウを開きます。 完了したら、「最小化」をクリックして、カスタムフォームの作業を続行します。

詳しくは、 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## カスタムフォームをグループに追加する

Group オブジェクトでカスタムフォームがサポートされるようになりました。 これにより、組織内のグループが、特定のニーズやワークフローを満たす情報を容易に取得および共有できます。 他のWorkfrontオブジェクトと同様に、ユーザーはグループに対して次の操作を実行できます。

* カスタムフォームの作成
* カスタムフォームを添付
* カスタムフォームデータを保存
* カスタムフォームの削除
* リストのカスタムデータを編集し、新しいWorkfrontエクスペリエンスで、グループページからカスタムデータを編集します。

カスタムフォームについて詳しくは、 [カスタムフォーム](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## OAuth2 アプリを作成してアプリケーションをWorkfrontと統合する

Workfrontを、Workfrontに組み込み統合を提供していない他のアプリケーションと統合できるようになりました。 統合するアプリケーションの OAuth2 アプリを作成すると、データが安全な業界標準の OAuth2 認証プロトコルで保護されていることを知りながら、そのアプリケーションがWorkfrontにアクセスできるようになります。

以前は、組み込みの統合、Workfront Fusion、Workfront API を使用して、他のアプリケーションとのみ統合できました。

詳しくは、 [Workfront統合用の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 会社領域のインターフェイステキストの改善

「設定」の「会社」領域で、新しい確認メッセージと若干の変更により、会社のメンバーシップを管理しやすくなります。 例えば、左側のパネルのセクション名「People」は、「会社メンバー」になりました。

会社メンバーシップの管理について詳しくは、 [会社メンバーシップの管理](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
