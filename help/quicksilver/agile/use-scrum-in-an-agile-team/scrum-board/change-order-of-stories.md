---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードでのストーリーの順序の変更
description: ストーリーボード上でのストーリーの表示順序は、優先度を示すものではありません。 しかし、物語をより目に見えるものにすることで、それは知覚される優先順位に影響を与えることができます。 デフォルトでは、ストーリーは、各 [!UICONTROL ステータス] ストーリーのボードの列。
author: Lisa
feature: Agile
exl-id: 326d78e0-06de-4b98-8fa6-102e0fd89d76
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# ストーリーの順序を変更 [!UICONTROL スクラム] ボード

ストーリーボード上でのストーリーの表示順序は、優先度を示すものではありません。 しかし、物語をより目に見えるものにすることで、それは知覚される優先順位に影響を与えることができます。 デフォルトでは、ストーリーボードの各ステータス列内に、ストーリーがアルファベット順に表示されます。 （スイムレーンのあるストーリーはストーリーボードの上部に表示され、スイムレーンのないストーリーはスイムレーンの下に別々に表示されます）。

ストーリーボード上の列を並べ替えると、行った変更はイテレーションまたはプロジェクトに保存されるので、次回ユーザがストーリーボードを表示したときにも変更が保持されます。 （ブラウザーのキャッシュをクリアしても、加えた変更は元に戻されません）。

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
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 反復でストーリーの順序を変更

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL チーム]**.

1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 並べ替えるストーリーが含まれている繰り返しまたはプロジェクトに移動します。
1. ストーリーカードまたはスイムレーンを、ストーリーボード上のステータス列内の目的の垂直位置にドラッグします。

## プロジェクト内のストーリーの順序を変更する

俊敏な反復とは異なり、俊敏なビューでプロジェクトを表示する際にストーリーの順序を変更することはできません。 プロジェクトのストーリーの順序を変更するには、プロジェクトを標準ビューで表示する必要があります。

プロジェクトビューを変更する方法については、 [[!UICONTROL プロジェクトを管理] 内 [!UICONTROL アジャイル] 表示](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md). アジャイルビューを選択する代わりに、標準ビューを選択します。
