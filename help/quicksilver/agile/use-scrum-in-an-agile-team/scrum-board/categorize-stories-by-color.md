---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードのカラーでストーリーを分類
description: スクラムボードストーリーのデフォルトの色分けは、ストーリーボードが反復に配置されているかプロジェクトに配置されているかによって異なります。
author: Courtney
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 67%

---

# [!UICONTROL スクラム]ボードでのストーリーの色分け

## ストーリーのデフォルト色分けの変更

ストーリーのデフォルトの色分けは、ストーリーボードが反復に配置されているかプロジェクトに配置されているかによって異なります。

* **[!UICONTROL イテレーション]**：イテレーションでは、ストーリーボードのタイルは、ストーリーが関連付けられているプロジェクトに従って色分けされます。（各プロジェクトには、ストーリーボード上で任意にカラーが割り当てられます）。 各アジャイルチームのデフォルトの動作を変更できます。 イテレーションのアジャイルストーリーの色は、プロジェクト（デフォルト）、ストーリーの優先順位、所有者、またはフリーフォームに関連付けることができます。 詳しくは、[ スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4)の記事「[ アジャイルストーリーボード ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)」のストーリーにカラーインジケーターを使用する方法の設定を参照してください。

* **[!UICONTROL プロジェクト]**：プロジェクトでは、サブタスクは親タスクの色と一致するので、特定のスイムレーン内のストーリーの色はすべて同じになります。サブタスクや親タスクがないタスクの色は、タスクを作成するときにランダムに割り当てられます。アジャイルビューを変更することで、このデフォルトの動作を変更できます。 プロジェクトのアジャイルストーリーの色は、親ストーリー（デフォルト）、ストーリーの優先順位、所有者、またはフリーフォームに関連付けることができます。 詳しくは、[ビューの概要： [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) の[[!UICONTROL アジャイル]ビューの作成またはカスタマイズ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p> 
   または
   <p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 自由形式を使用した場合のストーリーの色の変更

アジャイルチームの設定で「[!UICONTROL  カードカラーを]に関連付ける」オプションが[!UICONTROL  フリーフォーム ]」に設定されている場合、ユーザーは個々のストーリータイルの色を手動で変更できます。 これは、チームや組織にとって重要な他の種類の情報を伝えるのに役立ちます。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定の反復を選ぶか、「**[!UICONTROL 進行中の反復]**」を選択します。
1. ストーリータイルの上部にある色付きバナーにポインタを合わせます。

   ![ ストーリーカード ](assets/agile-story-color1-nwe-350x140.png)

1. 「**[!UICONTROL 色の変更]**」をクリックし、目的の色を選択します。

   ![ カラーを選択](assets/agile-story-color2-nwe-350x138.png)
