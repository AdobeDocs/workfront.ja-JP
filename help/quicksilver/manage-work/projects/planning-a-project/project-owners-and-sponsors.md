---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: プロジェクト所有者とスポンサーの概要
description: プロジェクト所有者とプロジェクトスポンサーを指定できます。
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# プロジェクト所有者とスポンサーの概要

プロジェクト所有者とプロジェクトスポンサーを指定できます。

プロジェクト所有者は、時間と予算に基づいてプロジェクトを完了する個人です。

プロジェクトスポンサーは、プロジェクトに投資するリソースを持つプロジェクトの重要な関係者です。 通常、このプロジェクトの完了は、プロジェクトスポンサーに恩恵を与えます。

プロジェクト所有者またはプロジェクトスポンサーを更新する方法については、 [プロジェクトの所有者とスポンサーの更新](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## プロジェクト所有者

プロジェクトまたはテンプレートに対してプロジェクト所有者を指定することで、プロジェクトの管理者を指定できます。

1 つのプロジェクトに対して定義できるプロジェクト所有者は 1 つだけです。

「プロジェクト所有者」フィールドを使用して、次の操作を実行できます。

* 1 人のユーザーのみをプロジェクト所有者として指定できます。
* プロジェクトの承認者として、プロジェクトの所有者を指定できます。
* プロジェクト、タスク、または問題の承認プロセスを定義する際に、プロジェクト所有者を汎用承認者として指定できます。 承認について詳しくは、 [承認プロセスの編集](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >プロジェクト所有者に承認を割り当てて、誰もプロジェクトの所有者に指定されていない場合、「セットアップ」領域の「顧客情報」セクションで示されたように、承認はメインのWorkfront管理者に再割り当てされます。 詳しくは、 [システムの基本情報を設定する](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* プロジェクト所有者にのみ配信される特定の通知を有効にすることができます。

   電子メール通知について詳しくは、 [システムの全員に対するイベント通知を設定する](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) 記事内 [システムの全員に対するイベント通知を設定する](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* レポートまたはリストに「プロジェクト所有者」フィールドを表示できます。

   また、ビュー、グループ化、プロンプトに [ プロジェクト所有者 ] フィールドを表示することもできます。

   例えば、次のテキストモード式をフィルターにコピーして、ログインしたユーザーが所有するプロジェクトを表示できます。 

   ```
   ownerID=$$USER.ID
   ```

レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## プロジェクトスポンサー

システム内の任意のユーザーをプロジェクトスポンサーとして指定できます。 プロジェクトスポンサーは、通常、プロジェクトで何が起きているかを知る必要があるマネージャー、エグゼクティブまたは関係者です。

プロジェクトスポンサーを割り当てる際は、次の点を考慮してください。

* プロジェクトスポンサーは、プロジェクトへの追加のアクセス権を取得しませんが、プロジェクトの電子メール通知に追加されます。 通知について詳しくは、 [システムの全員に対するイベント通知を設定する](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 指定できるプロジェクトスポンサーは 1 つだけです。
* プロジェクト、タスク、または問題の承認プロセスを定義する際に、プロジェクトスポンサーを一般的な承認者として指定できます。 承認について詳しくは、 [承認プロセスの編集](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >プロジェクトスポンサーに承認を割り当て、誰もプロジェクトのスポンサーとして指定されていない場合、承認はプロジェクト所有者に再割り当てされます。 プロジェクトの所有者が指定されていない場合、承認はWorkfront管理者に割り当てられます。

* 「プロジェクトスポンサー」フィールドをレポートまたはリストに表示できます。

   「プロジェクトスポンサー」フィールドを表示、グループ化またはプロンプトで表示することもできます。

   例えば、次のテキストモードの式をフィルターにコピーして、ログインしたユーザーがスポンサーとするプロジェクトを表示できます。

   ```
   sponsorID=$$USER.ID
   ```

    

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
