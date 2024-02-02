---
title: カスタム条件をプロジェクトのデフォルトとして設定する
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: プロジェクトの状況タイプが「手動」ではなく「進行ステータス」に設定されている場合、「プロジェクト条件と条件タイプの概要」で説明されているとおり、Adobe Workfront はプロジェクトの進行に応じて、プロジェクトの 3 つの組み込みのデフォルト条件（「目標どおり」、「危険あり」、または「トラブル発生中」）のいずれかを自動的に表示します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '352'
ht-degree: 100%

---

# カスタム条件をプロジェクトのデフォルトとして設定する

プロジェクトの状況タイプが「手動」ではなく「進行ステータス」に設定されている場合、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)で説明されているとおり、Adobe Workfront はプロジェクトの進行に応じて、プロジェクトの 3 つの組み込みのデフォルト状況（「目標どおり」、「危険あり」、または「トラブル発生中」）のいずれかを自動的に表示します。

![](assets/condition-in-project-header-nwe.png)

これら 3 つの組み込みのデフォルト条件を使用する代わりに、カスタム条件をデフォルト条件として設定できます。例えば、オンターゲットのデフォルト条件を変更して、すべてのプロジェクトでトラッキングウェルとして表示することができます。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタム条件をすべてのプロジェクトのデフォルト条件として設定します。

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**設定** ![](assets/gear-icon-settings.png)」の順にクリックします。

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

1. 「**プロジェクト**」タブをクリックします。
1. 「**デフォルトの条件をセット**」をクリックします。
1. 変更するデフォルト条件の横にあるドロップダウンメニューで、代わりに使用するカスタム条件をクリックします。
1. 変更する他のデフォルト条件については、前の手順を繰り返します。
1. 「**保存**」をクリックします。

タスクとイシューのデフォルト条件としてカスタム条件を設定する方法については、[タスクとイシューのデフォルトとしてカスタム条件を設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)を参照してください。

ユーザーがプロジェクトの条件を手動で更新できるようにプロジェクトを設定する方法については、[タスクとイシューの条件を更新](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)を参照してください。

カスタム条件について詳しくは、[カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)を参照してください。
