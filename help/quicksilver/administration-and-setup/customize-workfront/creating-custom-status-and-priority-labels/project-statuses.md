---
title: システムプロジェクトステータスのリストへのアクセス
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: ユーザーはプロジェクトのステータスを指定して、他のユーザーが特定の時点でのプロジェクトの現在の開発ステージを表示できるようにします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 92%

---

# システムプロジェクトステータスのリストへのアクセス

ユーザーはプロジェクトのステータスを指定して、他のユーザーが特定の時点でのプロジェクトの現在の開発ステージを表示できるようにします。

Workfront には、9 つのシステムプロジェクトステータスがあります。これらのステータスの名前は変更できますが、削除はできません。

また、組織のニーズに合わせて、カスタムプロジェクトステータスを追加することもできます。

Workfront 管理者が、システム内のすべての新規プロジェクトのデフォルトステータスを設定します。 手順については、[システム全体のプロジェクト環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

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
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## プロジェクトのステータスへのアクセス

Workfront 管理者は、システムレベルのプロジェクトステータスのリストにアクセスできます。

システムステータスの編集とカスタムステータスの作成について詳しくは、[ステータスを作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. **プロジェクト環境設定**／**ステータス**&#x200B;をクリックします。

1. 「**プロジェクト**」タブをクリックします。

   Workfront で使用できるプロジェクトステータスがこのタブに表示されます。

   ![](assets/project-status.png)

   組み込みの各システムプロジェクトのステータスについて詳しくは、 [システムプロジェクトのステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## カスタムプロジェクトステータスを作成およびシステムステータスをカスタマイズ

Workfront 管理者は、システムプロジェクトのステータスを Workfront に追加できます。 グループの所有者は、1 つのグループに固有のカスタムステータスを追加できます。 カスタムステータスの作成やシステムステータスの編集について詳しくは、[ステータスを作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

カスタムプロジェクトステータスを作成する場合は、常に新規ステータスを既存のシステムステータスと同じにする必要があります。 カスタムステータスをどのステータスとみなすのが適切かを知るには、システムステータスの動作を理解する必要があります。 同じステータスを選択した後は、この選択を変更することはできません。 システムプロジェクトのステータスの詳細については、 [システムプロジェクトのステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
