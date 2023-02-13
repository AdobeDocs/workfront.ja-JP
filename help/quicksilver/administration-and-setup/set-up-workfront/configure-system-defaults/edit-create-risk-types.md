---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: リスクタイプの編集と作成
description: 計画段階でプロジェクトにリスクを追加して、作業の承認前に潜在的な障害を特定できます。 リスクとは、時間通りに、または予算内でプロジェクトが完了するのを妨げる可能性のあるイベントです。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# リスクタイプの編集と作成

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

計画段階でプロジェクトにリスクを追加して、作業の承認前に潜在的な障害を特定できます。 リスクとは、時間通りに、または予算内でプロジェクトが完了するのを妨げる可能性のあるイベントです。

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

## リスクのタイプ

リスクタイプは、レポート目的で分類するためにリスクに使用できるラベルです。 これらは、 **[!UICONTROL 設定]** 領域 [!DNL Adobe Workfront] 管理者。 リスクタイプが **[!UICONTROL 設定]** 領域内では、システムに対して普遍的です。 プロジェクト所有者は全員、プロジェクトに同じリスクタイプを使用できます。

## リスクタイプの編集と作成

一部のリスクタイプは既にに存在します [!DNL Workfront]（デフォルト）。 組織のニーズを反映するには、既存のリスクタイプを編集するか、新しいリスクタイプを作成します。

* [既存のリスクタイプの編集](#edit-existing-risk-types)
* [新しいリスクタイプの作成](#create-new-risk-types)

### 既存のリスクタイプの編集 {#edit-existing-risk-types}

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL リスクタイプ]**.
1. 編集するリスクタイプを選択します。
1. クリック **[!UICONTROL 編集]**.
1. （オプション）リスクタイプの名前と説明を変更します。

   文字数の上限は 50 文字です **[!UICONTROL 名前]** そして **[!UICONTROL 説明]** フィールド。

1. クリック **[!UICONTROL 変更を保存].**

### 新しいリスクタイプの作成 {#create-new-risk-types}

デフォルトのリスクタイプに加えて、組織のニーズを反映した新しいリスクタイプを作成できます。

新しいリスク・タイプを作成する手順は、次のとおりです。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL リスクタイプ]**.
1. クリック **[!UICONTROL 新しいリスクタイプ]**.
1. タイプ a **[!UICONTROL 名前]** （必須）および **[!UICONTROL 説明]** （オプション）リスクタイプ。

   文字数の上限は 50 文字です **[!UICONTROL 名前]** そして **[!UICONTROL 説明]** フィールド。

1. クリック **[!UICONTROL リスクタイプの作成]**. インライン編集を使用してリスクタイプを追加した場合は、[ **[!UICONTROL 入力]** 完了したら

   >[!NOTE]
   >
   >カスタムリスクタイプを編集する必要がある場合は、「 [[!UICONTROL 既存の項目を編集] リスクタイプ](#edit-existing-risk-types) 」を参照してください。

## プロジェクトにリスクタイプを付加

リスクタイプは、プロジェクトに追加されるリスクのラベル付けに使用できます。 プロジェクトにリスクを追加する方法の詳細については、 [プロジェクトのリスクの作成と編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
