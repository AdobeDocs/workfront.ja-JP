---
product-area: enterprise-scenario-planner-product-area
keywords: プラン,権限,共有,イニシアチブ,シナリオ
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでのプランの共有
description: Adobe Workfront シナリオプランナーで作成したプランを他のユーザーと共有できます。
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: ht
source-wordcount: '916'
ht-degree: 100%

---

# [!DNL Scenario Planner]でのプランの共有

[!DNL Adobe Workfront Scenario Planner]でプランを他のユーザーと共有して、自分と同じ作業を他のユーザーと共同で行うことができます。

>[!TIP]
>
>プランへのリンクを他のユーザーに送信する場合は、そのプランも共有して、他のユーザーがプランを表示できるようにする必要があります。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> プラン*</b> </p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>ライセンス*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>この記事で説明されている機能にアクセスするには、[!DNL Adobe Workfront Scenario Planner]の追加ライセンスを購入する必要があります。</p> <p>[!DNL Workfront Scenario Planner]の入手については、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a>の使用に必要なアクセス権を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>[!UICONTROL Edit]アクセス権 [!DNL Scenario Planner]</p> <p>それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p> 計画の[!UICONTROL Manage]権限
     <p>計画への追加アクセス権の申請については、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a>での計画へのアクセス権の[!UICONTROL Request]を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

* 計画への権限を付与されたユーザーが計画への権限を受け取るには、[!DNL Workfront] 管理者から[!DNL Scenario Planner]エリアへのアクセス権がアクセスレベルに付与されている必要があります。

  例えば、[!UICONTROL 要求者]は計画の表示、作成または編集を行えません。要求者ライセンスを持つユーザーと計画を共有する場合は、この点に留意してください。

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

様々なライセンスタイプの[!DNL Scenario Planner]へのアクセス権については、[ [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)へのアクセス権の付与を参照してください。

## 計画の共有に関する考慮事項

* 1 つの計画を共有することも、複数の計画を一括で共有することもできます。
* 自分が作成していない計画または自分と共有されていない計画は表示できません。
* 計画は他のユーザーとのみ共有できます。計画をグループ、チームまたは会社と共有することはできません。
* 計画を共有するには、まず計画を保存する必要があります。
* 計画の URL を別のユーザーと共有できます。少なくとも計画を表示する権限を持っていないユーザーは、URL を受け取ったときに、別のユーザーに計画へのアクセス権を申請できます。計画へのアクセス権の申請については、[ [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)での計画へのアクセス権の申請を参照してください。
* 既に他のユーザーと共有している複数の計画を共有する場合、共有するユーザーは置き換えられず、選択した各計画の既存のユーザーに追加されます。

## 計画の共有

1. Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**[!UICONTROL シナリオ]**」をクリックします。
1. 計画の名前をクリックして、計画を開きます。

   または

   複数の計画を選択して、それらを一括で共有します。

   >[!TIP]
   >
   >計画のヘッダーの右上隅に表示されている、計画の共有相手となるユーザーのアバターをクリックすると、計画を共有できます。

1. （条件付き）計画が開かれている場合は、[!UICONTROL 計画]の名前の右側にある&#x200B;**[!UICONTROL その他]**&#x200B;アイコン ![](assets/more-icon.png) をクリックし、次に「**[!UICONTROL 共有]**」をクリックします。

   または

   複数の計画を選択して一括で共有する場合は、計画のリストの上部にある&#x200B;**[!UICONTROL 共有]**&#x200B;アイコン ![](assets/share-icon-26x26.png) をクリックして、[!UICONTROL 計画アクセス]ボックスを開きます。

   >[!TIP]
   >
   >* 選択したすべての計画に対する権限を持つユーザーが、[!UICONTROL 計画アクセス]ボックスに表示されます。
   >* 追加ユーザーは、選択したすべての計画の既存ユーザーに追加され、既存ユーザーを置き換えることはありません。

1. 「**[!UICONTROL 計画へのアクセス権の付与先]**」フィールドに、計画を共有するユーザーの名前を入力していき、該当する名前がリストに表示されたら選択します。
1. ユーザー名の右側にある権限ドロップダウンメニューから、ユーザーに付与する、計画に対する権限のレベルを選択します。
1. 次の中から選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>計画を共有するユーザーには、計画を表示する権限が付与されます。計画に関する情報の編集、イニシアチブやシナリオの追加またはシナリオの公開はできません。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>計画を共有するユーザーには計画を管理する権限があります。この権限には、情報の編集、イニシアチブやシナリオの追加、計画の公開などが含まれます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >計画を削除できるのは、それを自分が作成した場合のみです。自分と共有されている計画は削除できません。

1. 「**[!UICONTROL 保存]**」をクリックします。

   これで、指定したユーザーと計画が共有されます。

   計画に対する権限を持つユーザーは、計画のリストの「自分と共有」列または計画ヘッダーの右上隅に表示されます。

   >[!TIP]
   >
   >自分と共有されている計画を表示するには、計画のリストで[!UICONTROL 自分と共有]フィルターを適用します。

## 計画の権限オプション

計画を共有する際に付与できる権限を次の表に示します。ライセンスに基づいてユーザーが取得するアクセス権について詳しくは、[へのアクセス権の付与 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)を参照してください。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>アクション</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>計画の表示 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>イニシアチブの表示 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>シナリオの表示</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>担当業務の表示</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>コストと予算の情報の表示*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>コストと予算の情報の管理*</td> 
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
   <td> <p>イニシアチブまたはシナリオの削除</p> </td> 
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

*計画に対する管理権限がある場合でも、計画の財務情報を表示または管理するには、財務データへのアクセス権が必要です。財務データへのアクセス権については、[財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

**シナリオを公開するには、プロジェクトを作成するためのアクセス権とプロジェクトの管理権限が必要です。

プロジェクトのアクセスレベルについては、[プロジェクトへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

プロジェクト権限について詳しくは、[ [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) でプロジェクトを共有を参照してください。
