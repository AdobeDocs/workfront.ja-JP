---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: プロジェクトのタイムライン再計算の設定
description: タイムラインを再計算すると、管理者は、プロジェクト外の力がプロジェクトのタイムラインに与える影響を確認できます。 プロジェクトのタイムラインは、プロジェクトの計画日と予定日を指します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# プロジェクトのタイムライン再計算の設定

タイムラインを再計算すると、管理者は、プロジェクト外の力がプロジェクトのタイムラインに与える影響を確認できます。 プロジェクトのタイムラインは、プロジェクトの計画日と予定日を指します。

As a [!DNL Adobe Workfront] 管理者は、システム内のすべてのプロジェクトのタイムラインを手動で再計算できます。 プロジェクトの所有者は、個々のプロジェクトのタイムラインを手動で再計算することもできます。 詳しくは、 [プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

この記事では、 [!DNL Workfront] 管理者は、方法とタイミングを決定できます [!DNL Workfront] プロジェクトのプリファレンスを [!UICONTROL 設定] 領域

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者のアクセスレベル</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自動再計算の設定

As a [!DNL Adobe Workfront] 管理者は、次の場合に設定できます [!DNL Workfront] プロジェクトタイムラインを自動的に再計算します。 [!DNL Workfront] では、毎晩、またはプロジェクトの範囲が変更されたとき、あるいはその両方に対して、プロジェクトのタイムラインを再計算できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL プロジェクト環境設定]** > **[!UICONTROL プロジェクト].**

1. 内 **[!UICONTROL タイムライン]** セクションで、以下の設定のいずれかまたは両方を有効または無効にします。 デフォルトでは、両方の設定が有効になっています。

   * **毎晩：** [!DNL Workfront&#x200B;&#x200B;&#x200B;] ステータスが [!UICONTROL 現在] 過去 3 ヶ月間に更新された

      この場合、 [!DNL Workfront] を持つすべてのプロジェクトのタイムラインを再計算します [!UICONTROL 更新タイプ] / [!UICONTROL 自動] または [!UICONTROL 自動および変更時].

   * **プロジェクトの範囲が変更されたとき**:プロジェクト範囲の変更を構成する情報については、 [プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      この場合、 [!DNL Workfront] [ 更新の種類 ] が設定されているすべてのプロジェクトのタイムラインを再計算します [!UICONTROL 自動および変更時] または [!UICONTROL 変更時のみ].
プロジェクトの更新タイプの詳細については、 [プロジェクト更新タイプの概要](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. 「**[!UICONTROL 保存]**」をクリックします。

   システム内のすべてのプロジェクトのタイムラインは、各プロジェクトの [ 更新の種類 ] に基づいて自動的に再計算されます。

## 全体のタイムラインを再計算 [!DNL Workfront] インスタンス

次を実行できます。 [!UICONTROL タイムラインを再計算] 診断： [!DNL Workfront] システム。 これにより、すべてのプロジェクトマネージャは、計画日と予定日の両方に対する外部の変更の影響を即座に確認できます。 詳しくは、 [診断を使用して自動プロセスをトリガー化](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
