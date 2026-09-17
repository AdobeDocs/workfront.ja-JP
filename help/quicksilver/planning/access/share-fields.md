---
title: Workfront計画フィールドの共有
description: Workfront計画レコードのフィールドを他のユーザーと共有して、Adobe Workfront計画を使用する際にコラボレーションを確保できます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 4%
---

# Workfront計画フィールドの共有

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Workfront計画レコードのフィールドを他のユーザーと共有して、Adobe Workfront計画を使用する際にコラボレーションを確保できます。

フィールド共有を使用すると、ワークスペース管理者は個々のフィールドへのアクセスを制御できます。 レコードタイプの各フィールドには独自の共有ダイアログがあり、アクセスを「アクセスなし」、「フィールド値を表示」、「フィールド値を管理」に設定できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p> 
または
<p>スタンドアロンの製品パッケージとしてのWorkfront Planningは</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>フィールドの値を変更するためのフィールドへの権限を管理します</p>  
   <p>レコードタイプに対して権限を付与するか、それ以上の権限を付与して、フィールドに管理権限を継承します</p>  
   </td> 
  </tr>
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## フィールドの共有に関する考慮事項

* ユーザー、担当業務、グループ、チーム、会社とフィールドを共有できます。
* フィールドを共有できるのは、レコードタイプのテーブルビューのみです。
* 次の種類のフィールドは共有できません。

  * システムフィールド（作成者、レコード IDなど）
  * プライマリフィールド
  * ルックアップフィールド： ソースオブジェクトフィールドの権限は常に継承されます。
* フィールドへのアクセスは、次の設定を組み合わせることで可能になります。

  * **継承された権限**: デフォルトでは、フィールドは、レコードタイプに対して誰かが持っているのと同じアクセス権を継承します。 継承された権限をオフにして、ユーザーにレコードタイプよりも低いアクセス権を与えることができます。
  * ワークスペース内の&#x200B;**すべてのユーザーが表示できます**&#x200B;または&#x200B;**招待されたユーザーのみが**&#x200B;の選択にアクセスできます。 ワークスペースに対する権限を持つ全員にフィールドの表示を許可するか、個々のエンティティにのみ権限を与えることができます。

  同じユーザーに複数のルールが適用される場合、いずれかのルールから利用可能な最も高い権限が付与されます。

* レコードタイプの権限に応じて、ユーザーは次のフィールド権限を受け取ることができます。

  * 表示レコードタイプの権限は、フィールド値を表示するためのユーザー権限を与えます
  * レコードタイプのコントリビュートまたは管理の権限は、フィールド値を管理するためのユーザー権限を与えます

* ワークスペースの所有者とマネージャーのみがフィールド権限を調整できます。 Workspace管理者は、すべてのフィールドへの管理アクセス権を常に保持します。このアクセス権を下げることはできません。
* フィールド共有は、フィールド設定ではなく値へのアクセスを制御します。 フィールドの設定を変更できるのは、ワークスペースマネージャーのみです。
* フィールドの共有リストにユーザーを追加しても、ワークスペースまたはレコードタイプのアクセス権は付与されません。 そのアクセス権がない場合、警告アイコンは、権限がレコードタイプに追加された後にのみ有効であることを示します。
* 制限された権限を持つフィールドは、フィールドが表示されるすべての場所で適用されます。 これには、すべてのビュー、レコードの詳細ページ、リクエストフォーム、接続およびルックアップフィールド、キャンバスダッシュボード、API、およびMCP ツールが含まれます。
* パブリックビューは、完全に表示され、アクセスできるユーザーには読み取り専用のままになります。
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* 制限されたフィールド値の変更は、レコードの履歴には記録されません。
* フィールドの権限の変更は、通知をトリガーしません。
* グローバルレコードタイプの場合、フィールド権限はすべてのセカンダリワークスペースに適用され、ローカルで調整することはできません。

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## フィールドの共有

