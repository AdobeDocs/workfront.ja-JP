---
product-area: enterprise-scenario-planner-product-area
keywords: プラン，権限，共有，イニシアチブ，シナリオ，シナリオ
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでのプランの共有
description: Adobe Workfront Scenario Planner で作成したプランを他のユーザーと共有できます。
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# プランを [!DNL Scenario Planner]

プランは [!DNL Adobe Workfront Scenario Planner] 他のユーザーと共同で作業を行うことができます。

>[!TIP]
>
>プランへのリンクを他のユーザーに送信する場合は、プランを他のユーザーと共有して、プランを表示できるようにする必要があります。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計画*</b> </p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> ライセンス*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>の追加ライセンスを購入する必要があります。 [!DNL Adobe Workfront Scenario Planner] をクリックして、この記事で説明する機能にアクセスします。</p> <p>詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">を使用するために必要なアクセス [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>[!UICONTROL 編集 ] で [!DNL Scenario Planner]</p> <p>まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p> プランに対する [!UICONTROL 管理 ] 権限
     <p>プランへの追加アクセス権のリクエストについて詳しくは、 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL リクエスト ] で [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 前提条件

* プランに対して権限を付与されたユーザーは、 [!DNL Scenario Planner] の領域（ユーザーが付与するアクセスレベル） [!DNL Workfront] 管理者（プランに対する権限を受け取るため）

   例： [!UICONTROL リクエスタ] プランの表示、作成、編集はできません。 要求者のライセンスを持つユーザーとプランを共有する場合は、この点に留意してください。

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

の [!DNL Scenario Planner] 各種ライセンスの種類については、 [へのアクセス権の付与 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## プラン共有に関する考慮事項

* 1 つのプランを共有することも、複数のプランを一括で共有することもできます。
* 自分が作成していないプランや、自分と共有されていないプランは表示できません。
* プランは他のユーザーとのみ共有できます。 プランをグループ、チーム、会社と共有することはできません。
* プランを共有する前に、まずプランを保存する必要があります。
* プランに対する URL を別のユーザーと共有できます。 少なくともプランを表示する権限を持っていないユーザーは、URL を受け取ったときに別のユーザーにプランへのアクセスを要求できます。 プランへのアクセス権のリクエストについて詳しくは、 [内のプランへのアクセスをリクエスト [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* 既に他のユーザーと共有されている複数のプランを共有する場合、共有したユーザーは置き換えられず、選択した各プランの既存のユーザーに追加されます。

## プランを共有

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **[!UICONTROL シナリオ]**.
1. プランの名前をクリックして開きます

   または

   一括で共有するプランを複数選択します。

   >[!TIP]
   >
   >プランのヘッダーの右上隅にある、プランの共有相手となるユーザーのアバターをクリックして、プランを共有できます。

1. （条件付き）プランを開いた場合、 **[!UICONTROL 詳細]** アイコン ![](assets/more-icon.png) 右 [!UICONTROL プラン] 名前を入力し、「 **[!UICONTROL 共有]**

   または

   複数のプランを選択して一括で共有する場合は、 **[!UICONTROL 共有]** アイコン ![](assets/share-icon-26x26.png) を開く予定のリストの一番上に [!UICONTROL プラン] アクセスボックス

   >[!TIP]
   >
   >* 選択したすべてのプランに対する権限を持つユーザーが、 [!UICONTROL プラン] アクセスボックス
   >* 選択したすべてのプランで、追加のユーザーがに追加され、既存のユーザーは置き換えられません。


1. 内 **[!UICONTROL へのプランアクセス権の付与]** 「 」フィールドに、プランを共有するユーザーの名前を入力し、リストに表示されたら選択します。
1. ユーザー名の右側にある権限ドロップダウンメニューから、プランに付与する権限のレベルを選択します。
1. 次の中から選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 表示 ]</td> 
      <td>プランを共有するユーザーには、プランを表示する権限が与えられます。 プランに関する情報の編集、イニシアチブ、シナリオの追加、シナリオの公開はできません。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 管理 ]</td> 
      <td> <p>プランを共有するユーザーには、プランを管理する権限があります。これには、情報の編集、イニシアチブの追加、シナリオの追加、プランの公開が含まれます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >プランは、作成時にのみ削除できます。 自分と共有されているプランは削除できません。

1. 「**[!UICONTROL 保存]**」をクリックします。

   これで、プランが指定したユーザーと共有されます。

   プランに対する権限を持つユーザーは、プランのリストの「自分と共有」列またはプランヘッダーの右上隅に表示できます。

   >[!TIP]
   >
   >自分と共有されているプランを表示するには、 [!UICONTROL 自分と共有済み] プランのリストでフィルターします。

## プラン権限オプション

次の表に、プランを共有する際に付与できる権限を示します。 ユーザーがライセンスに基づいて取得するアクセスについて詳しくは、 [へのアクセス権の付与 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>アクション</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL 管理 ]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL 表示 ]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>プランを表示 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>イニシアチブの表示 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>シナリオを表示</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>ジョブの役割の表示</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>コストと予算情報の表示*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>コストと予算情報の管理*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>イニシアチブの作成</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>シナリオの作成</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>イニシアチブまたはシナリオを削除</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>シナリオのコピー</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>シナリオの公開**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*プランに対する権限を管理している場合でも、プランの財務情報を表示または管理するには、財務データへのアクセス権が必要です。 財務データへのアクセスについて詳しくは、 [財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**シナリオを公開するには、プロジェクトを管理するための作成権限と権限が必要です。

プロジェクトのアクセスレベルについては、 [プロジェクトへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

プロジェクト権限について詳しくは、 [でプロジェクトを共有 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
