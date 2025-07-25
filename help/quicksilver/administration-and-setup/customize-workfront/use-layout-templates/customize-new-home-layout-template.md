---
title: レイアウトテンプレートを使用したホームのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートを使用すると、Adobe Workfrontでホームを開いたときに表示される内容を設定できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 39%

---

# レイアウトテンプレートを使用したホームのカスタマイズ

レイアウトテンプレートを使用すると、ユーザーが最初にホームを開いたときに表示される内容を設定できます。

以下を設定できます。

* ワークスペースにデフォルトで表示されるウィジェット
* 背景の選択
* 特定のウィジェット設定（マイプロジェクト、マイタスク、マイタスク、マイイシューのウィジェットで使用できるフィルターとグループ、そのデフォルトなど）

>[!IMPORTANT]
>
>エンドユーザーは、レイアウトテンプレートの適用後に、ページ上で背景を変更したり、ウィジェットを並べ替えたりできます。 Workfront管理者が提供するウィジェットを削除することはできません。
> 
>管理者は、ユーザーに新しいウィジェットを追加できます。 ただし、エンドユーザーが既にウィジェットの順序や背景の選択をカスタマイズしている場合、それらの特定のカスタマイズは変更されません。

ホームについては、[ ホームの基本を学ぶ ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md) を参照してください。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td><p>新規：標準</p>
  <p> 現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レイアウトテンプレートを使用したホームのカスタマイズ

レイアウトテンプレートを使用してホームをカスタマイズするには：

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。

1. ![Customize what users see](assets/dropdown-arrow.png) の下の下向き矢印 **下向き矢印）をクリックし、** ホームWorkspace **をクリックし** す。

1. 右のタブで、次のいずれかをクリックします。

   * **デザインとレイアウト**：選択すると、ウィジェットと背景を選択して配置します
   * **ウィジェット設定**：使用可能なフィルターやグループなど、個々のウィジェットの設定を管理する場合に選択します。

   各タブの詳細は次の表のとおりです。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">デザインとレイアウト</td> 
      <td>
      <p>ユーザーのワークスペースに表示するウィジェットとその位置を選択し、背景を選択します。</p> 
      <p>ユーザーは選択したウィジェットを削除できませんが、ウィジェットを自由に移動およびサイズ変更できます。 ウィジェットをさらに追加することもできます。</p>
      <p>このタブは、基本的に、このレイアウトテンプレートを使用しているユーザーが体験する実際のホームワークスペースのプレビューとして機能します。</p> 
      <p> 次のいずれかの操作を行います。 </p>
      <ul><li><a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref"> ホームでのウィジェットの追加、編集、削除 </a> で説明されている手順に従って、このタブをカスタマイズします。 </li>
      <li>ウィジェットを選択し、ユーザーに対して表示するようにワークスペースを配置します。</li>
      <li>背景を変更するには、<b> ホームの概要 </b> の <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref"> 背景のカスタマイズ </a> の手順に従います。</li></p>
      <p>

   >[!NOTE]
   >
   >レイアウトテンプレート内のウィジェットを移動またはサイズ変更しても、ユーザーのホームページにはレイアウトの更新がトリガーされません。 ただし、ウィジェットを追加または削除すると、ユーザーのページが更新されます。

   </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ウィジェット設定</td> 
      <td>
      <p>個々のウィジェットの設定を変更します。</p> 
      <p>

   >[!NOTE]
   >
   >これらのオプションは、概要パネルには拡張されません。 その領域は、レイアウトテンプレートの「概要」タブで設定する必要があります。

   </p>
      <p> 左のリストで次のウィジェットから選択します。</p>
      <ul>
        <li>マイプロジェクト</li>
        <li>マイタスク</li>
        <li>マイ問題</li>
      </ul>
      <p>編集するウィジェットを選択したら、右側のホームで使用できるようにする <b> フィルター </b>、<b> 列 </b>、<b> グループ </b> を選択します。</p>
      <p> 実行できる操作：</p>
      <ul>
      <li><p>リストのオプションの横にあるボックスをオンにして、ユーザーが使用できるフィルター、列、グループを選択して並べ替えます。 チェックを外したオプションはユーザーには表示されません。</p></li>
      <li> <p>リスト内のオプションをドラッグ＆ドロップして、順序を設定します。</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* [ フィルタ ]、[ 列 ]、および [ グループ ] オプションは、レイアウト テンプレートのリスト カスタマイズ オプションにリンクされています。 ここで行った変更は、これらの設定にも適用されます。
   >* 管理者カラムの構成をホーム ページに適切に適用するには、ユーザーに少なくともビューへの作成アクセス権が必要です。

   </p>
      <li><p>オプションの上にマウスポインターを置いて、「デフォルトとして設定 <b> をクリックして、ウィジェットのデフォルトのフィルターまたはグループを設定し </b> す。 現在のデフォルトでは、右側に青い <b> デフォルト </b> バッジが表示されます。</p></li>
      <li><p>各リストの下部にあるプラス記号ボタンをクリックして、使用可能なオプションのリストに既存のフィルター、列またはグループを追加し、そのリストにオプションを追加します。 この方法で追加できるのは、既存のフィルター、フィールド（カラム用）、グループのみであることに注意してください。</p></li>
      </ul>
      <p>

   >[!NOTE]
   >
   >レイアウトテンプレートを使用して特定のウィジェットにデフォルトのフィルターまたはグループ化を設定した場合、既存のユーザー設定によりすぐには有効にならない場合があります。新しいフィルターまたはグループ化を直ちに適用するには、システム管理者またはユーザーが、URL の末尾に「/resetUser」を付けて、ユーザーの環境設定をリセットする必要がある場合があります。

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、左下隅の「**保存**」をクリックします。

   >[!IMPORTANT]
   >
   >レイアウトテンプレートからカスタマイズを表示するには、ユーザーがホームページを更新する必要があります。
