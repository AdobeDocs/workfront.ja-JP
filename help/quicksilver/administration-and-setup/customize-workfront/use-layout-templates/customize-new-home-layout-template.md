---
title: レイアウトテンプレートを使用したホームのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートを使用すると、Adobe Workfrontでホームを開いたときに表示される内容を設定できます。
author: Lisa and Courtney
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
TQID: https://experienceleague.adobe.com/j2Y56liYA3jg5L5GFq--2iLfv3kYPI7MsyaLWIlzZ0o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 837
ht-degree: 36%

---

# レイアウトテンプレートを使用したホームのカスタマイズ

レイアウトテンプレートを使用すると、ユーザーが最初にホームを開いたときに表示される内容を設定できます。

以下を設定できます。

* デフォルトでワークスペースに表示されるウィジェット
* 背景の選択
* 特定のウィジェット設定（マイプロジェクト、マイタスク、マイタスク、マイイシューのウィジェットで使用できるフィルターとグループ、そのデフォルトなど）

>[!IMPORTANT]
>
>エンドユーザーは、レイアウトテンプレートが適用された後、ページ上の背景を変更したり、ウィジェットを並べ替えたりできます。 Workfront Administratorに含まれているウィジェットを削除できません。
> 
>管理者は、ユーザーに新しいウィジェットを追加できます。 ただし、エンドユーザーが既にウィジェットの順序または背景選択をカスタマイズしている場合、それらの特定のカスタマイズは変更されません。

ホームについて詳しくは、[&#x200B; ホームの基本を学ぶ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md)を参照してください。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。 レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

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

## レイアウトテンプレートを使用したホームのカスタマイズ

レイアウトテンプレートを使用してホームをカスタマイズするには：

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。

1. **ユーザーに表示される内容をカスタマイズ**&#x200B;の下の下向き矢印![下向き矢印](assets/dropdown-arrow.png)をクリックし、**ホーム Workspace**&#x200B;をクリックします。

1. 右側のタブで、次のいずれかをクリックします。

   * **デザインとレイアウト**: ウィジェットと背景を選択して配置します
   * **ウィジェット設定**：利用可能なフィルターやグループなど、個々のウィジェットの設定を管理する場合に選択します。

   次の表に、各タブの詳細を示します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">デザインとレイアウト</td> 
      <td>
      <p>ユーザーのワークスペースに表示するウィジェットとその位置を選択し、背景を選択します。</p> 
      <p>ユーザーは選択したウィジェットを削除することはできませんが、移動やサイズ変更は自由にできます。 ウィジェットを追加することもできます。</p>
      <p>このタブは、基本的に、このレイアウトテンプレートを使用するユーザーが体験する実際のホームワークスペースのプレビューとして機能します。</p> 
      <p> 次のいずれかの操作を行います。 </p>
      <ul><li>このタブは、<a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref"> ホーム </a>でのウィジェットの追加、編集、削除の手順に従ってカスタマイズします。 </li>
      <li>ウィジェットを選択し、ユーザーに対して表示するようにワークスペースを配置します。</li>
      <li>背景を変更するには、<a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref"> ホームの基本を学ぶ</a>の<b>背景カスタマイズ </b>の手順に従います。</li></p>
      <p>

   >[!NOTE]
   >
   >レイアウトテンプレート内のウィジェットを移動したりサイズを変更したりするだけでは、ユーザーのホームページにレイアウトの更新をトリガーすることはできません。 ただし、ウィジェットを追加または削除すると、ユーザーのページが更新されます。

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
   >これらのオプションは、概要パネルには適用されません。 レイアウトテンプレートの「概要」タブでその領域を設定する必要があります。

   </p>
      <p> リストから左のウィジェットを選択します。</p>
      <ul>
        <li>マイプロジェクト</li>
        <li>マイタスク</li>
        <li>マイ問題</li>
      </ul>
      <p>編集するウィジェットを選択したら、右側のホームで利用できるようにしたい<b> フィルター</b>、<b>列</b>、および<b> グループ </b>を選択します。</p>
      <p> 実行できる操作：</p>
      <ul>
      <li><p>リストのオプションの横にあるボックスをオンにして、ユーザーが利用できるフィルター、列、またはグループを選択して並べ替えます。 チェックを外したオプションはユーザーには表示されません。</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* フィルター、列、グループの各オプションは、レイアウトテンプレートのリストカスタマイズオプションにリンクされています。 ここで行った変更は、これらの設定にも適用されます。
   >* 管理者の列設定をホームページに適切に適用するには、ユーザーに少なくとも「ビューへのアクセスを作成」権限が必要です。
   ></p>
   >   <li><p>ウィジェットのデフォルトのフィルターまたはグループを設定するには、オプションの上にカーソルを置き、<b> デフォルトとして設定</b>をクリックします。 現在のデフォルトでは、右側に青い<b>Default</b> バッジが表示されます。</p></li>
   >   <li><p>各リストの下部にあるプラス記号ボタンをクリックして、既存のフィルター、列、またはグループを使用可能なオプションのリストに追加し、そのリストにオプションを追加します。 この方法で追加できるのは、既存のフィルター、フィールド（カラム用）、グループのみであることに注意してください。</p></li>
   >   </ul>
   >   <p>

   >[!NOTE]
   >
   >レイアウトテンプレートを使用して特定のウィジェットにデフォルトのフィルターまたはグループ化を設定した場合、既存のユーザー設定によりすぐには有効にならない場合があります。 新しいフィルターまたはグループ化を直ちに適用するには、システム管理者またはユーザーが、URL の末尾に「/resetUser」を付けて、ユーザーの環境設定をリセットする必要がある場合があります。

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. レイアウトテンプレートのカスタマイズを続行します。 「**適用**」はいつでもクリックして、進行状況を保存できます。

   または

   カスタマイズが完了したら、**保存して閉じる**&#x200B;をクリックします。

   >[!IMPORTANT]
   >
   >レイアウトテンプレートからカスタマイズを表示するには、ユーザーがホームページを更新する必要があります。