ワークスペースマネージャーは、個々のフィールドに対する権限を調整できます。

{{step1-to-planning}}

1. ワークスペースを開き、フィールドを共有するレコードタイプを開きます。

1. テーブル表示で、フィールドの列ヘッダーの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**フィールドを共有**&#x200B;をクリックします。

   **共有** ボックスが開きます。

1. （オプション） **アクセス権を付与**&#x200B;領域で、**ワークスペース内のすべてのユーザーが表示できる** オプションがデフォルトで選択されています。 ワークスペースおよびレコードタイプに対する&#x200B;**ビュー**&#x200B;以上の権限を持つユーザーはすべて、フィールドに対して同じ権限を持っています。

1. （オプション）「**から権限を継承」オプションの下にあるユーザーのアバターをクリックして、ワークスペースから権限を継承するユーザー、チーム、グループ、企業、またはジョブロールを表示します。**

   継承された権限を展開すると、レコードタイプに対するユーザーの権限が表示されます。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。 ワークスペースとレコードタイプが共有されたときに関連付けられたエンティティの代わりに、チーム、グループ、会社、または担当業務のユーザーが一覧表示されます。

1. （オプションおよび条件付き）特定のエンティティとフィールドを共有し、レコードタイプに対して既に持っているフィールドとは異なるアクセス権を与える場合は、次の操作を行います。

   1. **継承した権限**&#x200B;から&#x200B;**オンにした** オプションの選択を解除します。 デフォルトで選択されています。

      オプションが&#x200B;**に変更され、オフになりました**。

      >[!TIP]
      >
      >Workspace マネージャーには、レコードタイプとフィールドに対する管理権限が引き続き付与されます。

   1. 「**アクセス権を付与**」ボックスに、ワークスペースまたはレコードタイプに対して付与する権限レベルとは異なる権限レベルを付与するユーザー、チーム、グループ、会社、またはジョブロールを追加します。

      ユーザーとフィールドを共有すると、そのユーザーの主な担当業務と電子メールもフィールドに表示されます。 ユーザーの電子メールを表示するには、アクセスレベルのUsers オブジェクトで「連絡先情報を表示」設定を有効にする必要があります。

   1. 次のいずれかの権限レベルを選択します。

      * フィールドの値を表示
      * フィールドの値を管理

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* ユーザーがレコードタイプに対してContribute以上を持っている場合、フィールドに対して少ない権限を付与することはできません。
      >
      >* ワークスペース内にないユーザーに権限を付与することはできません。 ワークスペースおよびレコードタイプに対する権限を持たないユーザーは、どのフィールドにもアクセスできません。 ワークスペースとレコードタイプに対する権限を取得すると、フィールドにアクセスできるようになります。

1. 「**保存**」をクリックします。

   これで、フィールドは他のユーザーと共有されました。

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## フィールドへの権限の削除

フィールドからユーザーの権限を削除できます。 ただし、少なくともワークスペースに対する表示権限とレコードタイプを保持し、少なくともフィールドに対する表示権限を付与します。

ワークスペース内のレコードタイプまたはフィールドに対する権限を付与しない場合は、ワークスペースからアクセス権を削除する必要があります。

継承された権限からユーザーを削除することはできません。

{{step1-to-planning}}

1. フィールドの共有を停止するワークスペースを開き、レコードタイプカードをクリックします。 レコードタイプページが開きます。
1. テーブル表示で、フィールドの列ヘッダーの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**フィールドを共有**&#x200B;をクリックします。

   **共有** ボックスが開きます。
1. 権限を削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、権限ドロップダウンメニューを名前右側に展開し、**削除**&#x200B;をクリックします。

1. 「**保存**」をクリックします。

   ユーザーには、フィールドに対する指定された権限がなくなりました。 ただし、レコードタイプとワークスペースに対する権限は、それらの権限から削除しない限り、引き続き保持されます。

   これらの権限を持たなくなったフィールドへのアクセスを削除されたユーザーに対する通知はありません。
