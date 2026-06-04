---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: リスクタイプの編集と作成
description: 計画段階では、すべての作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。 リスクとは、プロジェクトを期限内または予算内で完了することを妨げる可能性のあるイベントです。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
TQID: https://experienceleague.adobe.com/KwUrEyHt6dqTcmP3JrTObsfvkcjP9q7O6-msiBuZVP4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 578
ht-degree: 35%

---

# リスクタイプを編集および作成

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfrontには、計画段階でプロジェクトに関連付けて、作業が承認される前に潜在的な障害を特定できる、デフォルトのリスクタイプがいくつかあります。

リスクとは、プロジェクトを期限内または予算内で完了することを妨げる可能性のあるイベントです。

デフォルトのリスクタイプに加えて、新しいリスクタイプを追加して、組織のニーズを反映できます。

リスクタイプをプロジェクトリスクに関連付けることで、プロジェクトでどのようなリスクが発生する可能性があるのかを特定できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リスクタイプ

リスクタイプとは、レポート用にリスクを分類するために使用できるラベルです。

[!DNL Workfront]管理者は、[!UICONTROL **セットアップ**]&#x200B;領域で[!UICONTROL  リスクタイプ ]を作成できます。

リスクタイプを設定した後は、システムに対して共通です。

すべてのプロジェクト所有者は、プロジェクトに同じリスクタイプを使用できます。

## リスクタイプを編集および作成

一部のリスクタイプは、デフォルトで既に[!DNL Workfront]にあります。


Workfront インスタンスのリスクタイプの数を増やすには、次の操作を実行します。

* [既存のリスクタイプを編集](#edit-existing-risk-types)
* [リスクタイプの作成](#create-risk-types)

### 既存のリスクタイプを編集 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. 「**[!UICONTROL リスクタイプ]**」をクリックします。
1. 編集するリスクタイプを選択します。
1. **[!UICONTROL 編集]** アイコン ![編集アイコン ](assets/edit-icon.png)をクリックします。

   「[!UICONTROL **リスクタイプを編集**]」ボックスが開きます。

   ![ リスクタイプボックスの編集](assets/edit-risk-type-box.png)

   >[!TIP]
   >
   >リスクタイプのリストでリスクタイプの「名前」または「説明」をダブルクリックすると、リスクタイプ情報をインラインで編集できます。

1. （オプション）リスクタイプの名前と説明を変更します。

   **[!UICONTROL 名前]**&#x200B;フィールドと&#x200B;**[!UICONTROL 説明]**&#x200B;フィールドには 50 文字の文字数制限があります。

1. 「**[!UICONTROL 変更を保存]」をクリックします。**

1. （オプション）リスクタイプを削除するには、リストでリスクタイプを選択し、[!UICONTROL **削除**] アイコン ![削除アイコン ](assets/delete.png)をクリックしてから、[!UICONTROL **はい、削除**]&#x200B;をクリックします。 リスクの種類は削除され、復元できません。

1. （オプション）リスクタイプのリストを書き出すには、[!UICONTROL **書き出し**] アイコン ![書き出しアイコン ](assets/export-icon.png)をクリックします。 次のファイルタイプに書き出すことができます。

   * PDF
   * Excel
   * Excel（xlsx）
   * タブ区切り

   >[!TIP]
   >
   >   最初に限られた数のリスクタイプを選択し、次に小さいリスト用に書き出すことができます。

### リスクタイプの作成 {#create-risk-types}

デフォルトタイプに加えて、リスクタイプを作成できます。

{{step-1-to-setup}}

1. 「**[!UICONTROL リスクタイプ]**」をクリックします。

1. 「**[!UICONTROL 新しいリスク タイプ]**」をクリックして、[!UICONTROL **新しいリスク タイプ**] ボックスを開きます

   または

   リスクタイプリストの左下隅にある「[!UICONTROL **その他のリスクタイプを追加**]」をクリックして、リスクタイプをインラインで追加します。

   「**新しいリスクの種類**」ボックスが開きます。

   ![新しいリスク タイプ ボックス ](assets/new-risk-type-box.png)

1. リスクの種類に「**[!UICONTROL 名前]**」（必須）と「**[!UICONTROL 説明]**」（オプション）を追加します。

   **[!UICONTROL 名前]**&#x200B;フィールドと&#x200B;**[!UICONTROL 説明]**&#x200B;フィールドには 50 文字の文字数制限があります。

1. 「**[!UICONTROL リスクタイプを作成]**」をクリックします。

   または、インライン編集を使用してリスクタイプを追加した場合は、完了したら&#x200B;**[!UICONTROL Enter]**&#x200B;をクリックします。

   >[!TIP]
   >
   >カスタムリスクタイプを編集するには、この記事の「[[!UICONTROL 既存の] リスクタイプを編集](#edit-existing-risk-types)」の節を参照してください。

## プロジェクトのリスクタイプにリスクを添付

リスクタイプを使用すると、プロジェクトに追加されたリスクにラベルを付けることができます。

プロジェクトにリスクを追加する方法について詳しくは、[プロジェクトのリスクを作成および編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)を参照してください。
