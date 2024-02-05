---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: プロジェクト所有者とスポンサーの概要
description: プロジェクトのプロジェクト所有者およびプロジェクトスポンサーを指定できます。
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 111c776af19fbc2982c14cc9d3b3778d37bc0be3
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 100%

---

# プロジェクト所有者とスポンサーの概要

<!-- Audited: 1/2024 -->

プロジェクトのプロジェクト所有者およびプロジェクトスポンサーを指定できます。

プロジェクト所有者は、予定通りおよび予算通りにプロジェクトを完了する担当者です。

プロジェクトスポンサーは、プロジェクトに投資するリソースを持つプロジェクトの重要な関係者です。通常、プロジェクトの完了は、プロジェクトスポンサーにメリットを与えます。

プロジェクトのプロジェクト所有者またはプロジェクトスポンサーを更新する方法について詳しくは、[プロジェクトの所有者とスポンサーの更新](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md)を参照してください。

## プロジェクト所有者

プロジェクトまたはテンプレートに対してプロジェクト所有者を指定することで、プロジェクトのマネージャーを指定できます。

1 つのプロジェクトに対して定義できるプロジェクト所有者は 1 人だけです。

「プロジェクト所有者」フィールドを使用して、次の操作を実行できます。

* 1 人のユーザーのみをプロジェクト所有者として指定できます。
* プロジェクトの時間数の承認者として、プロジェクト所有者を指定できます。
* プロジェクト、タスクまたはイシューの承認プロセスを定義する際に、プロジェクト所有者を一般的な承認者として指定できます。承認について詳しくは、[承認プロセスの編集](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)を参照してください。

  >[!IMPORTANT]
  >
  >プロジェクト所有者に承認を割り当て、誰もプロジェクトの所有者として指定されていない場合、設定エリアの「顧客情報」セクションで示されているように、承認はメインの Workfront 管理者に再割り当てされます。詳しくは、[システムの基本情報の設定](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。
  >


* プロジェクト所有者にのみ配信される特定の通知を有効にできます。

  メール通知について詳しくは、[システムの全員に対するイベント通知の設定](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)の記事の[システムの全員に対するイベント通知の設定](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify)の節を参照してください。

* レポートまたはリストに「プロジェクト所有者」フィールドを表示できます。

  また、ビュー、グループ化またはプロンプトで「プロジェクト所有者」フィールドを表示できます。

  例えば、次のテキストモード式をフィルターにコピーして、ログインしたユーザーが所有するプロジェクトを表示できます。

  ```
  ownerID=$$USER.ID
  ```

レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。

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

システム内の任意のユーザーをプロジェクトスポンサーとして指定できます。プロジェクトスポンサーは、通常、プロジェクトで何が起きているかを知る必要があるマネージャー、エグゼクティブまたは関係者です。

プロジェクトスポンサーを割り当てる際は、次の点を考慮してください。

* プロジェクトスポンサーは、プロジェクトに対して追加のアクセス権を取得することはありませんが、プロジェクトのメール通知に追加されます。通知について詳しくは、[システムの全員に対するイベント通知の設定](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)の記事を参照してください。

* 指定できるプロジェクトスポンサーは 1 人のみです。
* プロジェクト、タスクまたはイシューの承認プロセスを定義する際に、プロジェクトスポンサーを一般的な承認者として指定できます。承認について詳しくは、[承認プロセスの編集](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)を参照してください。

  >[!IMPORTANT]
  >
  >プロジェクトスポンサーに承認を割り当て、誰もプロジェクトのスポンサーとして指定されていない場合、承認はプロジェクト所有者に再割り当てされます。プロジェクトの所有者として誰も指定されていない場合、承認は Workfront 管理者に割り当てられます。

* レポートまたはリストに「プロジェクトスポンサー」フィールドを表示できます。

  ビュー、グループ化またはプロンプトで「プロジェクトスポンサー」フィールドを表示できます。

  例えば、次のテキストモードの式をフィルターにコピーして、ログインしたユーザーがスポンサーするプロジェクトを表示できます。

  ```
  sponsorID=$$USER.ID
  ```

   

  レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。

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
