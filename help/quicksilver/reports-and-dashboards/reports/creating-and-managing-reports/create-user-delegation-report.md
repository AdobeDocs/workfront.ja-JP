---
product-area: reporting
keywords: ユーザー,デリゲーション,レポート,デリゲート,承認
navigation-topic: create-and-manage-reports
title: ユーザー委任レポートの作成
description: ユーザーのデリゲーションレポートの作成
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 95%

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準 </p>
   <p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>承認がデリゲートされた項目とデリゲーションに関係するユーザーに対する権限の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。
+++

## ユーザーのデリゲーションレポートの作成

1. Adobe Workfront の右上隅で&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**レポート**」をクリックします。

1. 「**新規レポート**」をクリックし、「**ユーザーのデリゲーション**」を選択します。\
   ![](assets/classic-new-report-user-delegation-350x644.png)

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
