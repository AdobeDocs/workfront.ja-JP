---
title: 22.4 管理者の機能強化
description: 22.4 管理者の機能強化
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4 管理者の機能強化

このページでは、プレビュー環境の 22.4 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、2022 年 10 月 3 日の週に提供されます。

22.4 リリースで使用可能なすべての変更点の一覧については、 [22.4 リリースの概要](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 承認プロセスでのロック解除済みステータスの使用

>[!NOTE]
>
>この機能は、22.3 リリース期間中に、プレビュー環境で初めて導入されました。 実稼動環境へのリリースは 2022 年 9 月 15 日です。

システム内の承認プロセスとステータスをより詳細に制御できるように、ロックが解除されたシステムステータスに基づいて承認プロセスを作成できるようになりました。 さらに、承認プロセスで既に使用されているステータスをロック解除できるようになりました。 以前は、承認プロセスで使用されるシステムステータスをロックする必要がありました。 これにより、すべてのグループに対して（削除や名前の変更を行わなくても）使用できるようになったので、グループ管理者は、特定のニーズに合わせてグループのステータスリストを合理化できませんでした。

## メインメニューのブループリントアイコンが、レイアウトテンプレートによって制御されるようになりました

システム管理者は、レイアウトテンプレートの設定を使用して、メインメニューのブループリントアイコンを追加または削除できるようになりました。 これにより、誰がブループリントカタログを参照できるかをより詳細に制御できます。

次の場合に、メインメニューにブループリントアイコンが表示されます。

* ユーザーに割り当てられたレイアウトテンプレートがありません

* ユーザーのレイアウトテンプレートの「アクティブな項目」リストに「ブループリント」オプションが表示されます

* ユーザーのレイアウトテンプレートの「使用可能な項目」リストに「ブループリント」オプションが表示されているので、このアイコンはメインメニューには表示されません。

既存のレイアウトテンプレートにはブループリントアイコンが自動的に含まれます。管理者は、レイアウトテンプレートからアイコンを削除して、ブループリントカタログの表示を制限できます。 22.4 リリース以降に作成された新しいレイアウトテンプレートでは、「アクティブな項目」リストにブループリントアイコンが表示されます。

詳しくは、 [ブループリントへのアクセスを設定](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 発行ヘッダーのカスタマイズ

Workfrontまたはグループ管理者は、レイアウトテンプレートの使用時に問題のヘッダーに表示されるフィールドをカスタマイズできるようになりました。

この更新で強化された機能は次のとおりです。

* イシューヘッダーから既存のフィールドを削除または並べ替えます。

* 編集不可能な新しい「問題の概要」フィールドを追加します。 編集可能なカスタムフィールドやカスタムフィールドは追加できません。 また、現在問題ヘッダーにある編集可能なフィールド（「ステータス」や「完了率」など）を表示することもできます。

* 問題ヘッダーには、最大 5 つのフィールドを含めることができます。

* これで、「解決者」フィールドをイシューヘッダーに追加できます。 解決オブジェクトが問題に関連付けられている場合、問題に関連付けられているオブジェクトの種類に応じて、「解決者」フィールドが「問題の解決」、「タスクの解決」、「プロジェクトの解決」に変わります。

このリリース以前は、プロジェクトヘッダーとタスクヘッダーのみをカスタマイズできました。



詳しくは、 [レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412383/){target=_blank}

## タスクヘッダーのカスタマイズ

Workfrontまたはグループ管理者は、レイアウトテンプレートの使用時にタスクのヘッダーに表示されるフィールドをカスタマイズできるようになりました。

この更新で強化された機能は次のとおりです。

* タスクヘッダーから既存のフィールドを削除または並べ替えます。

* 編集不可能な新しい「タスクの概要」フィールドを追加します。 編集可能なカスタムフィールドやカスタムフィールドは追加できません。 また、現在タスクヘッダーにある編集可能なフィールド（「ステータス」や「完了率」など）を表示することもできます。

* タスクヘッダーには、最大 5 つのフィールドを含めることができます。

このリリース以前は、カスタマイズできたのはプロジェクトヘッダーのみでした。

詳しくは、 [レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412384/){target=_blank}

## ボードの最新の機能に対する初期の機能オプトイン

初期の機能オプトイン用に新しいボード機能を開くことができます。 このオプションツールは、すべての組織で使用できます。

初期の機能をオプトインできるのは、Workfront管理者のみです。 管理者が初期の機能をオプトインすると、組織内のすべてのユーザーがオプトインし、追加の機能が実稼動用のWorkfront環境で有効になります。

詳しくは、 [Adobe Workfrontボードの初期機能のオプトイン](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412386/){target=_blank}

## カスタムフォームフィールドの計算エディターにエラー情報が表示されます

>[!NOTE]
>
>この機能は、22.3 リリース期間中に、プレビュー環境で初めて導入されました。 22.4 リリースで実稼動環境にリリースされます。

カスタムフィールドの計算を簡単に編集できるようになりました。計算に直接示される便利なエラー情報が追加されました。 カスタムフォームで計算フィールドを作成する場合、エラーはピンク色でハイライト表示されます。 ハイライト表示された部分にマウスポインターを置くと、問題の内容を示すツールチップが表示されます。

詳しくは、 [計算データをカスタムフォームに追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Unified Experience へのAdobeの移行

注意：この移行は 2023 年にQ1-Q2 に延期されました。 該当するお客様には、その時点で通知が送信されます。

組織がAdobe Admin Consoleにオンボーディングされている場合、Workfrontインスタンスは 22.4 リリースのAdobeUnified Experience に移行されます。

AdobeUnified Experience には次の内容が含まれます。

* Adobe Experience Cloudを介したすべてのAdobe・アプリケーションへの 1 回のログイン

* Workfrontの組織と環境の間を移動する「組織の切り替え」

* Workfrontページ、Adobe Experience Cloud環境設定およびWorkfrontプロファイルのオプションを使用したナビゲーション

詳しくは、 [Workfront向けAdobe統合エクスペリエンス](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3412388/){target=_blank}
