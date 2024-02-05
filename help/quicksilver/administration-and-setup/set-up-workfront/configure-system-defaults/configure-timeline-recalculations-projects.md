---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: プロジェクトのタイムライン再計算を設定
description: タイムラインを再計算すると、管理者は、プロジェクトの外部の力がプロジェクトのタイムラインに与える影響を確認できます。プロジェクトのタイムラインとは、プロジェクトの予定日と見込み日のことです。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 84%

---

# プロジェクトのタイムライン再計算を設定

タイムラインを再計算すると、管理者は、プロジェクトの外部の力がプロジェクトのタイムラインに与える影響を確認できます。プロジェクトのタイムラインとは、プロジェクトの予定日と見込み日のことです。

[!DNL Adobe Workfront] 管理者は、システム内のすべてのプロジェクトのタイムラインを手動で再計算できます。 プロジェクトの所有者は、個々のプロジェクトのタイムラインを手動で再計算することもできます。詳しくは、[プロジェクトタイムラインの再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)を参照してください。

この記事では、[!DNL Workfront] 管理者として、[!UICONTROL 設定]エリアでプロジェクトの環境設定を行うことで、[!DNL Workfront] プロジェクトのタイムラインを自動計算する方法とタイミングの決定方法について説明します。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者のアクセスレベル</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自動再計算の設定

[!DNL Adobe Workfront] 管理者は、[!DNL Workfront] がプロジェクトタイムラインの自動再計算するタイミングを設定できます。[!DNL Workfront] では、毎晩、またはプロジェクトの範囲が変更されたとき、あるいはその両方に対して、プロジェクトのタイムラインを再計算できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) を右上に配置するか、 [!UICONTROL **メインメニュー**] アイコン ![](assets/lines-main-menu.png) 左上隅に [!DNL Workfront]（使用可能な場合）、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. **[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL プロジェクト]をクリックします。**

1. 「**[!UICONTROL タイムライン]**」セクションで、以下の設定のいずれかまたは両方を有効または無効にします。デフォルトでは、両方の設定が有効になっています。

   * **毎晩：** [!DNL Workfront&#x200B;&#x200B;&#x200B;] ステータスが「 」のプロジェクトの場合のみ、24 時間に 1 回、夜間にタイムラインを再計算します。 [!UICONTROL 現在] そしてそれは過去 3 ヶ月で更新された システム負荷やその他の要因によっては、再計算時間が 24 時間以上遅れる場合があります。

     この場合、[!DNL Workfront] は[!UICONTROL 更新タイプ]が[!UICONTROL 自動]または[!UICONTROL 自動および変更時]のすべてのプロジェクトのタイムラインを再計算します。

   * **プロジェクトのスコープが変更されたとき**：プロジェクトスコープの変更を構成する要素について詳しくは、[プロジェクトタイムラインの再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)を参照してください。

     この場合、[!DNL Workfront] は更新タイプが[!UICONTROL 自動/変更時]または[!UICONTROL 変更時のみ]のプロジェクトのタイムラインを再計算します。
プロジェクトの更新タイプの詳細については、[プロジェクト更新タイプの概要](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)を参照してください。

1. 「**[!UICONTROL 保存]**」をクリックします。

   システム内のすべてのプロジェクトのタイムラインは、各プロジェクトの「更新の種類」に基づいて自動的に再計算されます。

## [!DNL Workfront] インスタンス全体のタイムラインの再計算

[!UICONTROL タイムラインを再計算]の診断を実行し、[!DNL Workfront] システム内で手動ですべてを再計算することができます。これにより、すべてのプロジェクトマネージャーは、予定日と見込み日の両方に対する外部の変更の影響を即座に確認できます。詳しくは、[診断を使用した自動プロセスの実行](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)を参照してください。
