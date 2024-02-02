---
content-type: release-notes
keywords: メモ、四半期、更新
navigation-topic: product-releases
title: 21.1 管理者の機能強化
description: このページでは、プレビュー環境の 21.1 リリースで行われた管理者向けの機能強化について説明します。これらの機能強化は、2021年2月15日（PT）の週に実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: ht
source-wordcount: '1393'
ht-degree: 100%

---

# 21.1 管理者の機能強化

このページでは、プレビュー環境の 21.1 リリースで行われた管理者向けの機能強化について説明します。これらの機能強化は、2021年2月15日（PT）の週に実稼動環境で利用可能になる予定です。

21.1 リリースで使用可能なすべての変更点の一覧については、[21.1 リリースの概要](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)を参照してください。

## プロジェクトをコピーするための新しいアクセスレベル設定を導入しました。

システム管理者は、プロジェクトでプランナーが実行できる操作をより詳細に制御できるように、新しい設定を導入して、プロジェクトのコピー機能を有効または無効にすることで、アクセスレベルのプロジェクトへの編集アクセスをより詳細にしました。この変更以前は、ユーザーのプロジェクト編集へのアクセスを有効にした場合、ユーザーは自動的にそれらのプロジェクトをコピーするためのアクセス権を付与されました。新しい機能を使用すると、新しいコピー設定を無効にして、プロジェクトをコピーするアクセス権なしで、他のユーザーに編集プロジェクトへのアクセス権を付与できるようになります。

この変更以前に、ユーザーがアクセスレベルでプロジェクトを編集にアクセスできた場合、この機能のリリース時に、この設定が自動的に有効になります。

計画のアクセスレベルについて詳しくは、[プロジェクトへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

プロジェクトのコピーについて詳しくは、[プロジェクトをコピー](../../../manage-work/projects/manage-projects/copy-project.md)を参照してください。

この機能は、[新しい Workfront エクスペリエンスの管理者の基本、パート 1：ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY)に含まれています。

## オブジェクトのカスタムフォームで、複数選択ドロップダウンフィールドのすべての項目を選択します。

>[!NOTE]
>
>この機能は、現在、新しいリクエストを送信する際には使用できません。

オブジェクトの詳細ページで、カスタムフォームの複数選択ドロップダウンフィールドに入力する際に、使用可能なすべてのオプションを選択する必要がある場合は、「すべてを選択」をクリックします。

カスタムフォーム上のデータの編集について詳しくは、[カスタムフォームフィールドの情報を編集](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)を参照してください。

## オブジェクトのすべてのカスタムフォームフィールドを再計算

オブジェクトの計算カスタムフィールドのすべてのデータを最新の状態に保つのが容易になりました。新しい式を再計算メニューオプションを使用すると、これらのフィールド内のすべてのデータをすばやく再計算できます。

これは、オブジェクト内の計算カスタムフィールドで参照される別のオブジェクト内のデータを編集した後に特に便利です。

以前は、計算されたカスタムフィールド内のすべてのデータが最新であることを確認するために、回避策を使用する必要がありました。例えば、オブジェクトを他のオブジェクトと共に編集し、一括編集が可能な再計算オプションを使用しました。

詳しくは、[カスタムフォームフィールドの情報を編集](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)を参照してください。

## グループ管理者のタスクとイシューの環境設定のロックを解除

>[!NOTE]
>
>2021年6月24日（PT）までは、段階的なロールアウトの一環として、グループのプロジェクト設定をロック解除できるお客様のみが使用できました。現在は、すべてのお客様が利用できます。

Adobe Workfront の管理者は、個々のタスクとイシューの環境設定をロック解除することで、グループ管理者にさらに自律性を与えることができるようになりました。グループ管理者は、環境設定のロックが解除されると、各グループの一意なニーズと内部プロセスに対応するように、グループ用に環境設定を構成できます。

詳しくは、[グループのタスクとイシューの環境設定を行う](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスの管理者の基本、第 2 部：プロジェクトの設定](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY)に含まれています。

## ポートフォリオとプログラムのアクセスレベルを個別に設定する

ポートフォリオとプログラムのアクセスレベルを個別に設定できるので、ポートフォリオとプログラムへのユーザーアクセスを管理しやすくなりました。

以前は、ポートフォリオとプログラムのアクセスレベル設定を組み合わせていました。つまり、ポートフォリオの場合と同じ方法でプログラムのアクセス設定を構成しないと、その逆も同様に設定できませんでした。

アクセスレベルの設定について詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

プログラムおよびポートフォリオ用に設定できるアクセス設定について詳しくは、[各オブジェクトタイプの機能への設定可能なアクセス](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)を参照してください。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスにおける管理者の基礎、パート 1：ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY)に含まれるようになりました。

