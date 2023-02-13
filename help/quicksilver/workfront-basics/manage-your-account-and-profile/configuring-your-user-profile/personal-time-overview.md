---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: での個人のオフタイムの設定 [!DNL Adobe Workfront]
description: Adobe Workfrontは、個人のタイムオフを管理、計上、および追跡するために、既存のシステムを複製または置き換えるように設計されていません。 ただし、承認のオフが発生するタイミングを指定することが重要です。承認のオフは、スケジュールに影響し、割り当てられているタスクの計画完了日に影響を与えるからです。
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e87f2a459314b8059a3df634e97560b5c1dffac4
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 1%

---

# での個人のオフタイムの設定 [!DNL Adobe Workfront]

[!DNL Adobe Workfront] は、個人のタイムオフを管理、計上、および追跡するために、既存のシステムを複製または置き換えるように設計されていません。

ただし、承認のオフが発生するタイミングを指定することが重要です。これは、スケジュールに影響し、 [!UICONTROL 計画完了日] 割り当てられているタスクの数を指定します。

例えば、2 週間かかる予定のタスクに割り当てられていて、その間に 3 日間の休暇を取る予定がある場合、 [!DNL Workfront] タスクタイムラインに 3 日を追加して、オフ時間を考慮します。

また、リソース管理ツールは、個人の休日を使用して、作業のスケジュールを設定できるタイミングを示します。

>[!NOTE]
>
>休日のスケジュールを設定した日付との不一致が生じないようにするには、ユーザープロファイルのタイムゾーンがスケジュールのタイムゾーンと一致するようにすることをお勧めします。 詳しくは、次の記事を参照してください。
>
>* [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>




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
   <td> <p>[!UICONTROL Work] 以降（個人のタイムオフを設定する場合）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td>[!UICONTROL ユーザーを編集 ] アクセス権を持つ [!UICONTROL Manager] （他のユーザーのタイムオフカレンダーを変更する場合）</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## での個人のオフタイムの設定 [!DNL Workfront]

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]をクリックし、プロフィール画像の横にあるユーザー名をクリックします。

1. 左側のパネルで、 **[!UICONTROL オフの時間]**.
1. 個人の休日に希望する日付を選択します。
1. 選択 **[!UICONTROL 終日]**&#x200B;を返します。\
   1 日未満のオフを取っていて、オフの開始時間と終了時間を示す場合は、このチェックボックスをオフのままにします。

1. 「**[!UICONTROL 保存]**」をクリックします。\
   オフタイムが [!DNL Workfront] システムを使用して、リソースグリッドなどのスケジューリングツールを実行します。 この時間に作業を割り当てると、予定時間がオフになったことをユーザーに知らせるツールヒントが表示されます。
