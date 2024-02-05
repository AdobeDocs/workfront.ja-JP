---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 独自の為替レートを使用した財務データレポートの作成
description: Adobe Workfront で複数の為替レートが設定されている場合、レポートおよびリストの財務値をデフォルトの通貨以外の通貨で表示するように設定できます。
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 98%

---

# 独自の為替レートを使用した財務データレポートの作成

Adobe Workfront で複数の為替レートが設定されている場合、レポートおよびリストの財務値をデフォルトの通貨以外の通貨で表示するように設定できます。

>[!IMPORTANT]
>
>ビューでデフォルト通貨以外の通貨を選択すると、プロジェクトリストの下部にリンク「**タスクをさらに追加**」および「**イシューをさらに追加**」が表示されなくなります。

特定のプロジェクトのデフォルト通貨を変更する方法については、[プロジェクト通貨の変更](../../../manage-work/projects/project-finances/change-project-currency.md)を参照してください。

レポート内に単一通貨のプロジェクトがある場合、グループ内の合計もシステムのデフォルト通貨で表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

この節で説明するように代替通貨を表示するには、まず Workfront 管理者が Workfront の設定エリアで複数の通貨を有効にして設定する必要があります。詳細については、[為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。

## 財務値をレポートに適用する {#apply-financial-values-to-a-report}

レポートを操作するときに通貨間の財務値を変換するには、次の手順を実行します。

1. 財務値を別の通貨に変換するレポートに移動します。
1. **表示**&#x200B;ドロップダウンリストをクリックし、**通貨の変更**&#x200B;を選択して、財務値を表示する次の通貨のいずれかを選択します。

   * プロジェクトの元の通貨
   * その他の通貨

     >[!TIP]
     >
     >選択できるのは、以前に設定で選択した通貨のみです。

   このオプションを使用すると、レポート内の財務値をレート値間で迅速に変換できます。

   ![通貨を変更](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## 異なる通貨を使用する複数のプロジェクトにわたってデフォルト通貨を表示する

プロジェクトレベルで通貨をカスタマイズし、すべてのプロジェクトの情報を同じレポートに表示する場合は、次のようなシナリオがあります。

* 異なる通貨が適用されている 2 つ以上のプロジェクトから財務情報を取得するレポートを作成する場合、デフォルトでは、グループ化概要には Workfront 管理者が選択したシステムのデフォルト通貨が反映されます。
* 通貨は同じでもシステムのデフォルト通貨とは異なる 2 つ以上のプロジェクトのレポートを作成する場合、グループ内の合計はシステムのデフォルト通貨を使用して表示されます。
* 通貨の上書きに関連付けられた担当業務の割り当てを持つ 2 つ以上のプロジェクトのレポートを作成する場合、Workfront は、財務情報を担当業務の上書きされた通貨レートからプロジェクトの通貨に変換するか（ビューでプロジェクトの元の通貨を選択した場合）、または、レポートの表示時に選択した別の通貨に変換します。担当業務の通貨の上書きについては、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

レポートにカスタム通貨を使用して 2 つのプロジェクトを表示するには、次の手順を実行します。

1. 異なる通貨を適用した 2 つのプロジェクトを作成します。

   ![](assets/qs-currency-350x217.png)

1. 両方のプロジェクトの作業時間を記録します。

   時間の記録の詳細については、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

1. **メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**レポート**&#x200B;の順にクリックします。
1. **新規レポート**、**プロジェクトレポート**&#x200B;の順にクリックします。
1. 「**列（ビュー）**」タブから、**実際コスト**&#x200B;列を追加し、「**合計**」で集計します。

   列の作成方法については、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

1. 「**グループ**」タブで、**予定完了日**&#x200B;のグループ化を適用します。

   グループ化の作成方法については、[Adobe Workfront のグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 「**フィルター**」タブで、**プロジェクト名**&#x200B;のフィルターを追加し、通貨が異なる 2 つのプロジェクトを選択します。

   フィルターの作成方法について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 「**保存して閉じる**」をクリックします。

   **実際のコスト**&#x200B;の合計は、レポート内のプロジェクトの通貨に関係なく、システムのデフォルト通貨を使用してグループ化に表示されます。

   ![グループ化で表示された通貨](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   2 つのプロジェクトの通貨が異なる場合、システムのデフォルト通貨もレポートのグループ化に表示されます。

## レポートにプロジェクト通貨をプロジェクトレベルで表示する

プロジェクト内のタスクまたは時間リストにグループ化が適用されている場合、グループ化の合計はプロジェクトの通貨で表示されます。

1. システムのデフォルト通貨とは異なるカスタム通貨を使用してプロジェクトを作成します。
1. プロジェクトに移動し、タスクに対して記録された時間が含まれていることを確認します。

   時間の記録の詳細については、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

   >[!NOTE]
   >
   >タスクは、時間あたりのコスト率を使用してユーザーまたは担当業務に割り当てる必要があります。

1. **タスク**&#x200B;をクリックします。
1. **表示**&#x200B;ドロップダウン メニューを展開し、**新規表示**&#x200B;を選択します。
1. **実際のコスト**&#x200B;を新しい列として新規表示に追加し、「**合計**」で集計します。
1. 「**完了**」、「**表示を保存**」の順にクリックします。
1. **グループ化**&#x200B;ドロップダウンメニューを展開し、**新しいグループ化**&#x200B;を選択します。
1. 新しいグループ化で、新しいフィールドとして「**実際の完了日**」を追加し、次に「**グループ化を保存**」をクリックします。

   **実際のコスト**&#x200B;列には、新しいグループ化の概要が表示され、プロジェクトの通貨での合計が表示されます。

## 独自の通貨でレポートを編集

レポート内の財務フィールドは、プロジェクトの元の通貨を表示するようにレポート設定を変更するまで編集できません。

レポート内の財務フィールドをインライン編集するには、次の手順に従います。

1. レポートに移動します。

   >[!NOTE]
   >
   >他のエリアのリストにデフォルトの通貨が表示されない場合は、ビューを編集してデフォルトの通貨を表示できます。\
   >ビューでの通貨の変更方法については、この記事の、[レポートへの財務値の適用](#apply-financial-values-to-a-report)の節を参照してください。

1. **レポートのアクション**&#x200B;をクリックし、次に「**編集**」を選択します。
1. **レポート設定**&#x200B;をクリックします。
1. **デフォルトの通貨**&#x200B;ドロップダウンをクリックし、**プロジェクトの元の通貨**&#x200B;を選択します。

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. 「**完了**」をクリックします。
