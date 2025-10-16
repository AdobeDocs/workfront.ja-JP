---
title: レイアウトテンプレートへのユーザーの割り当て
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Adobe Workfront の管理者は、作成したレイアウトテンプレートを、使用する必要のある任意のユーザー、担当業務、チームまたはグループに割り当てることができます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 91%

---

# レイアウトテンプレートにユーザーを割り当て

作成したレイアウトテンプレートを、使用する必要のある任意のユーザー、担当業務、チーム、またはグループに割り当てることができます。

レイアウトテンプレートが割り当てられていないユーザーの場合は、デフォルトのレイアウトが使用されます。デフォルトのレイアウトについては、[デフォルトの Adobe Workfront レイアウトについて](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)を参照してください。

「レイアウトテンプレートを使用した自分のワークとワーク要求の変更」の説明に従って、レイアウトテンプレートを自分自身に割り当てることもできます。

同じ名前に複数の異なるレイアウトテンプレートを割り当てることができます。ユーザー、役割、グループ、チームに対して有効なレイアウトテンプレートについて詳しくは、この記事内で後ほど説明する[レイアウトテンプレートの割り当て優先度](#layout-template-assignment-priority)を参照してください。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレート](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

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
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーへのレイアウトテンプレートの割り当て

1. [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)に説明されているとおり、レイアウトテンプレートの使用を開始します。

   >[!TIP]
   >
   >レイアウトテンプレートに問題がなければ、[&#x200B; 新しいレイアウトテンプレートのテスト &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md) の説明に従ってテストすることをお勧めします。

1. ページの上位のセクションで「**割り当て先:**」をクリックします。
1. 表示されるボックスで、「**ユーザー、担当業務、チーム、またはグループを追加する**」をクリックし、ユーザー、担当業務、チームまたはグループの名前の入力を開始し、ドロップダウンに表示されたら名前をクリックします。

   最近追加された名前には、青色の背景が表示されます。これは、追加したばかりの名前とリストに既に存在する名前を区別できるため、既存のレイアウトテンプレートを編集する際に役立ちます。

   情報アイコン ![&#x200B; 情報アイコン &#x200B;](assets/info-icon.png) は、別のレイアウトテンプレートに既に割り当てられているユーザー、担当業務、チーム、グループの名前の右側に表示されます。 アイコンの上にポインタを合わせると、そのレイアウトテンプレートの名前が表示され、既存の割り当てを上書きするかどうかを決定できます。

1. 前の 2 つの手順を繰り返し、必要に応じて、レイアウトテンプレートを他のユーザー、担当業務、チームまたはグループに割り当てます。

   一度に 100 までのユーザーを割り当てることができます。

1. 「**完了**」、次に左下隅の「**保存**」の順にクリックします。

   この手順では、レイアウトテンプレートの作成と割り当てのプロセスを完了します。

## レイアウトテンプレートの割り当て優先度 {#layout-template-assignment-priority}

ユーザーと他の Workfront 管理者は、次の 4 つの方法で、同じユーザーに複数の異なるレイアウトテンプレートを割り当てることができます。

* 個々のユーザーに対して
* ユーザーが持つ特定の担当業務に対して
* ユーザーが属している特定のチームに対して
* ユーザーが属している特定のグループに対して

ただし、ユーザーには、一度に 1 つのレイアウトテンプレートのみが表示されます。表示されるテンプレートは、次の優先度階層によって決まります。

* **個々のユーザー**：個々のユーザーとして個人に割り当てられたレイアウトテンプレートが、他のすべてを上書きします。新しい割り当てを行うことで、個々のユーザーに対して行われた以前の割り当てを上書きできます。最新の割り当てが優先されます。
* **プライマリ担当業務**：ユーザーにレイアウトテンプレートが 1 人のユーザーとして割り当てられていない場合は、プライマリ担当業務に割り当てられたテンプレートが表示されます。

  ユーザーのプライマリ担当業務に割り当てられたレイアウトテンプレートのみが、ユーザーに対して表示されます。ユーザーが保持するセカンダリ担当業務に割り当てられたテンプレートは表示されません。

* **ホームチーム**：個人ユーザーとして、またはプライマリ担当業務を持つユーザーとして、レイアウトテンプレートが割り当てられていない場合は、ホームチームに割り当てられたテンプレートが表示されます。

  ユーザーのホームチームに割り当てられたテンプレートのみが、ユーザーに対して表示されます。ユーザーがメンバーである他のチームに割り当てられたテンプレートは表示されません。

* **ホームグループ**：レイアウトテンプレートが個人ユーザーとして、またはプライマリ担当業務を持つユーザーとして、またはホームチームのメンバーとして割り当てられていない場合は、自分のホームグループに割り当てられているテンプレートが表示されます。

  ユーザーのホームグループに割り当てられたテンプレートのみが、ユーザーに表示されます。他のグループに割り当てられたテンプレートは表示されません。

## レイアウトテンプレートに割り当てられた多数のユーザー

<!--If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
2,000 人を超えるユーザーをレイアウトテンプレートに割り当てる場合、次のいずれかを実行することをお勧めします。

* ユーザーをグループまたはチームに編成し、レイアウトテンプレートをそれらのグループまたはチームに割り当てます。詳しくは、[グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)および[チームの作成と管理](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md)を参照してください。

* ユーザーに担当業務を割り当て、レイアウトテンプレートをプライマリ担当業務に割り当てます。詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。
