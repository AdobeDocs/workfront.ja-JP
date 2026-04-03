---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードのストーリーの順序の変更
description: ストーリーボード上でのストーリーの表示順序は、優先度を示すものではありません。しかし、ストーリーを目につきやすくすることで、認識時の優先度に影響を与える可能性があります。デフォルトでは、ストーリーはストーリーボードのそれぞれの[!UICONTROL ステータス]列内に、アルファベット順に表示されます。
author: Courtney
feature: Agile
exl-id: 326d78e0-06de-4b98-8fa6-102e0fd89d76
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 73%

---

# [!UICONTROL スクラム]ボードでストーリーの順序を変更

ストーリーボード上でのストーリーの表示順序は、優先度を示すものではありません。しかし、ストーリーを目につきやすくすることで、認識時の優先度に影響を与える可能性があります。優先度はバックログで定義され、ストーリーがストーリーボードに取り込まれた場合、イテレーション期間中に作業が行われるため、優先度は設定されません。 バックログにストーリーが返された場合は、優先順位を示すためにストーリーを並べ替えることができます。

デフォルトでは、ストーリーはストーリーボードのそれぞれのステータス列内に、アルファベット順に表示されます。スイムレーン付きのストーリーはストーリーボードの上部に表示され、スイムレーンなしのストーリーはスイムレーンの下に個別に表示されます。

ストーリーボード上で列の順序を変更すると、加えたがイテレーションまたはプロジェクトに保存されるため、自分または別のユーザーが次回ストーリーボードを表示するときにも変更内容が保持されます。（ブラウザーキャッシュをクリアしても、加えた変更は元に戻せません）。

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

## イテレーションでストーリーの順序を変更

{{step1-to-team}}

1. （オプション）「**[!UICONTROL チームを切り替え]**」アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 順序を並べ替えるストーリーが含まれているイテレーションまたはプロジェクトに移動します。
1. ストーリーカードまたはスイムレーンを、ストーリーボード上のステータス列内の目的の垂直位置にドラッグします。

## プロジェクト内のストーリーの順序を変更

アジャイルイテレーションとは異なり、アジャイルビューでプロジェクトを表示する際にストーリーの順序を変更することはできません。 プロジェクトのストーリーの順序を変更するには、プロジェクトを標準ビューで表示する必要があります。

プロジェクトビューを変更する方法について詳しくは、[!UICONTROL アジャイル]ビュー](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)にある[[!UICONTROL プロジェクトを管理]を参照してください。アジャイルビューを選択する代わりに、標準ビューを選択します。
