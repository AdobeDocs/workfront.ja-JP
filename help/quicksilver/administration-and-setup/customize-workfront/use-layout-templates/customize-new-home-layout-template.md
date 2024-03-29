---
title: レイアウトテンプレートを使用して新しいホームをカスタマイズする
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートを使用して、新しいホームを開いたときにユーザーに表示する内容を設定できます。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: fcf4ff8525e3ac65aa75ab01463a3641e7898169
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 24%

---

# レイアウトテンプレートを使用して新しいホームをカスタマイズする

レイアウトテンプレートを使用して、新しいホームを開いたときにユーザーに表示する内容を設定できます。

以下を設定できます。

* デフォルトでワークスペースに表示されるウィジェットと、ページ上のレイアウト
* どの背景が選択されているか
* 特定のウィジェット設定（マイプロジェクト、マイタスク、マイタスク、マイイシューウィジェットで使用可能なフィルターとグループ、そのデフォルトなど）

>[!IMPORTANT]
>
>このページで説明する管理者レイアウトテンプレートの選択は、個々のユーザのカスタマイズ選択を上書きします。
>
>レイアウトテンプレートに対する変更を保存すると、そのレイアウトテンプレートのユーザーは、レイアウトテンプレートに合わせて新しいホームページを変更し、既存のウィジェットの選択をページの下部にプッシュします。 管理者が選択したウィジェットは、ユーザーによって再配置およびサイズ変更される場合がありますが、削除することはできません。

新しいホームについて詳しくは、 [新しいホームを使い始める](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## レイアウトテンプレートを使用して新しいホームをカスタマイズする

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。

1. 下向き矢印をクリックします。 ![](assets/dropdown-arrow.png) under **ユーザーに表示する内容をカスタマイズする**&#x200B;を選択し、次に **ホームワークスペース**.

1. 右側に表示されるタブで、 **デザインとレイアウト** ウィジェットと背景を選択して配置する、または **ウィジェット設定** を使用して、使用可能なフィルターやグループなどの個々のウィジェットの設定を管理します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">デザインとレイアウト</td> 
      <td>
      <p>ユーザーのワークスペースに表示するウィジェットとその位置を選択し、背景を選択します。 ユーザーは選択したウィジェットを削除できませんが、自由にウィジェットを移動およびサイズ変更したり、追加のウィジェットを追加したりできます。</p>
      <p>このタブは、基本的に、小さな新しいホームワークスペースとして機能します。そのため、 <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">新しいホームでウィジェットを追加、編集、または削除する</a>. ウィジェットを選択し、ユーザーに表示するようにワークスペースを配置します。</p>
      <p>背景を変更するには、以下の手順に従います。 <b>バックグラウンドのカスタマイズ</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">新しいホームを使い始める</a>.</p>
      <p>

>[!NOTE]
>
>レイアウトテンプレート内でのウィジェットの移動またはサイズ変更のみが、ユーザーの新しいホームページのトリガーを設定して、レイアウトを更新することはできません。 ただし、ウィジェットを追加または削除すると、トリガーのページの更新が行われます。

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ウィジェット設定</td> 
      <td>
      <p>個々のウィジェットの設定を変更します。 現在、サポートされているウィジェットは 3 つだけです。</p>
      <ul>
        <li>マイプロジェクト</li>
        <li>マイタスク</li>
        <li>マイ問題</li>
      </ul>
      <p>編集するウィジェットを選択すると、使用可能なオプションが右側に表示されます。 以下のオプションがあります。 <b>フィルター</b>, <b>列</b>、および <b>グループ</b>. 実行できる操作：</p>
      <ul>
      <li><p><b>ユーザーが使用できるフィルター、列またはグループを選択します。</b></p>
      <p>リスト内のすべてのオプションの横にあるチェックボックスをオンにします。 オフのオプションは、ユーザーには表示されません。</li></p>     
    <p>

>[!IMPORTANT]
>
>列の設定をウィジェットに正しく適用するには、ビューの作成アクセス権が必要です。

</p>
      <li><p><b>ウィジェットのデフォルトのフィルターまたはグループを設定します。</b></p>
      <p>オプションの上にマウスポインターを置くと、そのオプションをユーザーのデフォルトとして設定できるボタンが表示されます。 現在のデフォルトでは、右側に青いデフォルトバッジが表示されます。</li></p>
      <li><p><b>使用可能なオプションのリストに既存のフィルター、列、またはグループを追加します。</b></p>
      <p>各リストの下部にあるプラス記号ボタンをクリックして、そのリストにオプションを追加します。 この方法で追加できるのは、既存のフィルター、フィールド（列用）、グループのみです。</p></li>
      </ul>
      <p>

>[!NOTE]
>
>レイアウトテンプレートを使用して特定のウィジェットにデフォルトのフィルターまたはグループを設定した場合、既存のユーザー設定が原因で、すぐに有効にならない場合があります。 新しいフィルターまたはグループ化を直ちに適用するには、ユーザーまたはユーザーが、URL の末尾に「/resetUser」を付けて、ユーザーの環境設定をリセットする必要がある場合があります。

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、 **保存** をクリックします。
