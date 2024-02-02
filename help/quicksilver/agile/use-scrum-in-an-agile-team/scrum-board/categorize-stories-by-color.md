---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードでのストーリーの色分け
description: スクラムボードストーリーのデフォルトの色分けは、ストーリーボードが反復に配置されているかプロジェクトに配置されているかによって異なります。
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: ht
source-wordcount: '464'
ht-degree: 100%

---

# [!UICONTROL スクラム]ボードでのストーリーの色分け

## ストーリーのデフォルト色分けの変更

ストーリーのデフォルトの色分けは、ストーリーボードが反復に配置されているかプロジェクトに配置されているかによって異なります。

* **[!UICONTROL イテレーション]**：イテレーションでは、ストーリーボードのタイルは、ストーリーが関連付けられているプロジェクトに従って色分けされます。（各プロジェクトには、ストーリーボード上で色が任意に割り当てられます）。このデフォルトの動作は、アジャイルチームごとに変更できます。反復でのアジャイルストーリーの色は、プロジェクト（デフォルト）、ストーリーの優先度、所有者または自由形式に関連付けることができます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事の[アジャイルストーリーボードでストーリーに使用するカラーインジケーターの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4)を参照してください。

* **[!UICONTROL プロジェクト]**：プロジェクトでは、サブタスクは親タスクの色と一致するので、特定のスイムレーン内のストーリーの色はすべて同じになります。サブタスクや親タスクがないタスクの色は、タスクを作成するときにランダムに割り当てられます。このデフォルトの動作は、アジャイルビューを編集することで変更できます。プロジェクトでのアジャイルストーリーの色は、親ストーリー（デフォルト）、ストーリーの優先度、所有者または自由形式に関連付けることができます。詳しくは、[ビューの概要： [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) の[[!UICONTROL アジャイル]ビューの作成またはカスタマイズ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 自由形式を使用した場合のストーリーの色の変更

アジャイルチームの設定で「[!UICONTROL カードの色を関連付ける対象]」オプションが「[!UICONTROL 自由形式]」に設定されている場合、ユーザーは個々のストーリータイルの色を手動で変更できます。これは、チームや組織にとって重要な他の種類の情報を伝えるのに役立ちます。

1. [!DNL Adobe] Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**[!UICONTROL チーム]**」をクリックします。

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定の反復を選ぶか、「**[!UICONTROL 進行中の反復]**」を選択します。
1. ストーリータイルの上部にある色付きバナーにポインタを合わせます。

   ![](assets/agile-story-color1-nwe-350x140.png)

1. 「**[!UICONTROL 色の変更]**」をクリックし、目的の色を選択します。

   ![](assets/agile-story-color2-nwe-350x138.png)
