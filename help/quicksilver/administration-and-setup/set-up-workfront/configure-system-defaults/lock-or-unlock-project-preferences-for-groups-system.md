---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します
description: 組織内のグループでは、一意のワークフローに対して異なる設定をおこなったプロジェクト環境設定が必要になる場合があります。 組織全体のすべてのグループの環境設定のロックを解除して、グループが自分で設定できるようにすることができます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します

組織内のグループでは、一意のワークフローに対して異なる設定をおこなったプロジェクト環境設定が必要になる場合があります。 組織全体のすべてのグループの環境設定のロックを解除して、グループが自分で設定できるようにすることができます。

プリファレンスのロックが解除され、グループ管理者が変更すると、グループに関連付けられたプロジェクトは、システムレベルの設定ではなく、グループレベルの設定からそのプリファレンスの設定を取得します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ロックおよびロック解除の環境設定について

システムレベルで設定したプロジェクト、タスク、または問題の環境設定をロックすると、すべてのユーザーが同じ設定をその環境設定に使用するようになります。 ロックした環境設定は再構成できますが、グループ管理者はグループの環境設定を再構成できません。

反対に、プロジェクト、タスク、または問題の環境設定をロック解除すると、グループ管理者は、グループがそれらの項目に対してどのように機能するかを柔軟に管理できます。 プリファレンスをロック解除すると、グループ管理者はそのプリファレンスをグループ用に再設定できます。

システムレベルのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する手順については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>次の後： [!DNL Workfront] 管理者は、システムレベルでプリファレンスのロックを解除し、任意のグループ管理者が設定を行い、そのグループと以下のサブグループの全員が同じ設定を使用するようにロックできます。 これは、 [!DNL Workfront] 管理者は、システム内のすべてのユーザーに対して環境設定を設定およびロックする必要があります。 詳しくは、 [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) および [サブグループのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## プロジェクトの環境設定をロック解除して、グループが設定できるようにします

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL プロジェクト環境設定]**&#x200B;を選択し、「 **[!UICONTROL プロジェクト]**.

1. 次のいずれかの操作を行います。

   * グループ管理者がグループの環境設定を構成できるようにするには、グループのロックを解除します ![](assets/unlock-toggle-button.png).
   * すべてのグループで環境設定を使用する場合は、設定がロックされていることを確認します（デフォルト）。

      >[!IMPORTANT]
      >
      >ロックされた環境設定を構成する際にすべてのニーズが考慮されるように、システム全体の管理者やグループ内のユーザーとコミュニケーションを取ることをお勧めします。 ロックすると、その設定がシステム内のすべてのグループに継承されます。 また、環境設定のロックが一定期間解除されている場合は、グループ管理者が行った設定がその設定に置き換えられます。

1. 「**[!UICONTROL 保存]**」をクリックします。
