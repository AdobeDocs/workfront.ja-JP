---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: ページヘッダーにフィルターボタンが表示されない
description: ページヘッダーに表示されないフィルターボタンのトラブルシューティングについては、この記事を参照してください。
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: ht
source-wordcount: '276'
ht-degree: 100%

---

# ページヘッダーにフィルターボタンが表示されない

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

次のフィルターボタンは、それぞれのエリアに表示されません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] エリア</strong></td> 
   <td><strong>フィルターボタン</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects I'm On]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## ソリューション

[!UICONTROL プロジェクトとタイムシート]エリアのフィルターボタンは、対応するフィルターがユーザーに適用されるレイアウトテンプレートに含まれていないため表示されません。[!DNL Workfront] 管理者は、フィルターを含むレイアウトテンプレートを割り当てる必要があります。

>[!NOTE]
>
>場合によっては、[!UICONTROL 設定]の[!UICONTROL リストコントロール]エリアからフィルターが削除されることがあります。[!DNL Workfront] 管理者はこれらをレイアウトテンプレートで使用できるように、このエリアのリストにこれらを含める必要があります。

1. レイアウトテンプレートに次のフィルターが表示されていることを確認します。

   * [!UICONTROL プロジェクト]エリアの[!UICONTROL 担当プロジェクト]と[!UICONTROL 所有プロジェクト]
   * [!UICONTROL タイムシート]エリアの[!UICONTROL マイタイムシート承認] と [!UICONTROL マイタイムシート]

   手順は次のとおりです。

   1. レイアウトテンプレートにアクセスします。
   1. **[!UICONTROL ユーザーの表示項目をカスタマイズする]**&#x200B;の下にある&#x200B;**[!UICONTROL リスト]**&#x200B;を選択します。
   1. **[!UICONTROL カスタマイズするリストを選択する]**&#x200B;の下にある&#x200B;**[!UICONTROL プロジェクト]**&#x200B;または&#x200B;**[!UICONTROL タイムシート]**&#x200B;を選択します。
   1. 「**[!UICONTROL フィルター]**」セクションで、**[!UICONTROL 担当プロジェクト]**、**[!UICONTROL 所有プロジェクト]**（プロジェクトの場合）および&#x200B;**[!UICONTROL マイタイムシート承認]**&#x200B;と&#x200B;**[!UICONTROL マイタイムシート]**（タイムシートの場合）が選択されていることを確認します。
   1. 「**[!UICONTROL 保存]**」をクリックします。

   詳しくは、[レイアウトテンプレートを使用したフィルター、ビュー、およびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. レイアウトテンプレートを正しいユーザー、担当業務、チーム、またはグループに割り当てます。詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。
