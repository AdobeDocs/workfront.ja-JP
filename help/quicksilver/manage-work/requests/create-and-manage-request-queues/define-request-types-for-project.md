---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: プロジェクトの要求タイプの定義
description: Adobe Workfront に記録されるイシューやリクエストの種類を、リクエストタイプごとに整理できます。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 64%

---

# プロジェクトのリクエストタイプの定義

<!-- Audited: 6/2025 -->

Adobe Workfront に記録されるイシューやリクエストの種類を、リクエストタイプごとに整理できます。 これは、理由を報告したり、プロジェクトのライフタイム中にどのような予期しない作業が発生するかをユーザーが理解するのに役立ちます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
    <p>標準</p>
    <p>プラン</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対して権限を管理</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

始める前に、以下を行う必要があります。

* プロジェクトを作成または持っている。

  プロジェクトの作成について詳しくは、[プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md)を参照してください。

## リクエストタイプに関する考慮事項

* プロジェクトの「キューの詳細」領域を設定する際に、プロジェクトに記録できるイシューまたはリクエストのタイプを指定できます。
* プロジェクトのリクエストタイプを定義できるようにするために、プロジェクトをリクエストキューとして有効にする必要はありません。 プロジェクトに関して記録されるイシューには、別のリクエストタイプのラベルを付けることができます。
* プロジェクトにキュートピックを追加する場合、新しいイシューやリクエストを追加するときに表示されるように、それぞれのキュートピックでリクエストタイプを定義する必要があります。 詳しくは、[キュートピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

## プロジェクトのイシュータイプまたはリクエストタイプを定義

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。
1. 左側のパネルで、「**キューの詳細**」をクリックします。
1. 「**キューのプロパティ**」セクションで、プロジェクトに必要な&#x200B;**リクエストタイプ**&#x200B;を選択します。
   * バグレポート
   * 変更依頼
   * イシュー
   * リクエスト

   >[!NOTE]
   >
   >* 少なくとも 1 つのリクエストタイプを選択する必要があります。 複数のタイプを選択できます。
   >* Workfront 管理者が、これらのオプションの一部の名前を変更している可能性があります。 詳しくは、[リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)を参照してください。

1. 「**保存**」をクリックします。 指定したリクエストタイプは、タスクまたはプロジェクトに新しいイシューを入力する場合、またはプロジェクトに新しいリクエストを送信する場合（プロジェクトがリクエストキューとして有効になっている場合）に選択できます。
