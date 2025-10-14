---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 危険タイプの編集および作成
description: 計画段階では、すべての作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。リスクとは、プロジェクトを期限内または予算内で完了することを妨げる可能性のあるイベントです。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 35%

---

# リスクタイプを編集および作成

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

Adobe Workfrontには、計画段階のプロジェクトに関連付けて、作業を承認する前に潜在的な障害を特定できる、デフォルトのリスクタイプが多数あります。

リスクとは、プロジェクトを期限内または予算内で完了することを妨げる可能性のあるイベントです。

既定の危険タイプに加えて、組織のニーズを反映する新しい危険タイプを追加することができます。

危険タイプをプロジェクトの危険に関連付けて、プロジェクトで発生する可能性のある危険の種類を特定することができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td><p>新規：[!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

*このテーブルの詳細については、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## リスクタイプ

リスクタイプは、レポート目的でリスクを分類するためにリスクに使用できるラベルです。

[!DNL Workfront] 管理者は、「設定 [!UICONTROL &#x200B; エリアで &#x200B;] リスクタイプ [!UICONTROL **を作成でき**] す。

リスクタイプを設定した後、これらはシステムに対して普遍的です。

すべてのプロジェクト所有者は、プロジェクトに同じリスクタイプを使用できます。

## リスクタイプを編集および作成

一部の危険タイプは、既定で既に [!DNL Workfront] にあります。


次の手順を実行して、Workfront インスタンスのリスクタイプの数を増やすことができます。

* [既存のリスクタイプを編集](#edit-existing-risk-types)
* [危険タイプの作成](#create-risk-types)

### 既存のリスクタイプを編集 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. 「**[!UICONTROL リスクタイプ]**」をクリックします。
1. 編集するリスクタイプを選択します。
1. **[!UICONTROL 編集]** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックします。

   <span class="preview"> 危険タイプを編集 [!UICONTROL **ボックスが開きます**]。</span>

   ![[ 危険タイプの編集 ] ボックス &#x200B;](assets/edit-risk-type-box.png)

   >[!TIP]
   >
   >   危険タイプの一覧の危険タイプの名前または説明をダブルクリックすると、危険タイプ情報をインラインで編集できます。

1. （オプション）リスクタイプの名前と説明を変更します。

   **[!UICONTROL 名前]**&#x200B;フィールドと&#x200B;**[!UICONTROL 説明]**&#x200B;フィールドには 50 文字の文字数制限があります。

1. 「**[!UICONTROL 変更を保存]」をクリックします。**

1. （オプション）危険タイプを削除するには、リストで危険タイプを選択して、[!UICONTROL **削除**] アイコン ![&#x200B; 削除アイコン &#x200B;](assets/delete.png) をクリックし、[!UICONTROL **はい、削除**] をクリックします。 危険タイプは削除され、回復できません。

1. （任意）危険タイプの一覧をエクスポートするには、[!UICONTROL **エクスポート**] アイコン ![&#x200B; エクスポートアイコン &#x200B;](assets/export-icon.png) をクリックします。 次のファイル タイプに書き出すことができます。

   * PDF
   * Excel
   * Excel（xlsx）
   * タブ区切り

   >[!TIP]
   >
   >   最初に限られた数の危険タイプを選択し、次に小さなリスト用にエクスポートできます。


### 危険タイプの作成 {#create-risk-types}

デフォルトのタイプに加えて、危険タイプも作成できます。

{{step-1-to-setup}}

1. 「**[!UICONTROL リスクタイプ]**」をクリックします。

1. **[!UICONTROL 新規危険タイプ]** をクリックして、「[!UICONTROL **新規危険タイプ**]」ボックスを開きます

   または

   危険タイプ リストの左下隅にある [[!UICONTROL **その他の危険タイプの追加**]] をクリックし、危険タイプをインラインで追加します。

   <span class="preview"> 新規危険タイプ **ボックスが開き** す。<span>

   ![&#x200B; 新しい危険タイプ ボックス &#x200B;](assets/new-risk-type-box.png)


1. 危険タイプに **[!UICONTROL 名前]** （必須）と **[!UICONTROL 説明]** （オプション）を追加します。

   **[!UICONTROL 名前]**&#x200B;フィールドと&#x200B;**[!UICONTROL 説明]**&#x200B;フィールドには 50 文字の文字数制限があります。

1. **[!UICONTROL 危険タイプの作成]** をクリックし、

   または、インライン編集を使用して危険タイプを追加した場合は、完了したら **[!UICONTROL Enter]** をクリックします。

   >[!TIP]
   >
   >カスタムの危険タイプを編集するには、この記事の「[[!UICONTROL &#x200B; 既存の &#x200B;] 危険タイプの編集 &#x200B;](#edit-existing-risk-types)」セクションを参照してください。

## プロジェクトのリスクタイプにリスクを添付

危険タイプを使用して、プロジェクトに追加された危険にラベルを付けることができます。

プロジェクトにリスクを追加する方法について詳しくは、[プロジェクトのリスクを作成および編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)を参照してください。
