---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: ジョブの役割の非アクティブ化
description: As a [!DNL Adobe Workfront] 管理者またはジョブロールへの管理者アクセス権を持つユーザーは、システムで古くなったジョブロールを無効にすることができます。 ジョブの役割を削除する代わりに非アクティブ化すると、その役割に関連付けられている履歴情報を保持できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# ジョブの役割の非アクティブ化

As a [!DNL Adobe Workfront] 管理者またはジョブロールへの管理者アクセス権を持つユーザーは、システムで古くなったジョブロールを無効にすることができます。 ジョブの役割を削除する代わりに非アクティブ化すると、その役割に関連付けられている履歴情報を保持できます。

また、以前に非アクティブ化されたジョブの役割を再アクティブ化することもできます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] ライセンス*</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ジョブロールへの管理者アクセス</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ジョブの役割を無効にした場合の影響

ジョブの役割を非アクティブ化すると、次の領域には表示されなくなります。

* この [!UICONTROL 割り当て] typeahead フィールド（タスク、テンプレートタスク、問題、承認、ルーティングルール用）
* この [!UICONTROL 割り当て] リストとレポートのフィールド
* ユーザープロファイル

   >[!NOTE]
   >
   >新しいロールをユーザーに追加しても、非アクティブ化されたジョブのロールは表示されません。 ただし、これは引き続き [!UICONTROL プライマリの役割] および [!UICONTROL その他の役割] ユーザーが非アクティブ化される前にジョブの役割に関連付けられていた場合は、フィールド。

* この [!UICONTROL 共有] レイアウトテンプレートの割り当てを含む、オブジェクトのダイアログボックス
* カスタムフォームの先頭に入力するフィールド
* この [!UICONTROL プールメンバー] ～に入る [!UICONTROL リソースプール]
* この [!UICONTROL ジョブの役割] フィールド [!UICONTROL 請求率] ユーザーがプロジェクトの請求率を上書きする場合の編集画面
* この [!UICONTROL かんばんボードに割り当てを追加] プロジェクトのダイアログボックス
* この [!UICONTROL ジョブの役割] 誰かが [!DNL Adobe Workfront Scenario Planner].

   この [!DNL Scenario Planner] は、新しい [!DNL Adobe Workfront] を使用し、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 [この [!DNL Scenario Planner] 概要](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>非アクティブ化された役割は、常にリスト、レポートおよび他のツール ( [!DNL Workload Balancer].

## ジョブロールを非アクティブ化する前の考慮事項

古くなった役割を削除するよりは、非アクティブにする方が効果的です。これにより、以前に使用した役割に関連する履歴情報をすべて保持できます。

>[!NOTE]
>
>非アクティブ化の前にジョブの役割に割り当てられた作業は、割り当てられたままとなります。

未使用のジョブロールを非アクティブ化する前に、次の操作を行うことをお勧めします。

* 非アクティブ化する予定のロールに割り当てられたオブジェクトに関するレポートを作成し、アクティブなジョブロールに再度割り当てます。 レポートの作成について詳しくは、 [レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >非アクティブな役割が割り当てられているタスクや問題に対してフィルターを適用するレポートを作成できます。 次に、レポートを使用して、未処理のタスクまたは問題をアクティブな役割に再割り当てします。

* 非アクティブ化し、アクティブなロールに再割り当てする予定のジョブロールに割り当てられているすべての承認プロセス、現在の承認パス、ルーティングルールまたはその他のオブジェクトのインベントリを作成します。

   >[!TIP]
   >
   >リクエストキューを使用する場合、ルーティングルールでデフォルトの担当者として割り当てられているジョブロールを非アクティブ化しても、ロールはそのまま残り、リクエストは非アクティブなロールにルーティングされます。 チームを非アクティブ化する前に、アクティブなロールでルーティングルールを更新することをお勧めします。

   承認プロセスおよびルーティングルールの作成について詳しくは、次の記事を参照してください。

   * [作業項目の承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [ルーティングルールの作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## ジョブロールを非アクティブ化

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、「 」をクリックしま&#x200B;す。 **[!UICONTROL ジョブの役割].**
1. （オプション） **[!UICONTROL フィルター]** ドロップダウンメニューで、「 **[!UICONTROL アクティブ]** ：アクティブなジョブのロールのみを表示します。
1. 非アクティブ化するジョブロールの名前をクリックします。
1. 内 **[!UICONTROL アクティブ]** ドロップダウンメニューで、「 **[!UICONTROL いいえ]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. クリック **[!UICONTROL 変更を保存]**.

   ジョブの役割は無効になり、作業に割り当てられなくなり、レイアウトテンプレートに関連付けられるようになります。 でのジョブの役割のすべての使用に関する情報 [!DNL Workfront]を参照してください。 [ジョブロールの概要](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
