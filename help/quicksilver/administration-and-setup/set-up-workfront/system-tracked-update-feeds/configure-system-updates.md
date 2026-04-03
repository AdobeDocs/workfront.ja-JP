---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: システム更新の設定
description: Workfront は、オブジェクトの[!UICONTROL 更新]エリアで自動システム更新を生成し、ユーザーがオブジェクトに対して実行した変更を記録します。 [!DNL Workfront]  管理者は、 [!DNL Workfront]  がどのオブジェクトフィールドおよびアクションを追跡するかを設定して、システム更新を記録できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 48%

---

# システム更新の設定

<!-- Audited: 08/2025 -->

<!--

<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

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
   <td role="rowheader">[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>[!UICONTROL System Administrator]</p></td>
  </tr> 
 </tbody> 
</table>

* この表の詳細については、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>
-->

## [!DNL Workfront] がオブジェクトタイプのどのフィールドを追跡するかを決定

ユーザーが [!DNL Workfront] インターフェイス全体で特定のオブジェクトタイプに関連付けられた情報を変更したときに、[!DNL Workfront] がどの情報を追跡するかを決定できます。これを行うには、[!DNL Workfront] が追跡するオブジェクトタイプのフィールドを追加または削除します。

>[!NOTE]
>
>* [!DNL Workfront]は、計算されたカスタム フィールドに関する更新を追跡および記録できません。
>* プロジェクト、タスク、イシュー、ポートフォリオ、プログラムおよびユーザーのシステム更新をカスタマイズできます。テンプレート、ドキュメント、またはタイムシートのシステム更新をカスタマイズすることはできませんが、[!DNL Workfront]はこれらのオブジェクトのシステム更新を記録します。
>


### [!DNL Workfront] が追跡するフィールドの追加 {#add-fields-you-want-workfront-to-track}

[!DNL Workfront] インターフェイス全体に渡り、特定のタイプのオブジェクトについて [!DNL Workfront] が追跡するフィールドを追加できます。ユーザーがそのフィールドの情報を変更した場合、[!DNL Workfront] は、変更に関する情報をシステム更新として、オブジェクトの[!UICONTROL 更新]エリアに記録します。

>[!NOTE]
>
>更新フィードでは、最大 300 個のビルトインのフィールドとカスタムフィールドを追跡できます。フィールドの最大数を追跡しており、[!UICONTROL すべてのフィールド &#x200B;] サブタブに表示されない追加のフィールドを追跡する場合は、新しいフィールドを追跡するために、最初に追跡されたフィールドの一部を削除する必要があります。 更新フィールドからフィールドを削除する方法の詳細については、[&#x200B; トラッキングしないフィールドの削除](#remove-fields-you-don-t-want-tracked)を参照してください。

{{step-1-to-setup}}

1. 左側のパネルで、「**[!UICONTROL インターフェイス]**」、「**[!UICONTROL フィードを更新]**」の順にクリックします。
1. （オプション）「**追跡されたフィールド**」タブで、更新フィードで追跡するフィールドのタイプに応じて、次のいずれかのサブタブをクリックします。

   * **組み込みフィールド**：組み込みフィールドのリストを表示します。
   * **カスタムフィールド**：カスタムフィールドのリストを表示します。 カスタムフィールドをリストで使用する前に作成する必要があります。
   * **すべてのフィールド**：ビルトインフィールドとカスタムフィールドの両方のリストを表示します。

1. 「**[!UICONTROL フィールドを追加]**」をクリックし、ドロップダウンから追跡するオブジェクトを選択します。

   「更新」領域を持つすべてのオブジェクトでは、フィールドを手動で選択することはできません。

   次のオブジェクトのフィールドから選択します。

   * プロジェクト
   * タスク
   * イシュー
   * ポートフォリオ
   * プログラム
   * ユーザー

   選択した各オブジェクトについて、**フィールドを追加** ボックスが開きます。
1. 「**フィールドを追加**」ボックスで、オブジェクトの組み込み（標準）フィールドまたはカスタムフィールドのいずれかを入力し始め、リストに表示されたら選択します。

   >[!NOTE]
   >
   >[!DNL Workfront]が既にフィールドを追跡している場合、リストから2回目に追加することはできません。

1. [!DNL Workfront]で追跡するフィールドをすべて追加したら、**[!UICONTROL 追加]**&#x200B;をクリックします。
追加した組み込みフィールドは&#x200B;**[!UICONTROL 組み込みフィールド]** サブタブに表示され、カスタムフィールドは&#x200B;**[!UICONTROL カスタムフィールド]** サブタブに表示されます。
**[!UICONTROL すべてのフィールド]** サブタブには、[!DNL Workfront]が追跡する組み込みフィールドとカスタムフィールドの両方が表示されます。

### 追跡しないフィールドを削除 {#remove-fields-you-don-t-want-tracked}

特定のタイプのオブジェクトを追跡しないフィールドは、[!DNL Workfront] インターフェイス全体で削除できます。

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェイス]**」、「**[!UICONTROL フィードを更新]**」の順にクリックします。

1. 「**[!UICONTROL トラッキングフィールド]**」タブで、「**[!UICONTROL すべてのフィールド]**」サブタブを選択します。 現在追跡されているビルトインフィールドとカスタムフィールドの両方が表示されます。

1. トラッキングを停止するフィールドを選択し、**[!UICONTROL 削除]** アイコン ![削除アイコン &#x200B;](assets/remove-icon.png)をクリックします。

1. 表示される「**[!UICONTROL フィールドを削除]**」ボックスで、「**[!UICONTROL はい、削除します]**」をクリックして確定します。

   以前に追跡されたフィールドに関する更新は、記録された[!UICONTROL 更新]エリアに保存されます。

## [!DNL Workfront] がオブジェクトタイプのどのアクションを追跡するかを決定

ユーザーが[!DNL Workfront] インターフェイス内のオブジェクトに対して実行するアクションを[!DNL Workfront]回追跡できます。

例えば、ユーザーがタスクまたは問題への割り当てを変更するたびに、[!DNL Workfront]に更新を記録させることができます。

変更は、タスクまたはイシューの[!UICONTROL 更新]エリアに、システム更新として表示されます。

次の表に、[!DNL Workfront]のオブジェクトで追跡できるアクションを示します。

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

1. 「**[!UICONTROL インターフェイス]**」、「**[!UICONTROL フィードを更新]**」の順にクリックします。

1. 「**[!UICONTROL アクション]**」タブをクリックします。

1. アクションのチェックボックスを選択して有効にするか、選択を解除して無効にします。
1. 「**[!UICONTROL 保存]**」をクリックします。

   アクションを無効にすると、そのアクションに関して以前に記録された更新は、そのアクションが記録された[!UICONTROL 更新]領域に保持されます。 [!DNL Workfront]は、無効なアクションの新しい更新の記録を停止します。