## カスタムフォームで情報を編集する際に、一連のすべてのチェックボックスをオンにする

>[!NOTE]
>
>この機能は、現在、新しいリクエストを送信する際には使用できません。

オブジェクトの詳細ページで、カスタムフォームの複数選択ドロップダウンフィールドに入力する際に、使用可能なすべてのオプションを選択する必要がある場合は、「すべてを選択」をクリックします。

このオプションは、フィールドにチェックボックスが 3 つ以上含まれている場合にのみ表示されます。

詳しくは、[カスタムフォームフィールドの情報を編集する](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)を参照してください。

## Workfront メール許可リストの設定

データのセキュリティを強化するために、メールドメインの許可リストを使用して以下を実行できます。

* Workfront に保存されたレポートやドキュメントが Workfront メールに含まれる場合、メールの送信先を制御する
* メールアドレスに含めることができるメールドメインを制御する（ユーザープロファイルでユーザーが指定できます）

例えば、メールの許可リストに社内のメールドメインのみを含めると、リスクのある顧客をリストアップしたレポートなどの機密データを保護することができます。この場合、ユーザーは、そのレポートを（その他の Workfront レポートも）外部のメールアドレスに送信できません。

詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)の記事の[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur)の節を参照してください。

## サブグループのグループ管理者を割り当てる

組織の各レベルで独立して運用しやすくなるように、サブグループにグループ管理者を割り当てる機能を追加しました。これにより、サブグループの管理を適切な担当者に委任することができます。

以前は、トップレベルのグループにのみグループ管理者を置くことができ、その管理者がトップレベルのグループの下にあるすべてのサブグループを管理していました。

詳しくは、[サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)の記事の[サブグループのグループ管理者](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for)の節を参照してください。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスにおける管理者の基礎、パート 1：ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY)に含まれるようになりました。

## グループのイベント通知を設定

>[!NOTE]
>
>グループのプロジェクト環境設定のロックを解除できる顧客のみが、段階的なロールアウトの一部として使用できます。これには、クラスター 4 および 6 のすべてのお客様と、他のクラスターの少数のお客様が含まれます。このメモは、機能がより多くのクラスターで使用可能になり次第、更新されます。

Workfront 管理者は、トップレベルのグループに対するイベント通知を設定できるようになり、グループ管理者にさらに自律性を持たせることができるようになりました。サブグループは、トップレベルの親グループから通知設定を継承します。

以前は、Workfront 管理者がシステムレベルでしかイベント通知を設定できず、すべてのグループが同じ一連のイベント通知を使用する必要がありました。

詳しくは、次の記事を参照してください。

* [すべてのグループのイベント通知の設定をロックまたはロック解除](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [グループのイベント通知を表示および設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスにおける管理者の基礎、パート 1：ユーザー組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY)に含まれるようになりました。

この機能は、Workfront One の学習パス[新しい Workfront エクスペリエンスにおけるメール通知とアプリ内通知](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U)に含まれるようになりました。

## グループエリアでのグループプロジェクトと承認プロセスの操作

グループのプロジェクトや承認プロセスがグループエリアに一覧表示されるようになり、グループ管理者はそれらの表示と操作を簡単に行うことができます。グループのメインページから、次の操作を実行できます。

* 左側のメニューの「プロジェクト」をクリックすると、グループのプロジェクトを表示したり、新しく作成したりすることができます。選択したプロジェクトが共有されている場合は、ツールバーのボタンを使用して、編集、書き出し、コピー、削除を行うことができます。

  詳しくは、[グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

* 左側のメニューの「承認」をクリックすると、グループに関連付けられているすべての承認プロセスを表示したり、管理したりすることができます。

  詳しくは、[グループレベルの承認プロセス](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)を参照してください。

この機能は、Workfront 管理者も使用できます。

## グループ内で使用および割り当てられたライセンス数の表示

ライセンスの配布状況を判断するために、あるグループとその下のサブグループで使用されているライセンスの数を表示できます。

トップレベルのグループを管理している場合は、あるグループ（およびそのサブグループ）で使用されているライセンス数と、そのグループに割り当てられているライセンスの最大数の両方を表示できます。

詳しくは、[新しい Adobe Workfront エクスペリエンスで、グループに割り当てられ、使用されているライセンス数を表示](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)を参照してください。

