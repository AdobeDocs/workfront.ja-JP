---
navigation-topic: financials
title: 請求記録の作成
description: 収益および追跡の費用を設定することに加えて、請求する必要のある情報に関する請求記録をプロジェクトに作成できます。
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 97%

---

# 請求記録の作成

収益および追跡の費用を設定することに加えて、請求する必要のある情報に関する請求記録をプロジェクトに作成できます。

タスクの請求記録は作成できません。請求記録を作成できるのは、プロジェクトの場合のみです。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>プロジェクトおよび財務データへのアクセスを編集する</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>財務を管理する権限を持つプロジェクトに対する権限の管理</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 請求記録の概要

請求記録は、プロジェクトの添付ファイルとして作成され、プロジェクトの財務データとプロジェクトのタスクの財務情報が含まれます。

請求記録の使用を計画する際は、次の点を考慮してください。

* 請求記録は、プロジェクトに関連する金額を外部のベンダーまたはパートナーに請求する場合に作成します。外部ソースに固定金額を請求する以外に、（ログに記録された時間から）プロジェクトの作業量を外部請負業者に請求する必要がある場合や費用や固定収益の額を請求する必要がある場合があります。この情報をすべて同じ請求記録に含めることができます。
* 請求記録が請求済みに設定されると、編集できなくなります。

  >[!IMPORTANT]
  >
  >請求料率が変化する状況で、プロジェクトの収益と費用の情報をロックする場合、このことは重要です。請求記録に追加して請求済みとしてマークすると、システムで請求料率が更新されても、収益は更新されません。

* 請求済みとマークされた請求記録を含むプロジェクトは削除できません。

## 請求記録の作成

1. プロジェクトに移動します。
1. 左側のパネルで「**請求記録**」をクリックします。
1. 左側のパネルで「**請求記録の詳細**」を選択した場合、「**新規請求記録**」をクリックします。
1. 表示される「**新規請求記録**」ボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>必須フィールドです。請求記録の説明を指定して、この記録の目的または意図を反映します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">請求ステータス</td> 
      <td> <p>この記録がまだ請求されていない場合、「<strong>未請求</strong>」を選択します。</p> <p>請求記録が請求済みの場合、「<strong>請求済み</strong>」を選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">請求日</td> 
      <td>カレンダーアイコンをクリックして、この請求記録の請求日を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">PO 番号</td> 
      <td>この請求記録に PO 番号が関連付けられている場合は、このフィールドにこの情報を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">インボイス ID</td> 
      <td>この請求記録に関連付けられている請求書がある場合は、このフィールドでこの情報を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">追加金額</td> 
      <td>請求記録の固定金額を入力します。これは、このプロジェクトの外部顧客、請負業者またはパートナーに請求する金額です。請求記録のステータスが請求済みに変更された後は、この金額を変更できません。</td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「**カスタムフォーム**」の下で、請求記録に追加する請求記録カスタムフォームを選択します。

   ここで選択する前に、自分で（またはカスタムフォームへのアクセス権を持つその他のユーザーが）請求記録のカスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

   この手順を繰り返して、請求記録に必要な他のカスタムフォームを追加できます。

1. 「**保存**」をクリックします。

   請求記録が作成されます。請求記録に請求可能時間、費用、固定収益を含めるには、次の小節で説明する手順に従います。

## 請求記録に請求可能時間、費用、固定収益を含める

