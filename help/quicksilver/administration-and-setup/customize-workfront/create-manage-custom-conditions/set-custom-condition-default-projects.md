---
title: カスタム条件をプロジェクトのデフォルトとして設定
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: プロジェクトの状況タイプが「手動」ではなく「進行ステータス」に設定されている場合、「プロジェクト条件と条件タイプの概要」で説明されているとおり、Adobe Workfront はプロジェクトの進行に応じて、プロジェクトの 3 つの組み込みのデフォルト条件（「目標どおり」、「危険あり」、または「トラブル発生中」）のいずれかを自動的に表示します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 93%

---

# カスタム条件をプロジェクトのデフォルトとして設定する

プロジェクトの状況タイプが「手動」ではなく「進行ステータス」に設定されている場合、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)で説明されているとおり、Adobe Workfront はプロジェクトの進行に応じて、プロジェクトの 3 つの組み込みのデフォルト状況（「目標どおり」、「危険あり」、または「トラブル発生中」）のいずれかを自動的に表示します。

![](assets/condition-in-project-header-nwe.png)

これら 3 つの組み込みのデフォルト条件を使用する代わりに、カスタム条件をデフォルト条件として設定できます。例えば、オンターゲットのデフォルト条件を変更して、すべてのプロジェクトでトラッキングウェルとして表示することができます。

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
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタム条件をすべてのプロジェクトのデフォルト条件として設定します。

{{step-1-to-setup}}

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

1. 「**プロジェクト**」タブをクリックします。
1. 「**デフォルトの条件をセット**」をクリックします。
1. 変更するデフォルト条件の横にあるドロップダウンメニューで、代わりに使用するカスタム条件をクリックします。
1. 変更する他のデフォルト条件については、前の手順を繰り返します。
1. 「**保存**」をクリックします。

タスクとイシューのデフォルト条件としてカスタム条件を設定する方法については、[タスクとイシューのデフォルトとしてカスタム条件を設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)を参照してください。

ユーザーがプロジェクトの条件を手動で更新できるようにプロジェクトを設定する方法については、[タスクとイシューの条件を更新](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)を参照してください。

カスタム条件について詳しくは、[カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)を参照してください。
