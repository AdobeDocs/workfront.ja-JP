---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: プロジェクトのリクエストタイプを定義
description: Adobe Workfront に記録されるイシューやリクエストの種類を、リクエストタイプごとに整理できます。
author: Becky
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 55%

---

# プロジェクトのリクエストタイプの定義

<!-- Audited: 6/2025 -->

Adobe Workfrontに記録されるイシューやリクエストの種類を、リクエストタイプ別に整理できます。 これは、理由をレポートし、プロジェクトの有効期間中に発生する可能性のある予期しない作業の種類をユーザーが理解するのに役立ちます。

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

* プロジェクトを作成する。

  プロジェクトの作成について詳しくは、[プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md)を参照してください。

## リクエストタイプに関する考慮事項

* プロジェクトの「キューの詳細」領域を設定する際に、プロジェクトに記録できるイシューまたはリクエストのタイプを指定できます。
* プロジェクトのリクエストタイプを定義できるようにするために、プロジェクトをリクエストキューとして有効にする必要はありません。プロジェクトに関して記録されるイシューには、別のリクエストタイプのラベルを付けることができます。
* プロジェクトにキュートピックを追加する場合、新しいイシューやリクエストを追加するときに表示されるように、それぞれのキュートピックでリクエストタイプを定義する必要があります。詳しくは、[キュートピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

## プロジェクトのイシュータイプまたはリクエストタイプを定義

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。
1. 左側のパネルで、「**キューの詳細**」をクリックします。
1. 「**キューのプロパティ**」セクションで、プロジェクトに必要な **リクエストタイプ** を選択します。
   * バグレポート
   * 変更依頼
   * イシュー
   * リクエスト

   >[!NOTE]
   >
   >* 少なくとも 1 つのリクエストタイプを選択する必要があります。複数のタイプを選択できます。
   >* Workfront 管理者が、これらのオプションの一部の名前を変更している可能性があります。詳しくは、[リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)を参照してください。

1. 「**保存**」をクリックします。指定した要求タイプは、タスクまたはプロジェクトに新しい問題を入力するとき、またはプロジェクトに新しい要求を送信するとき（プロジェクトが要求キューとして有効になっている場合）に選択できます。
