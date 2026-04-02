---
title: ユーザーの非アクティブ化または再アクティブ化
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront管理者は、ユーザーをディアクティベートまたは再アクティベートできます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 56%

---

# ユーザーの非アクティブ化または再アクティブ化 {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="ユーザーの非アクティブ化"
>abstract="ユーザーを非アクティブ化すると、そのユーザーは Workfront および Frame.io から削除されます。非アクティブ化したユーザーは、後で再アクティブ化できます。"

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

ユーザーが組織を離脱した場合は、他のユーザーが更新に追加したり作業を割り当てたりする際に混乱が生じないように、システムでユーザーを非アクティブにすることをお勧めします。 ユーザーを非アクティブ化すると、他のユーザーがシステム内のユーザーを検索する際に、そのユーザーの名前が表示されなくなります。

管理者は、非アクティブなユーザーを設定エリアで確認できます。

ユーザーはいつでも再アクティブ化できます。

>[!IMPORTANT]
>
>* 組織を離れたユーザーは、削除するのではなく、非アクティブ化することをお勧めします。ユーザーを削除すると、そのユーザーに関連付けられた Workfront 内のすべての履歴が失われます。これには、作業割り当て、注釈、時間、ドキュメント、および一度作成したその他すべてのオブジェクトとの関連付けが含まれます。
>
>* Workfront でユーザーを非アクティブ化すると、Workfront とデジタルプルーフの両方に対するユーザーのライセンスが削除されます。また、ユーザーに作業を割り当てることもできなくなります。ユーザーのアクティブ化を解除すると、そのユーザーの Workfront ライセンスおよびプルーフライセンスを他のユーザーが使用できるようになります。アクティブ化を解除したユーザーのプロファイルに含まれるその他の情報は、変更されません。
>
>* Workfrontでユーザーを非アクティブ化しても、Adobe Admin ConsoleのWorkfront製品プロファイルからユーザーが削除されることはありません。 詳しくは、[&#x200B; ユーザーの削除](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)を参照してください。
>
>* ユーザーがAdmin Console ユーザーグループに属しており、そのユーザーグループの1つ以上に製品プロファイルが追加されている場合、Workfrontからユーザーを非アクティブ化しても、実際には製品から削除されません。 Admin Consoleのユーザーグループからユーザーを削除する必要があります。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これらの2つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

Workfront 管理者、スタンダードライセンスユーザーやプランライセンスユーザーのアクティブ化を解除する前に、オブジェクトとアクティビティを別のユーザーに関連付ける必要があります。

詳しくは、この記事の「[Workfront管理者と標準またはプランのライセンスユーザーの非アクティブ化について](#about-deactivating-workfront-administrators-and-plan-license-users)」を参照してください。

## ユーザーの非アクティブ化

ユーザーを非アクティブ化する場合は、次の点に注意してください。

* ユーザーはシステムにアクセスできません。
<!--
* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.
   -->
* ユーザーに関連付けられたすべてのデータが保持されます。
* 非アクティブ化されたユーザーのライセンスを別のユーザーに割り当てることができます。

ユーザーを非アクティブ化するには：

{{step-1-to-users}}

1. ユーザーリストでユーザーを選択します。
1. **詳細** アイコン ![詳細アイコン &#x200B;](assets/more-icon.png)をクリックし、**非アクティブ化**&#x200B;をクリックします。

1. **ユーザーを非アクティブ化** ダイアログボックスで、**非アクティブ化**&#x200B;をクリックします。

## ユーザーの非アクティブ化をスケジュール

管理者は、ユーザーが実際に組織を離れる前に、ユーザーにアクティブ化解除のマークを付けることをお勧めします。例えば、契約上の制約があるユーザーを使用している場合、そのユーザーは期間限定でシステム内に存在し、その終了日を把握できます。 そのユーザーを終了日に非アクティブ化するようにスケジュール設定できます。

Workfront 管理者とプランライセンスユーザーは、ユーザープロファイルに非アクティブ化の日付を表示できます。

ユーザーの非アクティブ化をスケジュールするには、次の手順に従います。

{{step-1-to-users}}

1. ユーザーリストでユーザーを選択します。

   または

   （オプション）複数のユーザーを選択して、一括で非アクティブ化をスケジュールします。

1. **編集** アイコン ![編集アイコン &#x200B;](assets/edit-icon.png)をクリックします。
1. **ユーザーの編集** ボックスの左側のパネルで、**リソース計画**&#x200B;をクリックします。
1. 「**アクティベーション解除日を設定**」をクリックします。

1. **非アクティブ化日**&#x200B;の日付と時刻を選択します。

   >[!NOTE]
   >
   >* 時間ボックスでは、分単位ではなく、時間単位のみを選択できます。
   >* 過ぎた現在の日の時間を選択すると、Workfrontは翌日午前12:00時にアクティベーション解除をスケジュールします。
   >* 選択した時間は、アクティブ化解除をスケジュールしているユーザーのコンピュータータイムゾーンに一致します。

1. 「**保存**」をクリックします。

ユーザーは、選択した日の選択した時刻以降にアクティブ化が解除されます。複数のユーザーに対して一括でアクティブ化を解除することを選択した場合、選択したすべてのユーザーは、選択した日の選択した時刻以降にアクティブ化が解除されます。

無効化が予定されているユーザーに関するレポートを作成して、無効化されるユーザーに関する情報を保持することをお勧めします。 ユーザーが非アクティブ化された後に非アクティブ化が行われたことを確認する情報はありません。

## ユーザーを再度アクティブ化

{{step-1-to-users}}

1. ユーザーを選択し、**詳細** アイコン ![詳細アイコン &#x200B;](assets/more-icon.png)をクリックしてから、**アクティブ化**&#x200B;をクリックします。

1. **ユーザーを再アクティブ化** ダイアログで、ドロップダウンメニューで新しい&#x200B;**アクセスレベル**&#x200B;を選択し、**再アクティブ化**&#x200B;をクリックします。
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration.
-->

### ユーザーを再度アクティブ化した際のプルーフへの影響

非アクティブ化されたユーザーは、割り当てられていたデフォルトのプルーフ役割とプルーフライセンスを失います（Workfront Premium レガシープランを使用している場合）。ユーザーを再度アクティブ化する場合は、次の操作を行う必要があります。

* ライセンスを再度割り当てます（Workfront Premium レガシープランを使用している場合）。Workfront のプルーフプランについて詳しくは、[Workfront のプルーフ機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)を参照してください。
* 正しいプルーフの役割を持っていることを確認してください。再アクティブ化されたプルーフユーザーには、新規ユーザーのデフォルトのプルーフの役割として指定されたものが割り当てられます。詳しくは、[デフォルトのプルーフの役割を設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)を参照してください。

## Workfront 管理者、スタンダードライセンスのユーザー、プランライセンスのユーザーの非アクティブ化について

Workfront 管理者またはプランライセンスを持つユーザーを非アクティブ化する前に、そのユーザーに関係する Workfront オブジェクトとアクティビティを確認し、必要に応じてそれらを別の Workfront 管理者またはプランライセンスユーザーに関連付けることが重要です。

これらのオブジェクトとアクティビティには以下が含まれる場合があります。

* ユーザーに割り当てられたタスクまたは問題。
* ユーザーが所有するプロジェクト。
* ユーザーのアクセス権で実行するように設定されたレポート。
* ユーザーが所有するテンプレート。
* ユーザーがリソースマネージャーとして設定されたプロジェクトとテンプレート。
* リクエストキューのルーティングルールは、Workfront管理者またはプランライセンスユーザーがデフォルトの担当者です。
* ユーザーを含むステージを持つ承認プロセス（特に、ステージで唯一の承認者である場合）。
* 承認者としてユーザーをリストするタイムシート。
* ユーザーを承認者としてリストするタイムシート プロファイル。
* ユーザーを含む自動ワークフローの校正。

## ユーザーの非アクティブ化をスケジュールする際のリソース計画への影響

ユーザーを非アクティブ化するようにスケジュールすると、そのユーザーは、予算編成時間に使用できるとしてリソースプランナーに表示されなくなります。これらのユーザーが引き続きリソースプールに含まれている場合、リソースプランナーに表示されますが、その空き時間は、スケジュールされた非アクティブ化の日付から 0 時間に設定されます。

リソースプランナーは、ユーザーのすべての職務とタスクの完了予定日を考慮し、それに応じてリソースを計算します。

リソースプランナーの詳細は、[リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

