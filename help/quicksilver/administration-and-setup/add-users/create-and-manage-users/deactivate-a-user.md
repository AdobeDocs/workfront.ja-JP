---
title: ユーザーのディアクティベートまたは再アクティベート
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront 管理者は、ユーザーを非アクティブ化または再アクティブ化できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 94%

---

# ユーザーの非アクティブ化または再アクティブ化

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

ユーザーが組織からいなくなった場合、そのユーザーを Adobe Workfront から削除する必要がある場合があります。更新に追加したり、作業を割り当てたりする際に、他のユーザーの混乱を引き起こす可能性があるため、組織を去ったユーザーをシステム内でアクティブなままにしておくべきではありません。ユーザーを非アクティブ化すると、他のユーザーがシステム内のユーザーを検索する際に、そのユーザーの名前が表示されなくなります。

管理者は、非アクティブなユーザーを設定エリアで確認できます。

ユーザーはいつでも再アクティブ化できます。

>[!IMPORTANT]
>
>組織を離れたユーザーは、削除するのではなく、非アクティブ化することをお勧めします。ユーザーを削除すると、そのユーザーに関連付けられた Workfront 内のすべての履歴が失われます。これには、作業割り当て、注釈、時間、ドキュメント、および一度作成したその他すべてのオブジェクトとの関連付けが含まれます。
>
>Workfront でユーザーを非アクティブ化すると、Workfront とデジタルプルーフの両方に対するユーザーのライセンスが削除されます。また、ユーザーに作業を割り当てることもできなくなります。ユーザーのアクティブ化を解除すると、そのユーザーの Workfront ライセンスおよびプルーフライセンスを他のユーザーが使用できるようになります。アクティブ化を解除したユーザーのプロファイルに含まれるその他の情報は、変更されません。
>
>削除による影響とユーザーの非アクティブ化の影響について詳しくは、[ユーザーの削除](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p><p>または</p><p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>この 2 つのオプションのうち、ユーザー<b>管理者（グループユーザー）</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

Workfront 管理者、スタンダードライセンスユーザーやプランライセンスユーザーのアクティブ化を解除する前に、オブジェクトとアクティビティを別のユーザーに関連付ける必要があります。

詳しくは、[Workfront 管理者とプランライセンスのユーザーの非アクティブ化について](#about-deactivating-workfront-administrators-and-plan-license-users)を参照してください。

## ユーザーの非アクティブ化

ユーザーをディアクティベートする際は、次の点に注意してください。

* ユーザーはシステムにアクセスできません。
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* ユーザーに関連付けられたすべてのデータは保持されます。
* 非アクティブ化されたユーザーのライセンスを別のユーザーに割り当てることができます。

ユーザーをディアクティベートするには：

{{step-1-to-users}}

1. ユーザーを選択し、**その他**&#x200B;アイコン ![](assets/more-icon.png) をクリックし、更に「**非アクティブ化**」をクリックします。

1. 表示されるボックスで「**非アクティブ化**」をクリックします。

## ユーザーの非アクティブ化をスケジュール

管理者は、ユーザーが実際に組織を離れる前に、ユーザーにアクティブ化解除のマークを付けることをお勧めします。例えば、契約期間が限定されているユーザーと業務を行っている場合、そのユーザーは限られた期間システム内に存在し、その終了日を把握しています。そのユーザーを終了日に非アクティブ化するようにスケジュール設定できます。

Workfront 管理者とプランライセンスユーザーは、ユーザープロファイルに非アクティブ化の日付を表示できます。

ユーザーの非アクティブ化をスケジュールするには、次の手順に従います。

{{step-1-to-users}}

1. ユーザー名を選択します。

   または

   （オプション）複数のユーザーを選択して、一括で非アクティブ化をスケジュールします。

1. 編集アイコン ![](assets/edit-icon.png) をクリックします。
1. 表示されるユーザーを編集ボックスで、「**リソース計画**」をクリックしてそのエリアに移動します。
1. 「**非アクティブ化をスケジュール**」オプションを有効にします。

1. 表示されるカレンダーで、**スケジュールされたアクティブ化解除日**&#x200B;の日付と時刻を指定します。

   >[!NOTE]
   >
   >* 時間ボックスでは、分単位ではなく、時間単位のみを選択できます。
   >* 現在の日の過ぎた時間を選択した場合、Workfront では翌日の午前 12 時にアクティブ化解除がスケジュールされます。選択した時間は、アクティブ化解除をスケジュールしているユーザーのコンピュータータイムゾーンに一致します。

1. 「**変更を保存**」をクリックします。

   ユーザーは、選択した日の選択した時刻以降にアクティブ化が解除されます。複数のユーザーに対して一括でアクティブ化を解除することを選択した場合、選択したすべてのユーザーは、選択した日の選択した時刻以降にアクティブ化が解除されます。

非アクティブ化が予定されているユーザーのレポートを作成し、どのユーザーが非アクティブ化されるかを常に把握することをお勧めします。ユーザーのアクティブ化が解除された後は、アクティブ化の解除が行われたかどうかは確認されません。

## ユーザーを再度アクティブ化

{{step-1-to-users}}

1. ユーザーを選択し、その他アイコン ![](assets/more-icon.png)、**アクティブ化**&#x200B;の順にクリックします。

1. ドロップダウンメニューで新しい&#x200B;**アクセスレベル**&#x200B;を割り当て、「**再アクティブ化**」をクリックします。
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### ユーザーを再度アクティブ化した際のプルーフへの影響

非アクティブ化されたユーザーは、割り当てられていたデフォルトのプルーフ役割とプルーフライセンスを失います（Workfront Premium レガシープランを使用している場合）。ユーザーを再度アクティブ化する場合は、次の操作を行う必要があります。

* ライセンスを再度割り当てます（Workfront Premium レガシープランを使用している場合）。Workfront のプルーフプランについて詳しくは、[Workfront のプルーフ機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)を参照してください。
* 正しいプルーフの役割を持っていることを確認してください。再アクティブ化されたプルーフユーザーには、新規ユーザーのデフォルトのプルーフの役割として指定されたものが割り当てられます。詳しくは、[デフォルトのプルーフの役割を設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)を参照してください。

## Workfront 管理者、スタンダードライセンスのユーザー、プランライセンスのユーザーの非アクティブ化について

Workfront 管理者またはプランライセンスを持つユーザーを非アクティブ化する前に、そのユーザーに関係する Workfront オブジェクトとアクティビティを確認し、必要に応じてそれらを別の Workfront 管理者またはプランライセンスユーザーに関連付けることが重要です。

これらのオブジェクトとアクティビティには以下が含まれる場合があります。

* ユーザーに割り当てられたタスクまたはイシュー
* ユーザーが所有するプロジェクト
* ユーザーのアクセス権で実行するように設定されたレポート
* ユーザーが所有するテンプレート
* ユーザーがリソースマネージャーとして設定されたプロジェクトとテンプレート
* Workfront 管理者またはプランライセンスユーザーがデフォルトの担当者であるリクエストキュールーティングルール
* ユーザーを含むステージを持つ承認プロセス（特に、ステージで唯一の承認者であった場合）
* ユーザーを承認者として一覧表示するタイムシート
* ユーザーを承認者として一覧表示するタイムシートプロファイル
* ユーザーを含む自動化されたワークフローのプルーフ

## ユーザーの非アクティブ化をスケジュールする際のリソース計画への影響

ユーザーを非アクティブ化するようにスケジュールすると、そのユーザーは、予算編成時間に使用できるとしてリソースプランナーに表示されなくなります。これらのユーザーが引き続きリソースプールに含まれている場合、リソースプランナーに表示されますが、その空き時間は、スケジュールされた非アクティブ化の日付から 0 時間に設定されます。

リソースプランナーは、ユーザーのすべての職務とタスクの完了予定日を考慮し、それに応じてリソースを計算します。

リソースプランナーの詳細は、[リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。
