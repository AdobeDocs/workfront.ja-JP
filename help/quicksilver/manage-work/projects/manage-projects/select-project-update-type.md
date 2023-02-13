---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトの更新タイプを選択
description: プロジェクトの [ 更新の種類 ] を選択すると、プロジェクトのタイムラインに加えた変更が親タスクまたはプロジェクトに保存される頻度を制御できます。
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# プロジェクトの更新タイプを選択

プロジェクトの [ 更新の種類 ] を選択すると、プロジェクトのタイムラインに加えた変更が親タスクまたはプロジェクトに保存される頻度を制御できます。

プロジェクトタイムラインを更新すると、プロジェクト、タスク、またはタイムラインが依存する別のプロジェクトに対して行われた変更に基づいてプロジェクトタイムラインが再計算されます。

例えば、プロジェクトトリガー上のタスクに対して次の変更を加え、プロジェクトのタイムラインに対する更新を行います。

* タスクの日付を更新
* タスクの先行関係の変更
* タスクの制約や期間の種類の変更に加えて、親子関係を変更し、割り当てを追加または削除します。

## アクセス要件

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトの更新タイプの更新

タスクが更新されると、親オブジェクト（親タスクまたはプロジェクト）は、[ 更新の種類 ] で示された時点で更新されます。  プロジェクトの更新タイプを指定するには：

1. 更新タイプを指定するプロジェクトに移動します。
1. その他メニューをクリックします。 ![](assets/more-icon.png) プロジェクト名の横にあるをクリックし、 **編集** .

1. クリック  **プロジェクト** **設定**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. 内 **更新タイプ** [ ] フィールドで、変更があったときにWorkfrontが自動的にプロジェクトのタイムラインを毎日計算するか、またはプロジェクトマネージャが手動で計算するかを選択します。

   以下のリストのオプションから「 」を選択します。 

   >[!IMPORTANT]
   >
   >プロジェクトのタイムラインが 15 年を超える場合、Workfrontは自動的にも変更時にもタイムラインを計算しません。 15 年を超えるプロジェクトの更新タイプは、常に手動です。

   * **自動および変更時：** これはデフォルト設定です。 プロジェクトタイムラインは、プロジェクト内またはタイムラインが依存する別のプロジェクト内で変更が発生するたびに更新されます。 プロジェクトのタイムラインも毎晩更新されます。 \
      これは、プロジェクトタイムラインが常に最新であることを確認するので、推奨される設定です。

      タスクまたはプロジェクトを更新し、タイムラインの再計算をトリガーすると、使用可能なすべての日付が直ちに表示され、作業を続行できます。 タスクが 100 を超えるプロジェクトでは、長い計算が必要な日付は淡色表示になります。

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      これは、再計算がまだ完了しておらず、日付が変更される可能性があることを示しています。

   * **変更のみ：** プロジェクトタイムラインは、プロジェクト内またはタイムラインが依存する別のプロジェクト内で変更が発生するたびに更新されます。スケジュールされた更新は行われません。\
      システムのパフォーマンスを気にする場合や、プロジェクト内や、タイムラインが依存する他のプロジェクト内で変更がほとんど発生しない場合は、このオプションを選択できます。

   * **自動のみ：** プロジェクトのタイムラインは毎晩更新され、変更を加えた後、直ちに更新されることはありません。\
      システムのパフォーマンスを気にする場合や、プロジェクト内またはタイムラインが依存する他のプロジェクト内で毎日多くの変更が発生する場合は、このオプションを選択します。

      >[!NOTE]
      >
      >Planning ステータスの場合、プロジェクトは毎晩自動的に再計算されません。 変更時に再計算されるだけです。

   * **手動のみ：** プロジェクトタイムラインは、「 **タイムラインを再計算**（この記事の「手動再計算」の節で説明） [プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      一度に多くの変更を加え、個々の変更の後ではなく、すべての変更が行われた後にタイムラインの再計算を行う場合は、このオプションを選択します。

1. 「**保存**」をクリックします。
