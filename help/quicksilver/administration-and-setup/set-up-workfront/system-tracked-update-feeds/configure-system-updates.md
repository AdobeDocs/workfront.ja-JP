---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: システム更新の構成
description: Workfrontは、オブジェクトの [!UICONTROL 更新] オブジェクトに対してユーザーが実行した変更を記録する領域。 As a [!DNL Workfront] 管理者は、どのオブジェクトフィールドとアクションを設定できます [!DNL Workfront] システムの更新を記録するトラッキング。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 7%

---

# システム更新の構成

[!DNL Adobe Workfront] オブジェクトの自動システム更新を生成します。 [!UICONTROL 更新] 以下のイベントを記録する領域：

* オブジェクトフィールドでユーザーがおこなった変更
* オブジェクトに対してユーザーが実行するアクション

これらのシステム更新には、次の種類の情報が含まれます。

* 変更が加えられた
* 変更を加えたユーザーの名前
* 変更日時

システムの更新の詳細については、 [システムで追跡された更新](../system-tracked-update-feeds/system-tracked-update-feeds.md).

As a [!DNL Workfront] 管理者は、どのオブジェクトフィールドとアクションを設定できます [!DNL Workfront] システムの更新を記録するトラッキング。

例えば、 [!DNL Workfront] システム全体でユーザーが行った問題の名前の変更をすべて追跡します。 問題名の変更は、問題の [!UICONTROL 更新] 領域。

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
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。</p> <p><b>注意</b>：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## どのフィールドを特定するか [!DNL Workfront] オブジェクトタイプのトラック

どの情報が表示されるかは、 [!DNL Workfront] ユーザーが、 [!DNL Workfront] インターフェイス。 これをおこなうには、目的のフィールドを追加または削除します [!DNL Workfront] をクリックして、そのオブジェクトタイプを追跡します。

>[!NOTE]
>
>* [!DNL Workfront] は、計算済みカスタムフィールドの更新を追跡して記録することはできません。
>* プロジェクト、タスク、問題、ポートフォリオ、プログラムおよびユーザーのシステム更新をカスタマイズできます。 テンプレート、ドキュメント、またはタイムシートのシステム更新はカスタマイズできませんが、 [!DNL Workfront] は、これらのオブジェクトのシステム更新を記録します。
>



* [必要なフィールドを追加します [!DNL Workfront] 追跡する](#add-fields-you-want-workfront-to-track)
* [追跡しないフィールドを削除します](#remove-fields-that-you-don-t-want-tracked)

### 必要なフィールドを追加します [!DNL Workfront] 追跡する {#add-fields-you-want-workfront-to-track}

必要なフィールドを追加できます [!DNL Workfront] を通して特定のタイプのオブジェクトを追跡するには [!DNL Workfront] インターフェイス。 ユーザーがそのフィールドの情報を変更した場合、 [!DNL Workfront] は、変更に関する情報をシステム更新として [!UICONTROL 更新] オブジェクトの領域。

>[!NOTE]
>
>更新フィードでは、最大 300 個の組み込みフィールドとカスタムフィールドを追跡できます。 追跡するフィールドの最大数を追跡していて、 [!UICONTROL すべてのフィールド] サブタブで、新しいフィールドを追跡するには、まず一部の追跡フィールドを削除する必要があります。 更新フィールドからフィールドを削除する方法について詳しくは、 [追跡しないフィールドを削除します](#remove-fields-that-you-don-t-want-tracked).

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) ～の右上隅に [!DNL Adobe Workfront]を選択し、次に **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **[!UICONTROL インターフェイス]** > **[!UICONTROL フィードを更新]**.

1. ク&#x200B;リック **[!UICONTROL フィールドを追加]**&#x200B;を選択し、追跡するオブジェクトをクリックします。

1. 内&#x200B;の **[!UICONTROL フィードを更新]** ボックスが表示されたら、オブジェクトの組み込み（標準）フィールドまたはカスタムフィールドを入力し、リストに表示されたときにクリックして選択します。

   次の場合 [!DNL Workfront] は既にフィールドを追跡しているので、リストから 2 回目は追加できません。

1. 必要なすべてのフィールドを追加した後 [!DNL Workfront] トラッキングするには、 **[!UICONTROL フィールドを追加]**.

   追加した組み込みフィールドが **[!UICONTROL 組み込みフィールド]** サブタブを使用します。

   追加したカスタムフィールドは、 **[!UICONTROL カスタムフィールド]** サブタブを使用します。

   The **[!UICONTROL すべてのフィールド]** サブタブには、追跡されている組み込みフィールドとカスタムフィールドの両方が表示されます。

### 追跡しないフィールドを削除します {#remove-fields-that-you-don-t-want-tracked}

特定のタイプのオブジェクトに対して、 [!DNL Workfront] インターフェイス。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) ～の右上隅に [!DNL Adobe Workfront]を選択し、次に **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL インターフェイス]** > **[!UICONTROL フィードを更新]**.

1. 次の日： **[!UICONTROL 追跡フィールド]** タブで、 **[!UICONTROL すべてのフィールド]** サブタブを使用します。

   これには、現在追跡中の組み込みフィールドとカスタムフィールドの両方が表示されます。

1. トラッキングを停止するフィールドを選択し、「 **[!UICONTROL 削除]**.

1. Adobe Analytics の **[!UICONTROL フィールドを削除]** 表示されるボックスで、 **[!UICONTROL はい、削除します]** をクリックして確定します。

以前に追跡されたフィールドに関する更新は、 [!UICONTROL 更新] 記録された領域。

## どのアクションを決定するか [!DNL Workfront] オブジェクトタイプのトラック

以下を使用できます。 [!DNL Workfront] を通じて、ユーザーがオブジェクトに対して実行できる次のアクションを追跡します。 [!DNL Workfront] インターフェイス。

例えば、 [!DNL Workfront] ユーザーがタスクまたはイシューに割り当てを変更するたびに、更新を記録します。 変更は、システム更新として「 [!UICONTROL 更新] タスクまたはイシューの領域。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>アクション</strong> </th> 
   <th><strong>オブジェクト</strong> </th> 
   <th><strong>プライマリ状況</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>割り当ての変更</td> 
   <td>タスク、問題</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>ベースラインの削除</td> 
   <td>プロジェクト</td> 
   <td> <p>無効</p> </td> 
  </tr> 
  <tr> 
   <td>請求レコードが作成または削除されました</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>ドキュメントの作成または削除</td> 
   <td>プロジェクト、タスク、問題、ポートフォリオ、プログラム</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>費用の作成または削除</td> 
   <td>プロジェクト、タスク</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>時間の記録または削除</td> 
   <td>プロジェクト、タスク、問題</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>問題の削除</td> 
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
   <td>プロジェクト、タスク、問題、ドキュメント、ポートフォリオ、プログラム</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>コメント オブジェクトを登録</td> 
   <td>プロジェクト、タスク、問題</td> 
   <td> <p>有効</p> </td> 
  </tr> 
 </tbody> 
</table>

目的のアクションを設定するには [!DNL Workfront] 追跡する

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) ～の右上隅に [!DNL Adobe Workfront]を選択し、次に **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL インターフェイス]** > **[!UICONTROL フィードを更新]**.

1. 次をクリック： **[!UICONTROL アクション]** タブをクリックします。

1. アクションを選択して有効にするか、アクションの選択を解除して無効にします。
1. 「**[!UICONTROL 保存]**」をクリックします。

アクションを無効にすると、そのアクションに関して以前に記録された更新は、 [!UICONTROL 更新] 記録された領域。
