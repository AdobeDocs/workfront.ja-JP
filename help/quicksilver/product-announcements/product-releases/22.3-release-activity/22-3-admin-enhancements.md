---
title: 22.3 管理者向けの機能強化
description: 22.3 管理者向けの機能強化
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 100%

---

# 22.3 管理者向けの機能強化

このページでは、22.3 リリースで行われたプレビュー環境の管理者向けの機能強化について説明します。これらの機能強化は、2022年7月11日（PT）の週に公開されました。22.3 リリースで使用可能なすべての変更点の一覧については、[22.3 リリースの概要](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)を参照してください。

## Adobe Workfront と JumpSeat を統合

JumpSeat とWorkfront を統合して、ユーザー向けのカスタムガイダンスを製品内で作成できるようになりました。統合を有効にするには、Adobe Workfront エンタープライズライセンスと、アクティブな JumpSeat サブスクリプションが必要です。

詳しくは、[JumpSeat 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md)を参照してください。

## プルーフのデフォルト設定を Workfront に移動

Workfront の設定エリアで、次のプルーフ設定を編集できるようになりました。

* プルーフのデフォルト設定

* プルーフ決定の設定

詳しくは、[プルーフのデフォルト設定](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)を参照してください。

## ロックを解除されたステータスを承認プロセスで使用

**メモ：** 22.3 実稼動版リリースから削除されました。この機能は、2022年9月15日（PT）に実稼動環境にリリースされる予定です。

システム内の承認プロセスとステータスをより詳細に制御できるように、ロックが解除されたシステムステータスに基づいて承認プロセスを作成できるようになりました。さらに、承認プロセスで既に使用されているステータスをロック解除できるようになりました。

以前は、承認プロセスで使用するシステムステータスは、ロックする必要がありました。これはすべてのグループに当てはまるので、ステータスの削除や名前の変更を行うことができず、グループ管理者は、個々のニーズに合わせてグループのステータスリストを合理化できませんでした。

詳しくは、次の記事を参照してください。

* [作業項目の承認プロセスの作成](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [ステータスの作成または編集](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [システムレベルのステータスのロックとロック解除](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## カスタムフォームに PDF ファイルを追加

画像や動画などの新しいアセットウィジェットを追加することで、より視覚的で役に立つカスタムフォームを作成できるようになります。カスタムフォームに PDF ファイルへのリンクを追加できるようになりました。フォームがオブジェクトに添付されていると、オブジェクトを操作するユーザーは、フォーム内から PDF の表示と操作を行うことができます。

詳しくは、[カスタムフォームでの画像や他のアセットウィジェットの追加と編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)を参照してください。

## カスタムフォームフィールドの計算エディターにエラー情報を表示

>[!NOTE]
>
>この機能は一時的に利用できません。このページは、この機能が使用可能になれば更新されます。

カスタムフィールドの計算を簡単に編集できるようになり、役に立つエラー情報が計算に直接表示されるようになりました。カスタムフォームで計算フィールドを作成しているとき、エラーがピンク色で強調表示されます。強調表示された部分にカーソルを合わせると、問題の内容を説明したツールヒントが表示されます。

詳しくは、[計算データのカスタムフォームへの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)を参照してください。

## プロジェクトヘッダーのカスタマイズ

Workfront 管理者またはグループ管理者は、レイアウトテンプレートの使用時にプロジェクトのヘッダーに表示されるフィールドをカスタマイズできるようになりました。

この更新で強化された機能は次のとおりです。

* プロジェクトヘッダーから既存のフィールドを削除。

* 編集不可能な新しい「プロジェクト概要」フィールドを追加。編集可能なフィールドやカスタムフィールドは追加できません。現在プロジェクトヘッダーにある編集可能なフィールドは、ヘッダーに残すことができます。

* オブジェクトヘッダーには、最大 5 つのフィールドを含めることができます。


このリリースより前は、オブジェクトヘッダーのフィールドをカスタマイズできませんでした。

詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

## 空のプロジェクトの作成を制御

システム管理者またはグループ管理者は、テンプレートを使用せずに、空のプロジェクトを作成できるかどうかを制御できるようになりました。設定のプロジェクトの環境設定領域に新しい設定が追加され、次のエリアで空のプロジェクトの作成を無効にできるようになりました。

* プロジェクトのリストの「新規プロジェクト」オプションから

* イシューページからイシューをプロジェクトに変換する場合


新しい設定は「テンプレートを使用せずにユーザーによるプロジェクト作成を許可する」で、デフォルトで有効になっています。

**メモ：** ユーザーは、引き続きタスクを空のプロジェクトに変換できます。

詳しくは、[システム全体のプロジェクト環境設定の設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

## グループページからグループを非アクティブ化します。

最近では、グループの非アクティブ化と再アクティブ化の機能が追加されました。この操作を迅速かつ容易にするために、グループのページに追加しました。グループ名をクリックしてそのページに移動した後、グループ名の横にある詳細メニュー ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) を選択して、「非アクティブ化」または「再アクティブ化」を選択できます。

以前は、グループの詳細ページの「アクティブ」チェックボックスを使用してのみ、グループの非アクティブ化または再アクティブ化できました。

詳しくは、[グループの非アクティブ化または再アクティブ化](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)を参照してください。

## カスタムフォームにビデオを追加する

ビデオを追加することで、新しい情報、視覚的な興味および創造性をカスタムフォームに提供できます。フォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーはいつでもビデオを再生できます。

以前は、カスタムフォームに追加できるのはテキストベースのフィールドと画像だけでした。

詳しくは、[カスタムフォームでの画像またはビデオアセットウィジェットの追加または編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)を参照してください。

