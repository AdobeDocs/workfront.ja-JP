---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクト更新タイプの概要
description: プロジェクトの更新タイプは、Adobe Workfront がプロジェクトのタイムラインを計算する方法を示します。プロジェクトプランの変更により、プロジェクトのトリガーが変更される場合があります。これらの変更を取り入れた最新の状態に保つには、プロジェクトのタイムラインを自動または手動で再計算する必要があります。
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 100%

---

# プロジェクト更新タイプの概要

プロジェクトの更新タイプは、Adobe Workfront がプロジェクトのタイムラインを計算する方法を示します。プロジェクトプランの変更により、プロジェクトのトリガーが変更される場合があります。これらの変更を取り入れた最新の状態に保つには、プロジェクトのタイムラインを自動または手動で再計算する必要があります。

プロジェクトタイムラインの再計算について詳しくは、[プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)を参照してください。

## プロジェクト更新タイプ

プロジェクトには、Workfront でプロジェクトタイムラインを再計算するタイミングに応じて、4 つの更新タイプがあります。更新タイプは以下のリストから選択します。

プロジェクトの更新タイプを更新する方法について詳しくは、[プロジェクト更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。

>[!IMPORTANT]
>
>プロジェクトのタイムラインが 15 年を超える場合、Workfront は自動的にも変更時にもタイムラインを計算しません。15 年を超えるプロジェクトの更新タイプは、常に手動です。

* **自動・変更時：**&#x200B;これはデフォルトの設定です。プロジェクトのタイムラインは、プロジェクト内またはタイムラインが依存する別のプロジェクト内で変更が発生するたびに更新されます。また、プロジェクトのタイムラインは毎晩更新されます。\
  これは、プロジェクトタイムラインが常に最新であることが保証されるので、推奨される設定です。

  タスクまたはプロジェクトを更新し、タイムラインの再計算をトリガーすると、利用可能なすべての日付が直ちに表示され、作業を続行できます。タスクが 100 を超えるプロジェクトでは、計算に時間がかかる日付は淡色表示になります。

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

  これは、再計算がまだ完了しておらず、日付が変更される可能性があることを示しています。

* **変更時のみ：**&#x200B;プロジェクトのタイムラインは、プロジェクト内またはタイムラインが依存する別のプロジェクト内で変更が発生するたびに更新されます。スケジュールされた更新は行われません。\
  システムのパフォーマンスが気になる場合や、プロジェクト内またはタイムラインが依存する他のプロジェクト内で変更がほとんど発生しない場合は、このオプションを選択するのがよいです。

* **自動のみ：**&#x200B;プロジェクトのタイムラインは毎晩更新され、変更が加えられた直後には更新されません。\
  システムのパフォーマンスが気になる場合や、プロジェクト内またはタイムラインが依存する他のプロジェクト内で毎日多くの変更が発生する場合は、このオプションを選択するのがよいです。

  >[!NOTE]
  >
  >計画中ステータスの場合、プロジェクトは毎晩自動的には再計算されません。変更時にのみ再計算されます。

* **手動のみ：**&#x200B;プロジェクトのタイムラインは、記事「[プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)」の「手動再計算」の節で説明されているように、「**タイムラインを再計算**」オプションを選択した場合にのみ更新されます。\
  プロジェクトに一度に多くの変更を加え、個々を変更した後ではなくすべての変更が行われた後でタイムラインの再計算を実行する場合は、このオプションを選択できます。
