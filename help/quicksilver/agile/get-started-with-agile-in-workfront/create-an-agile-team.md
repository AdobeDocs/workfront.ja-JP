---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: アジャイルチームの編成
description: Adobe Workfrontなら、アジャイルチームは段階的かつ組織的に作業を進めることができます。
author: Courtney
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 57%

---

# アジャイルチームの作成

<!--Audited: 01/2024-->

[!DNL Adobe Workfront]を使用すると、アジャイルチームは段階的かつ整理された方法で作業を完了できます。

組織内の誰もがアジャイルチームを利用して、バックログ、イテレーション、ストーリーボード、個々のストーリーなど、チームのあらゆるアジャイルコンポーネントを確認できます。 ただし、[!UICONTROL 編集]アクセス権があるチームのメンバーだけが、チームに割り当てられた作業を変更することができます。

[!DNL Workfront]は次のアジャイル手法をサポートしています。

* **[!UICONTROL スクラム]**：チームには、完了する必要がある作業のバックログがあります。チームが特定の量の作業に取り組む準備ができると、その作業はバックログからイテレーションに移動されます。スクラムチームの管理について詳しくは、「[&#x200B; アジャイルチームのスクラム &#x200B;](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md)」を参照してください。

* **[!UICONTROL かんばん]：** チームは、カンバンビューで事前に設定されたステータス間で作業を移動します。デフォルトのステータスは、バックログ、処理中、完了です。カンバンチームの管理について詳しくは、[&#x200B; アジャイルチームでのカンバン &#x200B;](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>新しいアジャイルチームの編成</p>
  <p>チームをアジャイルチームに転換する能力</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## アジャイル手法の決定

スクラムとカンバンのどちらのアジャイル手法も使用できます。 それぞれの方法論には様々なメリットがあります。アジャイルチームの働き方によって、使用するアジャイル手法が決まります。

[!DNL Workfront]のスクラムとカンバンの両方のアジャイル手法を使用すると、ストーリーボード上でストーリーを移動して、ストーリーのステータスの変更と進行状況を示すことができます。

[!DNL Workfront]のスクラムとカンバンのアジャイル手法には、次のような違いがあります。

### [!DNL Workfront] でかんばんを使用するメリット

[!DNL Kanban]の[!DNL Workfront] アジャイル手法では、進行中の作業の量を制限しながら、アジャイルストーリーボード上でストーリーをより簡単に移動できます。 [!DNL Kanban] アジャイル手法を使用する場合、開始日と終了日はありません。

以下の機能が、この方法論をサポートします。

* バックログを[!DNL Kanban] アジャイルストーリーボードに表示します。
詳しくは、[バックログを[!UICONTROL かんばん]ボードに追加](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)を参照してください。

* 他のアイテムが完了と等しいステータスに移動されると、バックログ上のアイテムを自動的に[!UICONTROL &#x200B; カンバン &#x200B;] アジャイルストーリーボードに追加するように設定します。
詳しくは、[かんばんを設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)の記事にある[バックログから自動的に追加されるようにストーリーを設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)の節を参照してください。

* [!UICONTROL &#x200B; カンバン &#x200B;] アジャイルストーリーボードに表示する進行中の作業（WIP）制限を設定します。
詳しくは、[かんばんボードでの作業中（WIP）の制限を管理](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)を参照してください。

### [!DNL Workfront] でスクラムを使用するメリット

[!DNL Workfront]のスクラムアジャイル手法では、一連のストーリーをアジャイルイテレーションに追加し、そのイテレーション用のストーリーボードを作成できます。 イテレーションは、定義した開始日と終了日に基づくものです。

以下の機能が、この方法論をサポートします。

* [!UICONTROL スクラム]ストーリーボードにイシューを含めます。
* アジャイルチームのバックログに問題を含める
* サブタスクは、[!UICONTROL スクラム]ストーリーボードに表示可能
* バーンダウンチャートで、イテレーション中のストーリーに対する進捗を確認できます
詳しくは、[&#x200B; アジャイルバーンダウンチャートの概要](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)を参照してください。

## アジャイルチームの作成

{{step1-to-team}}

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) を選択し、「**[!UICONTROL 新規チームを作成]**」をクリックします。

   ![新しいチームを作成を選択](assets/create-new-team.png)

   「新規チーム」ボックスが表示されます。

1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>新しいアジャイルチームの名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>この新しいチームをアジャイルチームに設定するには、このオプションを選択します。</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
      <td>このチームを有効化するには、このオプションを選択します。非アクティブなチームは、他のユーザーが作業に割り当てる際には表示されません。 </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>チームに追加するグループの名前を入力し、ドロップダウンリストに表示されたら、名前を選択します。</p> <p><b>メモ</b></p> <p> チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、そのチームのメンバーにならなくてもチームを管理できます。管理するグループに割り当てられているすべてのチームのリストを表示するには、グループ管理者は、[!UICONTROL Main Menu] から [!UICONTROL Teams] 領域に移動し、[!UICONTROL Switch Teams] 矢印 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> をクリックできます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>チームに参加するユーザーの名前の入力を開始し、ドロップダウンリストに表示されたら、名前を選択します。<br>複数のユーザーをチームに追加するには、このプロセスを繰り返します。<br> ユーザーは複数のチームに所属できるため、アジャイル チームとアジャイル以外のチームの両方に所属できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>チームの説明を入力します。</p> <p>チームを選択すると、[!UICONTROL Teams] 領域の右上に説明が表示されます。</p>
      <p>説明が長い場合は、クリックすると完全な説明がポップアップで表示されます。[!UICONTROL team settings] を編集するアクセス権がある場合は、ポップアップで直接説明を編集することもできます。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 作成]**」をクリックします。

   アジャイルチームの設定について詳しくは、次の記事を参照してください。

   * [[!UICONTROL かんばん]の設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [[!UICONTROL スクラム]の設定](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 既存チームのアジャイルチームへの編成

既存のチームをアジャイルチームに転換するには、次のようにします。

{{step1-to-team}}

1. **[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。

1. アジャイルチームに転換するチームを選びます。
1. **[!UICONTROL その他]**&#x200B;メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

   [!UICONTROL Standard]、[!UICONTROL &#x200B; プラン &#x200B;]、[!UICONTROL Work]のライセンスを持つチームメンバーのみがこのオプションを表示します。
   ![編集を選択](assets/edit-team-settings.png)

1. **[!UICONTROL アジャイル]**&#x200B;セクションで、「**[!UICONTROL アジャイルチームです]**」を選択します。

1. **[!UICONTROL 手法]** セクションで、チームが&#x200B;**[!UICONTROL スクラム]**&#x200B;と&#x200B;**[!UICONTROL カンバン]**&#x200B;のアジャイル手法のどちらを使用するかを選択します。

1. 「**変更を保存**」をクリックします。

   チームはアジャイルチームとして保存されます。チームの編集時に、新しいチームをスクラムまたはかんばんチームとして設定できます。

   詳しくは、次の記事を参照してください。

   * [[!UICONTROL かんばん]の設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [[!UICONTROL スクラム]の設定](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
