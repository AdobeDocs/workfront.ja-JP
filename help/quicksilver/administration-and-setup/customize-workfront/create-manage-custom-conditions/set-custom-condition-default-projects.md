---
title: カスタム条件をプロジェクトのデフォルトとして設定
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: プロジェクトの状況タイプが「手動」ではなく「進行ステータス」に設定されている場合、「プロジェクト条件と条件タイプの概要」で説明されているとおり、Adobe Workfront はプロジェクトの進行に応じて、プロジェクトの 3 つのビルトインのデフォルト条件（「目標どおり」、「危険あり」、または「トラブル発生中」）のいずれかを自動的に表示します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 73%

---

# カスタム条件をプロジェクトのデフォルトとして設定する

プロジェクトの状況タイプが「手動」ではなく「進行ステータス」に設定されている場合、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)で説明されているとおり、Adobe Workfront はプロジェクトの進行に応じて、プロジェクトの 3 つのビルトインのデフォルト状況（「目標どおり」、「危険あり」、または「トラブル発生中」）のいずれかを自動的に表示します。

![ プロジェクトヘッダーおよび詳細の条件 ](assets/condition-of-project-0825.png)

これら 3 つのビルトインのデフォルト条件を使用する代わりに、カスタム条件をデフォルト条件として設定できます。例えば、オンターゲットのデフォルト条件を変更して、すべてのプロジェクトでトラッキングウェルとして表示することができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタム条件をすべてのプロジェクトのデフォルト条件として設定します。

{{step-1-to-setup}}

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

1. 「**プロジェクト**」タブをクリックします。
1. 「**デフォルトの条件を設定**」をクリックします。
1. 変更する既定の条件のドロップダウン メニューで、代わりに使用するカスタム条件をクリックします。
1. 変更する他のデフォルト条件については、前の手順を繰り返します。
1. 「**保存**」をクリックします。

タスクとイシューのデフォルト条件としてカスタム条件を設定する方法については、[タスクとイシューのデフォルトとしてカスタム条件を設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)を参照してください。

ユーザーが手動で条件を更新できるプロジェクトの設定については、[ タスクおよび問題の条件の更新 ](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md) を参照してください。
