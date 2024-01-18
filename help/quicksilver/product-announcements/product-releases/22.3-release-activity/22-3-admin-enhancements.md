---
title: 22.3 管理者の機能強化
description: 22.3 管理者の機能強化
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 22.3 管理者の機能強化

このページでは、プレビュー環境の 22.3 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、2022 年 7 月 11 日の週に公開されました。 22.3 リリースで使用可能なすべての変更点の一覧については、 [22.3 リリースの概要](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Adobe Workfrontと JumpSeat の統合

JumpSeat とWorkfrontを統合して、ユーザー向けのカスタムの製品内ガイダンスを作成できるようになりました。 統合を有効にするには、Adobe Workfrontエンタープライズライセンスとアクティブな JumpSeat サブスクリプションが必要です。

詳しくは、 [JumpSeat 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## 配達確認のデフォルト設定がWorkfrontに移動されました

「Workfront Setup」領域内で、次の配達確認設定を編集できるようになりました。

* 配達確認のデフォルト設定

* 配達確認の決定設定

詳しくは、 [デフォルトの配達確認設定を構成](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## 承認プロセスでのロック解除済みステータスの使用

**注意：** 22.3 実稼動版リリースから削除されました。 この機能は、2022 年 9 月 16 日に実稼動環境にリリースされる予定です。

システム内の承認プロセスとステータスをより詳細に制御できるように、ロックが解除されたシステムステータスに基づいて承認プロセスを作成できるようになりました。 さらに、承認プロセスで既に使用されているステータスをロック解除できるようになりました。

以前は、承認プロセスで使用されるシステムステータスをロックする必要がありました。 これにより、すべてのグループに対して（削除や名前の変更を行わなくても）使用できるようになったので、グループ管理者は、特定のニーズに合わせてグループのステータスリストを合理化できませんでした。

詳しくは、次の記事を参照してください。

* [作業項目の承認プロセスの作成](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [ステータスの作成または編集](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [システムレベルのステータスのロックとロック解除](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## カスタムフォームにPDFファイルを追加する

アドビでは、画像やビデオなど、新しく追加できるアセットウィジェットを使用して、カスタムフォームをより視覚的かつ有益に作成するのに引き続き役立ちます。 これで、カスタムフォームにPDFファイルへのリンクを追加できます。 フォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーは、フォーム内からPDFの表示と操作を行うことができます。

詳しくは、 [カスタムフォームでの画像や他のアセットウィジェットの追加や編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## カスタムフォームフィールドの計算エディターにエラー情報が表示されます

>[!NOTE]
>
>この機能は一時的に利用できません。 このページは、この機能が使用可能になると更新されます。

カスタムフィールドの計算を簡単に編集できるようになりました。計算に直接示される便利なエラー情報が追加されました。 カスタムフォームで計算フィールドを作成する場合、エラーはピンク色で強調表示されます。 ハイライト表示された部分にマウスポインターを置くと、問題の内容を示すツールチップが表示されます。

詳しくは、 [計算データをカスタムフォームに追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## プロジェクトヘッダーのカスタマイズ

Workfrontまたはグループ管理者は、レイアウトテンプレートの使用時にプロジェクトのヘッダーに表示されるフィールドをカスタマイズできるようになりました。

この更新で強化された機能は次のとおりです。

* プロジェクトヘッダーから既存のフィールドを削除します。

* 編集不可能な新しい「プロジェクト概要」フィールドを追加します。 編集可能なカスタムフィールドやカスタムフィールドは追加できません。 現在プロジェクトヘッダーにある編集可能なフィールドは、ヘッダーに残ることができます。

* オブジェクトヘッダーには、最大 5 つのフィールドを含めることができます。


このリリースより前は、オブジェクトヘッダーのフィールドをカスタマイズできませんでした。

詳しくは、 [レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## 空のプロジェクトの作成を制御

システム管理者またはグループ管理者は、テンプレートを使用せずに、空白のプロジェクトを作成できるかどうかを制御できるようになりました。 「設定」の「プロジェクトの環境設定」領域に新しい設定が追加され、次の領域で空のプロジェクトの作成を無効にできるようになりました。

* プロジェクトのリストの「新規プロジェクト」オプションから

* イシューページからイシューをプロジェクトに変換する場合


新しい設定は、「ユーザーがテンプレートを使用せずにプロジェクトを作成できるようにする」で、デフォルトで有効になっています。

**注意：** ユーザーは、引き続きタスクを空のプロジェクトに変換できます。

詳しくは、 [システム全体のプロジェクト環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## グループページからグループを非アクティブ化します。

最近では、グループの非アクティブ化と再アクティブ化の機能が追加されました。 この操作を迅速かつ容易にするために、グループのページに追加しました。 グループ名をクリックしてそのページに移動した後、その他のメニューを選択できます。 ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) グループ名の横にある「非アクティブ化」または「再アクティブ化」を選択します。

以前は、グループの詳細ページの「アクティブ」チェックボックスを使用してのみ、グループのアクティベートを解除または再アクティブ化できました。

詳しくは、 [グループの非アクティブ化または再アクティブ化](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## カスタムフォームにビデオを追加する

ビデオを追加することで、新しい情報、視覚的な興味、創造性をカスタムフォームに提供できます。 フォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーはいつでもビデオを再生できます。

以前は、カスタムフォームに追加できるのはテキストベースのフィールドと画像だけです。

詳しくは、 [カスタムフォームでの画像またはビデオアセットウィジェットの追加または編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