* [請求記録に請求可能時間を含める](#include-billable-hours-in-a-billing-record)
* [請求記録に請求可能費用を含める](#include-billable-expenses-in-a-billing-record)
* [請求記録に固定収益を含める](#include-fixed-revenues-in-a-billing-record)

### 請求記録に請求可能時間を含める {#include-billable-hours-in-a-billing-record}

請求記録には、ログオンしたタスク、イシューまたはプロジェクトに関する時間を含めることができます。\
時間またはプライマリ担当業務を記録するユーザーが 1 時間当たりの請求率に関連付けられている場合、これらの時間からの収益が請求記録に追加されます。

* [請求記録に追加できる時間数](#what-hours-can-be-added-to-a-billing-record)
* [請求記録への時間の追加](#add-hours-to-a-billing-record)

#### 請求記録に追加できる時間数 {#what-hours-can-be-added-to-a-billing-record}

次の条件を満たした場合、請求記録に時間を追加できます。

* タスク、イシュー、またはプロジェクトに時間が記録されています。
* 記録される時間のタイプは、収益としてカウントされます。

  時間タイプについて詳しくは、[時間タイプの管理](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)の記事を参照してください。

* 時間を記録するユーザーが、ユーザーまたはプライマリ担当業務に関連付けられている 1 時間あたりの請求率を適用した場合、イシューまたはプロジェクトに対して記録された、すべての時間を請求記録に追加できます。
* タスクの時間を記録している場合、タスクの収益タイプは次のようになります。

   * 収益タイプを「請求不可」に設定することはできません。
   * 収益タイプが「ユーザー（毎時）」に設定されている場合、時間を記録するユーザーのプロファイルには、1 時間あたりの請求率が設定されている必要があります。
   * 収益タイプが役割（時間単位）に設定されている場合、時間を記録するユーザーのプライマリ役割に、1 時間あたりの請求率を適用する必要があります。

     >[!NOTE]
     >
     >プロジェクトレベルで、担当業務の請求率を上書きできます。\
     >担当業務の請求率の上書きについて詳しくは、[担当業務に対する請求率の上書きとプロジェクトにおける収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)の記事の「プロジェクトレベルで担当業務の請求率を上書き」の節を参照してください。

* 「プロジェクトの設定」の下で「**プロジェクト時間の承認**」がオンになっている場合は、プロジェクト所有者は記録された時間を承認する必要があります。\
  プロジェクト時間に対して承認を要求する方法について詳しくは、[プロジェクト時間の承認](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md)の記事を参照してください。

#### 請求記録への時間の追加 {#add-hours-to-a-billing-record}

請求記録に請求可能時間を追加する手順は、次のとおりです。

1. 請求記録を含むプロジェクトに移動します。
1. 左側のパネルにある「**請求記録**」をクリックします。
1. 請求記録の「**説明**」をクリックして、「**請求記録の詳細**」タブを開きます。
1. 左側のパネルにある「**請求可能時間**」をクリックします。
1. 請求記録に含まれる可能性のある時間数がある場合は、「**時間を追加**」をクリックします。\
   **請求可能時間を追加**&#x200B;ボックスが開きます。

   >[!NOTE]
   >
   >時間が記録されていない場合、または記録された時間が請求記録に追加する必要のある条件を満たしていない場合、「**時間を追加**」ボタンは表示されません。請求記録に記録できる時間について詳しくは、この記事の[請求記録に追加できる時間](#what-hours-can-be-added-to-a-billing-record)の節を参照してください。

1. 請求記録に含める時間エントリを選択し、「**時間を追加**」をクリックします。\
   時間の実際のコストは、**請求可能時間**&#x200B;数として&#x200B;**請求記録合計**&#x200B;に追加されます。

1. （オプション）「**請求記録の詳細**」をクリックして、**請求可能時間**&#x200B;および&#x200B;**請求記録合計**&#x200B;の値を確認します。請求記録のヘッダーで請求記録の合計を確認できます。

### 請求記録に請求可能費用を含める {#include-billable-expenses-in-a-billing-record}

請求記録に請求可能費用を追加する場合は、タスクの費用とプロジェクトの費用が請求可能としてマークされていることを確認します。請求可能とマークされていない費用は、請求記録に追加できません。費用の追加について詳しくは、[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)の記事を参照してください。

請求記録に請求可能費用を追加する手順は、次のとおりです。

1. 請求記録を含むプロジェクトに移動します。
1. 左側のパネルにある「**請求記録**」をクリックします。
1. 請求記録の「**説明**」をクリックして、「**請求記録の詳細**」タブを開きます。
1. 左側のパネルにある「**請求可能費用**」をクリックします。
1. （条件付き）タスクまたはプロジェクトに費用を追加し、請求可能とマークしている場合は、「**費用を追加**」をクリックします。

   >[!NOTE]
   >
   >費用が含まれていても、請求可能としてマークされていない場合、「**費用を追加**」ボタンは表示されません。請求記録に含めることができるのは、実際の金額が 0 より大きい請求可能な費用のみです。

1. 請求記録に追加できる請求可能費用を選択し、「**費用を追加**」をクリックします。\
   費用の実際の金額は、**請求可能費用**&#x200B;の金額として&#x200B;**請求記録合計**&#x200B;に追加されます。

1. （オプション）「**請求記録の詳細**」をクリックして、**請求可能費用**&#x200B;および&#x200B;**請求記録合計**&#x200B;の金額を確認します。請求記録のヘッダーで請求記録の合計を確認できます。

### 請求記録に固定収益を含める {#include-fixed-revenues-in-a-billing-record}

固定収益を利用できるタスクがある場合は、固定収益を請求記録に追加できます。他のタイプのタスクまたはプロジェクト収益は、請求記録に追加できません。収益タイプについて詳しくは、[請求と収益の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)の記事で[請求と収益の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)の節を参照してください。

請求記録に固定収益を追加するには、次の手順に従います。

1. 請求記録を含むプロジェクトに移動します。
1. 左側のパネルにある「**請求記録**」をクリックします。
1. 請求記録の「**説明**」をクリックして、「**請求記録の詳細**」タブを開きます。
1. 「**固定収益**」タブをクリックします。
1. タスクに固定収益を追加した場合は、「**固定収益を追加**」をクリックします。

   >[!NOTE]
   >
   >タスクに収益金額が含まれていても、それらが「固定」とマークされていない場合、「**固定収益を追加**」ボタンは表示されません。

1. 固定収益を請求記録に含めるタスクを選択し、「**タスクを追加**」をクリックします。\
   タスクの&#x200B;**固定収益**&#x200B;の金額が&#x200B;**請求可能な収益**&#x200B;の金額として&#x200B;**請求記録合計**&#x200B;に追加されます。

1. （オプション）「**請求記録の詳細**」をクリックして、**請求可能な収益**&#x200B;および&#x200B;**請求記録合計**&#x200B;の金額を確認します。請求記録のヘッダーで請求記録の合計を確認できます。

## 請求記録の編集

請求記録を作成し、請求記録に時間、費用、収益を含めた後、請求済みとしてマークされる前に、既存の記録に関する情報を編集できます。

1. 請求記録に移動します。
1. 左側のパネルで「**請求記録の詳細**」が選択させている場合、使用可能なフィールドの情報を編集します。

   または

   右上隅の **編集アイコン**![ 編集アイコン ](assets/edit-icon.png) をクリックし、使用可能な任意のフィールドで情報を編集します。

   次を更新します。

   * **説明**
   * **請求ステータス**

     >[!TIP]
     >
     >請求ステータスで「**請求済み**」を選択した場合、変更を保存した後は請求記録を編集できません。

   * **請求日**
   * **PO 番号**
   * **インボイス ID**
   * **追加金額**

   次のフィールドは編集できません。

   * **請求可能時間：** 請求記録に含まれる時間の実収益の合計。請求記録に時間を含める方法について詳しくは、この記事の[請求記録に請求可能時間を含める](#include-billable-hours-in-a-billing-record)を参照してください。

   * **請求可能な費用**：請求記録に含まれる請求可能な費用の実際の金額の合計。請求記録に請求可能な費用を含める方法について詳しくは、[請求記録に請求可能費用を含める](#include-billable-expenses-in-a-billing-record)の節を参照してください。

   * **請求可能な費用**：請求記録に含まれるタスクの固定収益の合計。請求記録に固定収益を含める方法について詳しくは、[請求記録に固定収益を含める](#include-fixed-revenues-in-a-billing-record)の節を参照してください。

   * **請求記録合計**：すべての請求可能額の合計。これは次の数式で計算されます。

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. 「**&#x200B;**&#x200B;**変更を保存**」をクリックします。
