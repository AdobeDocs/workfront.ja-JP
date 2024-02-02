---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: リスクタイプを編集および作成
description: 計画段階では、すべての作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。リスクとは、プロジェクトを期限内または予算内で完了することを妨げる可能性のあるイベントです。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: ht
source-wordcount: '457'
ht-degree: 100%

---

# リスクタイプを編集および作成

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

計画段階では、すべての作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。リスクとは、プロジェクトを期限内または予算内で完了することを妨げる可能性のあるイベントです。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ユーザーは [!DNL Workfront] 管理者である必要があります。</p> <p><b>メモ</b>：アクセスできない場合は、[!DNL Workfront] 管理者にアクセスレベルに追加の制限が設定されていないかお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## リスクタイプ

リスクタイプは、レポート目的でリスクを分類するために使用できるラベルです。リスクタイプは、[!DNL Adobe Workfront] 管理者が&#x200B;**[!UICONTROL 設定]**&#x200B;エリアで作成します。**[!UICONTROL 設定]**&#x200B;エリアでリスクタイプが確立されると、リスクタイプはシステムに共通になります。すべてのプロジェクト所有者は、プロジェクトに同じリスクタイプを使用できます。

## リスクタイプを編集および作成

一部のリスクタイプはデフォルトで、既に [!DNL Workfront] に存在します。組織のニーズを反映させるために、既存のリスクタイプを編集するか、新しいリスクタイプを作成することができます。

* [既存のリスクタイプを編集](#edit-existing-risk-types)
* [新しいリスクタイプを作成](#create-new-risk-types)

### 既存のリスクタイプを編集 {#edit-existing-risk-types}

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. 「**[!UICONTROL リスクタイプ]**」をクリックします。
1. 編集するリスクタイプを選択します。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. （オプション）リスクタイプの名前と説明を変更します。

   **[!UICONTROL 名前]**&#x200B;フィールドと&#x200B;**[!UICONTROL 説明]**&#x200B;フィールドには 50 文字の文字数制限があります。

1. 「**[!UICONTROL 変更を保存]」をクリックします。**

### 新しいリスクタイプを作成 {#create-new-risk-types}

デフォルトのリスクタイプに加えて、組織のニーズを反映させる新しいリスクタイプを作成することができます。

リスクタイプを新規作成。

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 「**[!UICONTROL リスクタイプ]**」をクリックします。
1. 「**[!UICONTROL 新しいリスクタイプ]**」をクリックします。
1. リスクタイプの&#x200B;**[!UICONTROL 名前]**（必須）と&#x200B;**[!UICONTROL 説明]**（オプション）を入力します。

   **[!UICONTROL 名前]**&#x200B;フィールドと&#x200B;**[!UICONTROL 説明]**&#x200B;フィールドには 50 文字の文字数制限があります。

1. 「**[!UICONTROL リスクタイプを作成]**」をクリックします。インライン編集を使用してリスクタイプを追加した場合、完了したら&#x200B;**[!UICONTROL Enter]** をクリックします。

   >[!NOTE]
   >
   >カスタムリスクタイプを編集する必要がある場合は、[[!UICONTROL 既存の]リスクタイプ](#edit-existing-risk-types)を編集の節を参照してください。

## プロジェクトのリスクタイプにリスクを添付

リスクタイプは、プロジェクトに追加されるリスクのラベル付けに使用できます。プロジェクトにリスクを追加する方法について詳しくは、[プロジェクトのリスクを作成および編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)を参照してください。
