---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: ページヘッダーにフィルターボタンが表示されない
description: ページヘッダーに表示されないフィルターボタンのトラブルシューティングについては、この記事を参照してください。
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# ページヘッダーにフィルターボタンが表示されない

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL システム管理者 ]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

次のフィルターボタンは、それぞれの領域に表示されません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 領域</strong></td> 
   <td><strong>フィルターボタン</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL プロジェクト ] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL プロジェクトを利用中 ]</p> </li> 
     <li> <p>[!UICONTROL プロジェクトは所有しています ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL タイムシート ]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL 自分のタイムシート承認 ]</span> </p> </li> 
     <li> <p><span>[!UICONTROL マイタイムシート ]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

「 [!UICONTROL プロジェクトとタイムシート] 対応するフィルターは、ユーザーに適用されたレイアウトテンプレートに含まれていないので、領域は表示されません。 この [!DNL Workfront] 管理者は、フィルターを含むレイアウトテンプレートを割り当てる必要があります。

>[!NOTE]
>
>フィルターが [!UICONTROL リストコントロール] 領域 [!UICONTROL 設定]. この [!DNL Workfront] 管理者がレイアウトテンプレートで使用できるようにするには、この領域のリストに管理者を含める必要があります。

1. レイアウトテンプレートに次のフィルターが表示されていることを確認します。

   * [!UICONTROL 自分がいるプロジェクト] および [!UICONTROL 自分が所有するプロジェクト] 内 [!UICONTROL プロジェクト] 領域
   * [!UICONTROL 自分のタイムシート承認] および [!UICONTROL マイタイムシート] 内 [!UICONTROL タイムシート] 領域

   手順は次のとおりです。

   1. レイアウトテンプレートにアクセスします。
   1. 選択 **[!UICONTROL リスト]** under **[!UICONTROL ユーザーに表示する内容をカスタマイズ]**.
   1. 選択 **[!UICONTROL プロジェクト]** または **[!UICONTROL タイムシート]** under **[!UICONTROL カスタマイズするリストを選択]**.
   1. 内 **[!UICONTROL フィルター]** セクションで、 **[!UICONTROL 自分がいるプロジェクト]**, **[!UICONTROL 自分が所有するプロジェクト]** （プロジェクトの場合）および **[!UICONTROL 自分のタイムシート承認]** および **[!UICONTROL マイタイムシート]** （タイムシートの場合）が選択されている。
   1. 「**[!UICONTROL 保存]**」をクリックします。

   詳しくは、 [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. レイアウトテンプレートを正しいユーザー、職務上の役割、チーム、またはグループに割り当てます。 詳しくは、 [レイアウトテンプレートにユーザーを割り当てる](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
