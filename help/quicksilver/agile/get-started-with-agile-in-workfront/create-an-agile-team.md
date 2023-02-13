---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: アジャイルチームの作成
description: Adobe Workfrontは、アジャイルチームが段階的かつ整理的な方法で作業を完了できるようにします。
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# アジャイルチームの作成

[!DNL Adobe Workfront] アジャイルチームは、段階的で整理された方法で作業を完了できます。

組織内の任意のユーザーは、アジャイルチームを表示し、バックログ、反復、ストーリーボード、個々のストーリーを含む、チームのアジャイルコンポーネントをすべて表示できます。 ただし、 [!UICONTROL 編集] 作業にアクセスすると、チームに割り当てられた作業に変更を加えることができます。

[!DNL Workfront] は、次のアジャイルな方法論をサポートしています。

* **[!UICONTROL スクラム]**:チームには、実行する必要がある作業のバックログがあります。 チームが特定の作業チャンクに対して作業を行う準備が整うと、作業はバックログから反復に移動します。 スクラムチームの管理について詳しくは、 [機敏なチームのスクラム](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL かんばん]:** チームは、かんばんビューで、事前に定義されたステータスにわたって作業を移動します。 デフォルトのステータスは次のとおりです。バックログ、処理中、完了。 かんばんチームの管理の詳細は、 [アジャイルチームのかんばん](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL プラン ] を使用して新しいアジャイルチームを作成する[!UICONTROL Work] 以降：チームをアジャイルチームに変換する場合</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、 [!DNL Workfront] 管理者。

## 機敏な方法論の決定

アジャイルチームには、スクラムまたはかんばんアジャイルの方法を使用できます。 各方法には様々な利点があります。 アジャイルチームの作業方法によって、使用するアジャイルな方法が決まります。

でのスクラムおよびかんばんのアジャイル方法論 [!DNL Workfront] ストーリーをストーリーボード全体に移動して、ステータスの変更と進行状況を示すことができます。

でのスクラムおよびかんばんアジャイル方法 [!DNL Workfront] 次の点が異なります。

### でかんばんを使用するメリット [!DNL Workfront]

この [!DNL Kanban] ～の機敏な方法論 [!DNL Workfront] を使用すると、進行中の作業量を制限しながら、より簡単にストーリーをアジャイルなストーリーボードに移動できます。 を使用する際に、開始日と終了日は設定されません [!DNL Kanban] アジャイル手法

次の機能では、この方法がサポートされています。

* バックログを [!DNL Kanban] アジャイルストーリーボード。\
   詳しくは、 [バックログを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* バックログの項目が自動的に [!UICONTROL かんばん] 他の項目が「完了」と等しいステータスに移動された場合のアジャイルストーリーボード。\
   詳しくは、 [バックログから自動的に追加されるストーリーの設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) 記事内 [かんばんの構成](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* WIP(Work In Progress) 制限を [!UICONTROL かんばん] アジャイルストーリーボード。\
   詳しくは、 [かんばんボードでの作業中 (WIP) の制限の管理](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### で Scrum を使用するメリット [!DNL Workfront]

スクラムアジャイルの手法： [!DNL Workfront] では、一連のストーリーをアジャイルな反復に追加し、その反復に対してストーリーボードを作成できます。 繰り返しは、定義した開始日と終了日に基づいておこなわれます。

次の機能では、この方法がサポートされています。

* 次に関する問題を含めます： [!UICONTROL スクラム] ストーリーボード
* アジャイルチームのバックログに関する問題を含める
* サブタスクは [!UICONTROL スクラム] ストーリーボード
* バーンダウンチャートを表示して、反復中のストーリーに対する進捗を確認します\
   詳しくは、 [アジャイルバーンダウンチャートの概要](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 新しいアジャイルチームを作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.
1. 次をクリック： **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)を選択し、「 **[!UICONTROL 新規チームの作成]**.

   ![「新しいチームを作成」を選択します。](assets/create-new-team-350x198.png)

1. 次の情報を [!UICONTROL 新規チーム] ダイアログ：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL チーム名 ]</strong> </td> 
      <td>新しいアジャイルチームの名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL アジャイルチーム ]</strong> </td> 
      <td>この新しいチームをアジャイルチームに設定するには、このオプションを選択します。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL グループ ]</strong> </td> 
      <td> <p>チームに追加するグループの名前を入力し、ドロップダウンリストに表示されたら名前を選択します。</p> <p>注意：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理できます。 グループ管理者は、[!UICONTROL メインメニュー ] から [!UICONTROL チーム ] 領域に移動し、[!UICONTROL チームを切り替え ] 矢印をクリックできます。 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> ：管理するグループに割り当てられているすべてのチームをリストします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL チームメンバー ]</strong> </td> 
      <td>チームに参加するユーザーの名前を入力し始め、ドロップダウンリストに表示されたら名前を選択します。<br>複数のユーザーをチームに追加するには、この手順を繰り返します。<br>ユーザーは複数のチームに参加できるので、俊敏なチームと俊敏でないチームの両方に参加できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 説明 ]</strong> </td> 
      <td><p>チームの説明を入力します。</p> <p>チームを選択すると、[!UICONTROL チーム ] 領域の右上に説明が表示されます。</p>
      <p>説明が長い場合は、クリックすると完全な説明がポップアップで表示されます。 [!UICONTROL チーム設定 ] の編集権限を持っている場合は、ポップアップで直接説明を編集することもできます。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 作成]**」をクリックします。

   アジャイルチームの設定について詳しくは、次の記事を参照してください。

   * [設定 [!UICONTROL かんばん]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [設定 [!UICONTROL スクラム]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 既存のチームをアジャイルチームに変換する

既存のチームをアジャイルチームに変換できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.
1. 次をクリック： **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。

1. アジャイルチームに変換するチームを選択します。
1. 次をクリック： **[!UICONTROL 詳細]** メニューから、 **[!UICONTROL 編集]**.\
   次のいずれかを持つチームメンバーのみ [!UICONTROL プラン] または [!UICONTROL 作業] ライセンスこのオプションを参照してください。\
   ![](assets/edit-team-settings-350x205.png)

1. 内 **[!UICONTROL アジャイル]** セクション、選択 **[!UICONTROL アジャイルチームです]**.

1. 内 **[!UICONTROL 方法]** セクションで、チームが **[!UICONTROL スクラム]** または **[!UICONTROL かんばん]** アジャイル手法

1. クリック **変更を保存します。**

   アジャイルチームの設定について詳しくは、次の記事を参照してください。

   * [設定 [!UICONTROL かんばん]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [設定 [!UICONTROL スクラム]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
