---
product-area: reporting
keywords: ユーザー,デリゲーション,レポート,デリゲート,承認
navigation-topic: create-and-manage-reports
title: ユーザー委任レポートの作成
description: ユーザーのデリゲーションレポートの作成
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 87%

---

# ユーザーのデリゲーションレポートの作成

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

Adobe Workfront では、ユーザーがプロジェクト、タスクおよびイシューの承認を他のユーザーにデリゲートして、不在時に承認が管理されるようにすることができます。プランライセンスを持つユーザーは、ユーザーのデリゲーションレポートを作成して、次の項目を確認できます。

* タスク、イシューおよびプロジェクトの承認を別のユーザーにデリゲートしたユーザー
* 割り当てられたタスク、イシューおよびプロジェクトの承認をデリゲートしたユーザー

* デリゲーションが開始および終了する日付

承認のデリゲーションについて詳しくは、[承認リクエストのデリゲート](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
      <p>標準</p>
      <p>プラン</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
 <td> <p>承認がデリゲートされた項目とデリゲーションに関係するユーザーに対する権限の表示</p></td>  
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーのデリゲーションレポートの作成

1. Adobe Workfrontの右上隅にある **メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) をクリックし、**レポート** をクリックします。

1. 「**新規レポート**」をクリックし、「**ユーザーのデリゲーション**」を選択します。

   ![&#x200B; 新しいレポートユーザーの委任 &#x200B;](assets/classic-new-report-user-delegation-350x644.png)

   次のフィールドは、デフォルトでこのレポートに表示されます。

   | フィールド | 説明 |
   |---|---|
   | **デリゲート元ユーザー** | タスク、イシューおよびプロジェクトの承認を別のユーザーにデリゲートするユーザーです。 |
   | **デリゲート先ユーザー** | タスク、イシューおよびプロジェクト承認がデリゲートされたユーザーです。 |
   | **開始日** | デリゲーションを行ったユーザーの不在時間の開始時です。 |
   | **終了日** | デリゲーションを行ったユーザーの不在時間の終了時です。 |

   {style="table-layout:auto"}

1. （オプション）Report Builder で、次の変更を行います。

   * カラム（表示）
   * グループ化
   * フィルター
   * グラフ

   これらの機能について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

1. レポートの作成が完了したら、「**保存して閉じる**」をクリックします。

   レポートが表示されます。
