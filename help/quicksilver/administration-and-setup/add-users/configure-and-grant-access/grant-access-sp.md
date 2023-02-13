---
title: シナリオプランナーへのアクセス権の付与
description: Adobe Workfront管理者は、アクセス・レベルを使用して、シナリオ・プランナへのユーザーのアクセスを定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# シナリオプランナーへのアクセス権の付与

Adobe Workfront管理者は、シナリオ・プランナに対するユーザーのアクセスを定義するアクセス・レベルを使用できます。詳しくは、 [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

シナリオ・プランナへのアクセスに加えて、システム管理者以外のアクセス・レベルのユーザーは、予算、コスト、ジョブ・ロール・レートなど、計画に含まれる財務情報を確認するために、財務データへのアクセス権も持っている必要があります。 詳しくは、 [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>ビジネス以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上 詳しくは、 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfrontライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、Adobe Workfront Scenario Planner の追加ライセンスを購入する必要があります。</p> <p>Workfront Scenario Planner の取得について詳しくは、 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">シナリオ・プランナを使用するために必要なアクセス</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>シナリオ・プランナへのアクセス権以上の表示</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>プランの権限以上を表示</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、 <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">シナリオ・プランナのプランへのアクセスを要求</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## カスタム・アクセス・レベルを使用して、シナリオ・プランナへのユーザー・アクセスを構成します。

1. アクセスレベルの作成または編集を開始します ( [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 右側のオプションをクリックします。 **シナリオプランナー** をこのアクセスレベルに使用します。

   >[!NOTE]
   >
   >「要求」または「外部」のライセンス・タイプでは、シナリオ・プランナへの表示または編集アクセスは許可されません。

1. （オプション）作業中のアクセスレベルの他のオブジェクトや領域のアクセス設定を構成するには、 [Adobe Workfrontへのアクセスの設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)例： [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) および [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完了したら、「 **保存**.

## ライセンス・タイプ別シナリオ・プランナへのアクセス

各アクセス・レベルのユーザーがシナリオ・プランナで実行できる操作については、「 [シナリオプランナー領域](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) 記事内 [各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## アクセス・レベル設定によるシナリオ・プランナのアクセス

次の情報は、アクセスレベル設定を使用して、Workfrontシナリオプランナー内の情報へのユーザーのアクセスを制御する方法を理解するのに役立ちます。

* [アクセスなし](#no-access)
* [アクセスを表示](#view-access)
* [アクセスを編集](#edit-access)

### アクセスなし {#no-access}

シナリオ・プランナにアクセスできないユーザーは、レイアウト・テンプレートに追加された場合に、メイン・メニューの「シナリオ」アイコンを表示できず、また、共有されたプランやイニシアチブを表示できません。 計画へのリンクがシナリオ・プランナへのアクセス権を持たないユーザーと共有されている場合、ユーザーは計画を表示または編集できません。

### アクセスを表示 {#view-access}

シナリオ・プランナへの表示アクセス権を持つユーザーは、次の操作を実行できます。

* メインメニューの「シナリオ」アイコンを参照してください。 ![](assets/esp-icon-in-main-menu.png)に設定されますが、別のユーザーが共有するプランリンクをユーザーがクリックしない限り、「プラン」領域は空になります。
* 別のユーザーがリンクを共有した場合に、プランを表示します。

   これには、プラン内の任意の役割情報が含まれます。

   また、受信者ユーザーが財務データにもアクセスできる場合は、ジョブの役割率とプランのコスト情報も含まれます。 詳しくは、 [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### アクセスを編集 {#edit-access}

「シナリオ・プランナの編集」アクセス権を持つユーザーは、次の操作を実行できます。

* メインメニューの「シナリオ」アイコンを参照してください。 ![](assets/esp-icon-in-main-menu.png) プランデータにアクセスする場合に使用します。
* プランを作成します。
* 作成したプランを表示、編集、削除します。
* 共有リンクを使用してアクセスした他のユーザーのプランを表示、編集、削除します。

   これには、プラン内の任意の役割情報が含まれます。

   また、受信者ユーザーが財務データにアクセスできる場合は、プランに関する役割率とコスト情報も含まれます。 詳しくは、 [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
