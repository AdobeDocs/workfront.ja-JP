---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: システム更新の構成
description: Workfront は、オブジェクトの[!UICONTROL 更新]エリアで自動システム更新を生成し、ユーザーがオブジェクトに対して実行した変更を記録します。 [!DNL Workfront]  管理者は、 [!DNL Workfront]  がどのオブジェクトフィールドおよびアクションを追跡するかを設定して、システム更新を記録できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f7cb314067d105d5534f4be356024aea8e8f9a28
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 47%

---

# システム更新の設定

<!-- Audited: 6/2025 -->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

[!DNL Adobe Workfront] は、オブジェクトの[!UICONTROL 更新]エリアで自動システム更新を生成し、次のイベントを記録します。

* オブジェクトフィールドでユーザーが行う変更
* オブジェクトに対してユーザーが実行するアクション

これらのシステム更新には、次のタイプの情報が含まれています。

* 行われた変更
* 変更を行ったユーザーの名前
* 変更の日時

システム更新について詳しくは、[システムで追跡される更新](../system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

[!DNL Workfront] 管理者は、[!DNL Workfront] がどのオブジェクトフィールドおよびアクションを追跡するかを設定して、システム更新を記録できます。

例えば、システム全体でユーザーがイシューの名前に対して行ったすべての変更を [!DNL Workfront] で追跡できます。イシュー名の変更は、イシューの[!UICONTROL 更新]エリアにシステム更新として表示されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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

*このテーブルの詳細については、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## [!DNL Workfront] がオブジェクトタイプのどのフィールドを追跡するかを決定

ユーザーが [!DNL Workfront] インターフェイス全体で特定のオブジェクトタイプに関連付けられた情報を変更したときに、[!DNL Workfront] がどの情報を追跡するかを決定できます。これを行うには、[!DNL Workfront] が追跡するオブジェクトタイプのフィールドを追加または削除します。

>[!NOTE]
>
>* 計算 [!DNL Workfront] れたカスタムフィールドに関する更新を追跡および記録することはできません。
>* プロジェクト、タスク、イシュー、ポートフォリオ、プログラムおよびユーザーのシステム更新をカスタマイズできます。テンプレート、ドキュメント、タイムシートのシステム更新はカスタマイズできませんが、[!DNL Workfront] ではこれらのオブジェクトのシステム更新が記録されます。
>


### [!DNL Workfront] が追跡するフィールドの追加 {#add-fields-you-want-workfront-to-track}

[!DNL Workfront] インターフェイス全体に渡り、特定のタイプのオブジェクトについて [!DNL Workfront] が追跡するフィールドを追加できます。ユーザーがそのフィールドの情報を変更した場合、[!DNL Workfront] は、変更に関する情報をシステム更新として、オブジェクトの[!UICONTROL 更新]エリアに記録します。

>[!NOTE]
>
>更新フィードでは、最大 300 個の組み込みフィールドとカスタムフィールドを追跡できます。最大数のフィールドを追跡していて、「[!UICONTROL &#x200B; すべてのフィールド &#x200B;]」サブタブに表示されていない追加フィールドを追跡する場合、新しいフィールドを追跡するには、最初に追跡対象のフィールドのいくつかを削除する必要があります。 更新フィールドからフィールドを削除する方法について詳しくは、[ 追跡しないフィールドの削除 ](#remove-fields-you-don-t-want-tracked) を参照してください。

{{step-1-to-setup}}

1. 左側のパネルで「**[!UICONTROL インターフェイス]**」をクリックし、「**[!UICONTROL フィードを更新]** をクリックします。
1. （オプション）「**追跡対象フィールド**」タブで、更新フィードで追跡するフィールドのタイプに応じて、次のいずれかのサブタブをクリックします。

   * **組み込みフィールド**：組み込みフィールドのリストを表示します。
   * **カスタムフィールド**：カスタムフィールドのリストを表示します。 リストで使用する前にカスタムフィールドを作成する必要があります。
   * **すべてのフィールド**：組み込みフィールドとカスタムフィールドの両方のリストを表示します。

1. **[!UICONTROL フィールドを追加]** をクリックして、追跡するオブジェクトをドロップダウンから選択します。

   「更新」領域を持つすべてのオブジェクトで、フィールドの手動選択を使用できるわけではありません。

   次のオブジェクトのフィールドから選択します。

   * プロジェクト
   * タスク
   * イシュー
   * ポートフォリオ
   * プログラム
   * ユーザー

   **フィールドを追加** ボックスが、選択したオブジェクトごとに開きます。
1. 「**フィールドを追加**」ボックスに、オブジェクトの組み込み（標準）フィールドまたはカスタムフィールドの入力を開始し、リストに表示されたら選択します。

   >[!NOTE]
   >
   >既にフィールドをトラッキングしている [!DNL Workfront] 合は、リストから 2 回目は追加できません。

1. 追跡するすべてのフィールドを追加し [!DNL Workfront] 後、「**[!UICONTROL フィールドの追加]** をクリックします。
追加した組み込みフィールドは「**[!UICONTROL 組み込みフィールド]** サブタブの下に表示され、カスタムフィールドは「**[!UICONTROL カスタムフィールド]** サブタブの下に表示されます。
**[!UICONTROL すべてのフィールド]** サブタブには、トラックする組み込みフィールドとカスタムフィールドの両方が表示 [!DNL Workfront] れます。

<!-- replace the above when releasing to Preview: 

1. In the panel on the left, click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.
1. (Optional) In the <span class="preview">**Tracked fields** tab</span>, click one of the following subtabs, depending on which types of fields you want to track in the update feed:

   * <span class="preview">**Built-in fields**</span>: Displays a list of built-in fields.
   * <span class="preview">**Custom fields**</span>: Displays a list of custom fields. You must create the custom fields before they are available in the list. 
   * <span class="preview">**All fields**</span>: Displays a list of both built-in and custom fields. 

1. Click <span class="preview">**[!UICONTROL Add fields]**,</span> then select the object that you want to be tracked from the drop-down. 

   Manually selecting fields is not available for all the objects that have an Updates area.

   Select from fields for the following objects:

      * Project
      * Task
      * Issue
      * Portfolio
      * Program
      * User

   The <span class="preview">**Add fields** </span> box opens, for each object selected.
1. In the <span class="preview">**Add fields** </span> box, start typing either a built-in (standard) field or a custom field for the object, then select it when it appears in the list.

   >[!NOTE]
   >
   >If [!DNL Workfront] is already tracking the field, you can't add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, <span class="preview"> click **[!UICONTROL Add]**.
   The built-in fields that you added show under the **[!UICONTROL Built-in fields]** subtab, and the custom fields show under the **[!UICONTROL Custom fields]** subtab.
   The **[!UICONTROL All fields]** subtab shows both the built-in and the custom fields that [!DNL Workfront] tracks.</span>

-->

### 追跡しないフィールドを削除 {#remove-fields-you-don-t-want-tracked}

特定のタイプのオブジェクトに対してシステムが追跡したくないフィールドを、[!DNL Workfront] インターフェイス全体で削除できます。

{{step-1-to-setup}}

1. **[!UICONTROL インターフェイス]** をクリックし、**[!UICONTROL フィードを更新]** をクリックします。

1. **[!UICONTROL トラッキングフィールド]** タブで「**[!UICONTROL すべてのフィールド]** サブタブを選択します。 現在追跡中のビルトインフィールドとカスタムフィールドの両方が表示されます。

1. トラッキングを停止するフィールドを選択し、「**[!UICONTROL 削除]**」をクリックします。


<!--replace above at Preview release with this:

1. On the <span class="preview">**[!UICONTROL Tracked fields]** tab</span>, select the **[!UICONTROL All fields]** subtab. Both the built-in and custom fields that are currently being tracked display.

1. Select the field you want to stop tracking, then click the <span class="preview">**[!UICONTROL Remove]** icon ![Remove icon](assets/remove-icon.png).</span>

-->

1. 表示される「**[!UICONTROL フィールドを削除]**」ボックスで、「**[!UICONTROL はい、削除します]**」をクリックして確定します。

   以前に追跡されたフィールドに関する更新は、記録された[!UICONTROL 更新]エリアに保存されます。

## [!DNL Workfront] がオブジェクトタイプのどのアクションを追跡するかを決定

[!DNL Workfront] ーザーインターフェイス [!DNL Workfront] は、ユーザーがオブジェクトに対して実行するアクションを追跡できます。

例えば、ユーザーがタスクまたは問題 [!DNL Workfront] 割り当てを変更するたびに更新を記録することができます。

変更は、タスクまたはイシューの[!UICONTROL 更新]エリアに、システム更新として表示されます。

次の表に、[!DNL Workfront] でオブジェクトに対して追跡できるアクションを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>アクション</strong> </th> 
   <th><strong>オブジェクト</strong> </th> 
   <th><strong>デフォルトのステータス</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>割り当ての変更</td> 
   <td>タスク、イシュー</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>ベースラインの削除</td> 
   <td>プロジェクト</td> 
   <td> <p>無効</p> </td> 
  </tr> 
  <tr> 
   <td>請求記録の作成または削除</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>ドキュメントの作成または削除</td> 
   <td>プロジェクト、タスク、イシュー、ポートフォリオ、プログラム</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>費用の作成または削除</td> 
   <td>プロジェクト、タスク</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>時間の記録または削除</td> 
   <td>プロジェクト、タスク、イシュー</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>イシューを削除</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>タスクの削除</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>誰かのアクセス権限の変更</td> 
   <td>プロジェクト、タスク、イシュー、ドキュメント、ポートフォリオ、プログラム</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>コメントオブジェクトの登録</td> 
   <td>プロジェクト、タスク、イシュー</td> 
   <td> <p>有効</p> </td> 
  </tr> 
 </tbody> 
</table>

[!DNL Workfront] で追跡するアクションを設定するには、次の操作を行います。

{{step-1-to-setup}}

1. **[!UICONTROL インターフェイス]** をクリックし、**[!UICONTROL フィードを更新]** をクリックします。

1. 「**[!UICONTROL アクション]**」タブをクリックします。

1. アクションのチェックボックスを選択して有効にするか、選択解除して無効にします。
1. **[!UICONTROL 保存]**&#x200B;をクリックします。

   アクションを無効にすると、そのアクションに関して以前に記録された更新は、記録された [!UICONTROL &#x200B; 更新 &#x200B;] 領域に保持されます。 無効 [!DNL Workfront] したアクションの新しい更新の記録を停止します。
