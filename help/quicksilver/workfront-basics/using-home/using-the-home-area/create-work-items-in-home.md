---
product-area: projects
navigation-topic: use-the-home-area
title: ホームエリアからの作業アイテムの作成
description: 作業項目は、[!UICONTROL ホーム]領域から作成できます。自分で個人用タスクを作成したり、他のユーザーから作業を依頼したり、特定のプロジェクトにタスクを追加したりできます。
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 95%

---

# ホームエリアからの作業アイテムの作成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

作業項目は、[!UICONTROL ホーム]領域から作成できます。自分で個人用タスクを作成したり、他のユーザーから作業を依頼したり、特定のプロジェクトにタスクを追加したりできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker]</p> <p><b>メモ</b></p> 
   <p>まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>タスクに対する [!UICONTROL Edit] アクセス権以上</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 個人用タスクの作成

[!UICONTROL ホーム] 領域でのみ利用可能な個人用タスクを作成できます。

1. 右上の [**[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png)]、[**[!UICONTROL ホーム]**] の順にクリックします。
1. [**[!UICONTROL 新規タスク]**] > [**[!UICONTROL 個人]**] をクリックします。

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. [**[!UICONTROL 名前]**] フィールドで、タスクの名前を指定します。
1. (オプション）[**[!UICONTROL 日付を選択]**] をクリックし、タスクの期限を選択します。これにより、タスクの[!UICONTROL 予定完了日]を設定できます。\
   右側のパネルで日付をクリックするか、**[!UICONTROL を変更することで、**[!UICONTROL &#x200B;予定完了日&#x200B;]**を変更できます。 これは、日付を直接タスクに]** して行います。

1. [**[!UICONTROL 作成]**] をクリックしてタスクを保存します。\
   タスクが自分に割り当てられ、[!UICONTROL ホーム]領域で利用可能になります。

>[!NOTE]
>
>* 個人用タスクを作成すると、そのタスクは、[!UICONTROL Workfront] で検索できない「非表示」プロジェクトに保存されます。プロジェクトの名前は「&lt;ユーザー名> のタスク」です。「ユーザー名」は、タスクを作成したユーザーのフルネームです。このプロジェクトにアクセスできるのは、タスクのパンくずリストなど、[!UICONTROL ホーム]領域にある個人用タスクをクリックした場合のみです。
>
>* 通常のプロジェクトタスクとは異なり、個人用タスクには、Workfrontインターフェイスに表示される一部のフィールドが制限され、プロジェクトのタイムラインや進行状況には影響しません。個人用タスクを別のユーザーに再割り当てすると、すべてのタスクフィールドが個人用タスクに追加されますが、タスクを作成したユーザーの個人用プロジェクトにタスクが残ります。
>
>
>* 個人用タスクは、時間が記録されている場合、またはタイムシートに固定されている場合にのみ、タイムシートに表示されます。 個人のタスクをタイムシートに固定できるのは、タスクに対して時間が記録されている場合のみです。 詳しくは、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。
> 
>* 個人用タスクを通常のワークフローの一部にしたい場合は、プロジェクトを作成し、個人用タスクをそのプロジェクトに移動することをお勧めします。
>
> ![[!UICONTROL 個人用タスクのプロジェクト]](assets/createworkitems-personal--project-350x105.png)

## 別のユーザーからの作業をリクエスト

別のユーザーに対しては、ホーム領域から直接作業を要求できます。このセクションで説明するように、別のユーザーから作業をリクエストすると、ユーザーが [**[!UICONTROL 作業開始]**] をクリックするまで、タスクがユーザーのホーム領域にリクエストとして表示されます

[!UICONTROL ホーム]領域で別のユーザーから作業をリクエストするには

1. 右上の [**[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png)]、[**[!UICONTROL ホーム]**] の順にクリックします。
1. [**[!UICONTROL 新規タスク]**] をクリックし、[**[!UICONTROL リクエスト]**] を選択します。

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. [**[!UICONTROL 名前]**] フィールドで、タスクの名前を指定します。
1. [**[!UICONTROL 割り当て先]**] フィールドに、割り当てるユーザー、チームまたは役割の名前を入力し、ドロップダウンメニューに表示されたら名前をクリックします。
1. [[!UICONTROL 名前を付けて追加] ドロップダウンメニューで、タスクまたはイシューを追加するかどうかを選択します。
1. [**[!UICONTROL 日付を選択]**] をクリックし、タスクの期限の日時を選択します。
1. [**[!UICONTROL 作成]**] をクリックしてタスクを保存します。\
   タスクは、指定した[!UICONTROL ホーム]領域で作業リクエストとして表示されます。

## プロジェクトへのタスクまたはイシューの追加

既存のプロジェクトにタスクやイシューをホーム領域から直接追加できます。

1. 右上隅にある&#x200B;**[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png)、「**ホーム**」の順にクリックします。
1. 「**[!UICONTROL 新規タスク]**」をクリックし、「**[!UICONTROL プロジェクトタスク]**」を選択します。

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. **[!UICONTROL 名前]**&#x200B;フィールドで、タスクまたはイシューの名前を指定します。
1. **[!UICONTROL 割り当て先]**&#x200B;フィールドに、割り当てるユーザー、チームまたは役割の名前の入力を開始し、ドロップダウンメニューに表示されたら名前をクリックします。
1. タスクまたはイシューを作成するプロジェクトの名前の入力を開始し、ドロップダウンメニューに表示されたら名前をクリックします。

   >[!IMPORTANT]
   >
   >プロジェクト[!UICONTROL ステータス]が[!UICONTROL 現在]に設定されている場合にのみ、[!UICONTROL 作業リスト]にタスクまたはイシューが表示されます。

1. （条件付き）イシューを作成するには、******[!UICONTROL 名前を付けて追加]**&#x200B;ドロップダウンメニューからイシューを選択します。デフォルトでは、**[!UICONTROL タスク]**&#x200B;が選択されています。

1. 「**[!UICONTROL 日付を選択]**」をクリックし、タスクの期限の日時を選択します。
1. 「**[!UICONTROL 作成]**」をクリックしてタスクを保存します。
