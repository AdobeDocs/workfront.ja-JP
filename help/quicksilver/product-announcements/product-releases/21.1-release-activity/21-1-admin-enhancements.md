---
content-type: release-notes
keywords: メモ，四半期，更新
navigation-topic: product-releases
title: 21.1 管理者の機能強化
description: このページでは、プレビュー環境の 21.1 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、2021 年 2 月 15 日の週に実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 21.1 管理者の機能強化

このページでは、プレビュー環境の 21.1 リリースでおこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、2021 年 2 月 15 日の週に実稼動環境で利用可能になる予定です。

21.1 リリースで使用可能なすべての変更点の一覧については、 [21.1 リリースの概要](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## プロジェクトをコピーするための新しいアクセスレベル設定を導入しました

システム管理者は、プロジェクトでプランナが実行できる操作をより詳細に制御できるように、新しい設定を導入して、プロジェクトのコピー機能を有効または無効にすることで、アクセスレベルでプロジェクトの編集アクセスをより詳細にしました。 この変更がおこなわれる前は、ユーザーのプロジェクト編集へのアクセスを有効にした場合、ユーザーは自動的にそれらのプロジェクトをコピーするためのアクセス権を持っていました。 新しい機能を使用すると、新しい [ コピー ] 設定を無効にして、必ずしもプロジェクトをコピーするアクセス権を持たずに、他のユーザーに編集プロジェクトへのアクセス権を付与できます。

この変更以前に、ユーザーがアクセスレベルでプロジェクトを編集にアクセスできた場合、この機能のリリース時に、この設定が自動的に有効になります。

プランのアクセスレベルについては、 [プロジェクトへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

プロジェクトのコピーについて詳しくは、 [プロジェクトのコピー](../../../manage-work/projects/manage-projects/copy-project.md).

この機能は、 [新しいWorkfrontエクスペリエンスの管理者の基本事項、パート 1:ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One の学習パス

## オブジェクトのカスタムフォームで、複数選択ドロップダウンフィールドのすべての項目を選択します

>[!NOTE]
>
>この機能は、現在、新しいリクエストを送信する際には使用できません。

オブジェクトの詳細ページで、カスタムフォームの複数選択ドロップダウンフィールドに入力する際に、使用可能なすべてのオプションを選択する必要がある場合は、「すべて選択」をクリックします。

カスタムフォーム上のデータの編集について詳しくは、 [カスタムフォームフィールドの情報を編集](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## オブジェクトのすべてのカスタムフォームフィールドを再計算する

オブジェクトの計算カスタムフィールドのすべてのデータを最新の状態に保つのが簡単になりました。 新しい [ 式を再計算 ] メニューオプションを使用すると、これらのフィールド内のすべてのデータをすばやく再計算できます。

これは、オブジェクト内の計算カスタムフィールドで参照される別のオブジェクト内のデータを編集した後に特に便利です。

以前は、計算されたカスタムフィールド内のすべてのデータが最新であることを確認するために、回避策を使用する必要がありました。 例えば、オブジェクトを他のオブジェクトと共に編集し、一括編集が可能な再計算オプションを使用しました。

詳しくは、 [カスタムフォームフィールドの情報を編集](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## グループ管理者のタスクと問題の環境設定をロック解除

>[!NOTE]
>
>2021 年 6 月 24 日までは、段階的なロールアウトの一環として、グループのプロジェクト設定をロック解除できるお客様のみに対して使用できました。 現在は、すべてのお客様が利用できます。

Adobe Workfrontの管理者は、個々のタスクと問題の環境設定をロック解除することで、グループ管理者にさらに自律性を与えることができるようになりました。 グループ管理者は、環境設定のロックが解除されると、各グループの固有のニーズと内部プロセスに対応するように、グループ用に環境設定を構成できます。

詳しくは、 [グループのタスクと問題の環境設定を設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

この機能は、 [新しいWorkfrontエクスペリエンスの管理者の基本、パート 2:プロジェクト設定](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) Workfront One の学習パス

## ポートフォリオとプログラムのアクセスレベルを個別に設定する

ポートフォリオとプログラムへのユーザーアクセスを管理しやすくなりました。ポートフォリオとプログラムのアクセスレベルを個別に設定できるからです。

以前は、ポートフォリオとプログラムのアクセスレベル設定を組み合わせていました。 つまり、ポートフォリオの場合と同じ方法でプログラムのアクセス設定を設定しないと、その逆も同じことができました。

アクセスレベルの設定について詳しくは、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

プログラムおよびポートフォリオ用に設定できるアクセス設定については、 [各オブジェクトタイプの機能への設定可能なアクセス](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

この機能は、 [新しいWorkfrontエクスペリエンスの管理者の基本事項、パート 1:ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One の学習パス

## カスタムフォームで情報を編集する際に、一連のすべてのチェックボックスをオンにする

>[!NOTE]
>
>この機能は、現在、新しいリクエストを送信する際には使用できません。

オブジェクトの詳細ページで、チェックボックスを含むカスタムフォームフィールドに入力する際に、使用可能なすべてのチェックボックスをオンにする必要がある場合は、「すべて選択」をクリックします。

このオプションは、フィールドに 2 つ以上のチェックボックスが含まれている場合にのみ表示されます。

詳しくは、 [カスタムフォームフィールドの情報を編集](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Workfront E メールの設定を許可リスト行う

データのセキュリティを強化するために、電子メールドメインドメインを使用して次のこ許可リストとをおこなうことができます。

* Workfrontに保存されたレポートやドキュメントがWorkfront電子メールに含まれる場合の移動先を制御
* ユーザープロファイルでユーザーが指定できる電子メールアドレスに、制御電子メールドメインを含めることができます

例えば、アットリスクを伴う顧客を一覧表示するレポートなど、機密データを保護する場合は、E メールドメインに社内 E メールドメインまたはドメインのみを含めることができ許可リストます。 この方法では、ユーザーは、そのレポート ( またはその他のWorkfrontレポート ) を外部の電子メールアドレスに送信できません。

詳しくは、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) 記事内 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## サブグループのグループ管理者を割り当てる

組織のレベルが個別に操作しやすくなるように、グループ管理者をサブグループに割り当てる機能を追加しました。 これで、適切な担当者にサブグループ管理を委任していることを確認できます。

以前は、最上位グループのみがグループ管理者を持つことができ、その管理者は最上位グループの下にあるすべてのサブグループを管理していました。

詳しくは、 [サブグループのグループ管理者](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) 記事内 [サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

この機能は、 [新しいWorkfrontエクスペリエンスの管理者の基本事項、パート 1:ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One の学習パス

## グループのイベント通知の設定

>[!NOTE]
>
>段階的なロールアウトの一部として使用できるのは、グループのプロジェクト環境設定をロック解除できる顧客のみです。 これには、クラスタ 4 および 6 のすべてのお客様と、他のクラスタの少数のお客様が含まれます。 このメモは、機能がより多くのクラスターで使用可能になったときに更新されます。

Workfrontの管理者は、最上位のグループに対するイベント通知を設定できるようになり、グループ管理者にさらに自律性を与えることができるようになりました。 サブグループは、最上位の親グループからイベント通知設定を継承します。

以前は、Workfrontの管理者がシステムレベルでのみイベント通知を設定できていました。つまり、すべてのグループが同じイベント通知のセットを使用する必要がありました。

詳しくは、次の記事を参照してください。

* [すべてのグループのイベント通知の設定をロック解除またはロックします](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [グループのイベント通知を表示および設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

この機能は、 [新しいWorkfrontエクスペリエンスの管理者の基本事項、パート 1:ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One の学習パス

この機能は、 [新しいWorkfrontエクスペリエンスでの電子メールおよびアプリ内通知](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) Workfront One の学習パス

## 「グループ」領域でのグループプロジェクトと承認プロセスの操作

グループ管理者は、グループのプロジェクトや承認プロセスが「グループ」領域に一覧表示されるので、簡単にグループのプロジェクトや承認プロセスを表示および操作できます。 グループのメインページから、次の操作を実行できます。

* 左側のメニューの「プロジェクト」をクリックして、グループのプロジェクトを表示し、グループ用の新しいプロジェクトを作成します。 選択したプロジェクトが共有されている場合は、ツールバーのボタンを使用して、編集、エクスポート、コピー、削除できます。

   詳しくは、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* 左側のメニューの「承認」をクリックして、グループに関連付けられているすべての承認プロセスを表示および管理します。

   詳しくは、 [グループレベルの承認プロセス](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

この機能は、Workfront管理者も使用できます。

## グループ内で使用および割り当てられたライセンス数の表示

ライセンスの配布状況を判断するために、1 つのグループとその下のサブグループで使用されているライセンスの数を表示できます。

最上位グループを管理する場合は、グループで使用されるライセンスの数（およびそのサブグループ）と、グループに割り当てられるライセンスの最大数の両方を表示できます。

詳しくは、 [新しいAdobe Workfrontエクスペリエンスで、グループに割り当てられ、使用されたライセンス数を表示します](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

