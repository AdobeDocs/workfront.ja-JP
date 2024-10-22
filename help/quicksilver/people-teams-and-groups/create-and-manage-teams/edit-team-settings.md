---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: チーム設定の編集
description: Workfront 管理者、またはプランライセンスもしくはワークライセンスを持つユーザーは、チーム設定を編集できます。
author: Lisa
feature: People Teams and Groups
exl-id: b6761188-8630-446e-bc70-70fe272881ce
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 90%

---

# チーム設定を編集

[!DNL Adobe Workfront] 管理者、または [!UICONTROL  標準 ]、[!UICONTROL  プラン ] または [!UICONTROL  作業 ] ライセンスを持つユーザーは、[!UICONTROL  チーム設定 ] を編集できます。

チームにユーザーを追加し、チームのレイアウトテンプレートを設定し、チームが作業項目を完了したときのステータスの記録方法を設定できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：ワーク以上</p></td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## チーム設定を編集

{{step1-to-team}}

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン（![チームの切り替えアイコン](assets/switch-team-icon.png)）をクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。

1. **[!UICONTROL その他]**&#x200B;メニュー（![](assets/more-icon.png)）をクリックして、「**[!UICONTROL 編集]**」を選択します。

   [!UICONTROL  標準 ]、[!UICONTROL  プラン ]、または [!UICONTROL  ワーク ] ライセンスのいずれかを持つチームメンバーのみがこのオプションを表示します。

   「[!UICONTROL 編集]」オプションがあるべきなのに表示されない場合は、[!UICONTROL スクラムチーム]、[!UICONTROL かんばんチーム]、または[!UICONTROL ウォーターフォールチーム]に対してレイアウトテンプレートで「[!UICONTROL チーム設定]」が表示されていることを確認するよう Workfront 管理者に依頼してください。

   ![](assets/edit-team-settings.png)

1. チーム設定では、次のような変更を行うことができます。

   * チーム名の変更
   * チームのディアクティベート
   * チームとグループの関連付け

     >[!NOTE]
     >
     >チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならなくてもチームを管理できます。グループ管理者は、「メインメニュー」から「チーム」エリアに移動して[!UICONTROL チームを切り替え]矢印（![チームを切り替えアイコン](assets/switch-team-icon.png)）をクリックし、自分が管理するグループに割り当てられているすべてのチームを一覧表示することができます。

     正しいグループにマウスを移動し、その横に表示される情報アイコン（![](assets/info-icon.png)）をクリックすると、自分がそのチームに関連付けられていることを確認できます。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。

   * チーム所有者の指定
   * チームメンバーの追加と削除
   * チームの説明の追加
   * チームへのレイアウトテンプレートの適用

     チームへのカスタムレイアウトテンプレートの適用について詳しくは、レイアウトテンプレートを使用した「[!UICONTROL 担当作業]」および「[!UICONTROL 作業要求]」エリアの変更の「チームへのカスタムテンプレートの適用」セクションを参照してください。

   * 「**[!UICONTROL これはアジャイル チームです]**」オプションを選択して、このチームがアジャイルチームかどうかを決定します。

     アジャイルチームとアジャイルチーム内での作業の管理方法について詳しくは、[アジャイルチームの作成](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md)を参照してください。

   * 「[!UICONTROL 作業をする]」ボタンを「[!UICONTROL 開始]」ボタンに変更します。「[!UICONTROL 開始]」ボタンの設定方法について詳しくは、[「作業をする」ボタンの「[!UICONTROL 開始]」ボタンへの置き換え](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)を参照してください。
   * 「**[!UICONTROL 完了]**」ボタンをカスタマイズします。「[!UICONTROL 完了]」ボタンをカスタマイズする方法の詳細については、次を参照してください。

      * [タスクの「[!UICONTROL 完了]」ボタンの設定](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
      * [イシューの「[!UICONTROL 完了]」ボタンの設定](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
