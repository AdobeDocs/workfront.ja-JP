---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：ユーザーの個人の休暇
description: 表示：ユーザーの個人的な休暇
author: Nolan
feature: Reports and Dashboards
exl-id: 9b55b302-5cdc-4437-9ce4-a15b5b43dccb
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 87%

---

# 表示：ユーザーの個人の休暇

<!--Audited: 11/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider hiding this article because this is not a custom view anymore.)</p>
-->

休暇レポートを作成して、ユーザーの休暇情報を取り込むことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p> 現在： 
   <ul>
   <li>表示の変更をリクエスト</li> 
   <li>レポートを変更するためのプラン</li>
   </ul>
     </p>
     <p> 新規： 
   <ul>
   <li>ビューを変更する場合は Contributor</li> 
   <li>レポートを変更する場合は Standard</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーの個人の休暇を表示

1. 右上隅の **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**レポート /新しいレポート** をクリックします。
1. ドロップダウンメニューから、「**休暇**」を選択します。
1. 「**保存して閉じる**」をクリックします。

   デフォルトでは、レポートのビューに次のフィールドが表示されます。

   | ユーザー | プロファイルで休暇を示したユーザーの名前。 |
   |---|---|
   | 開始日 | ユーザーが示した休暇の期間の開始日。 |
   | 終了日 | ユーザーが示した休暇の期間の終了日。 |

   {style="table-layout:auto"}

1. （オプション）次のいずれかのタブを編集して、レポートの作成を完了します。

   * カラム（表示）
   * グループ化
   * フィルター
   * グラフ

   レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。

   >[!TIP]
   >
   >レポートを読みやすくするために、User オブジェクトのグループ化を追加することをお勧めします。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Add Time Off information to a user report</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: old way of doing this, not working anymore)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To add a column to a user view or report to display a list of future days which have been marked for time off by users:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/time-off-report-350x61.png" alt="time_off_report.png" style="width: 350;height: 61;"> </p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;<strong>Reports > New Report.</strong> </li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the&nbsp;<strong>New Report</strong> drop-down menu, select&nbsp;<strong>User Report</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Add Column</strong>.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the header of the new column, then click<strong>Switch to Text Mode</strong>.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
   -->

<!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:<br><!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre>
   </li>
   -->

<!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <strong>Save</strong>+<strong>Close</strong>.</li>
   -->
