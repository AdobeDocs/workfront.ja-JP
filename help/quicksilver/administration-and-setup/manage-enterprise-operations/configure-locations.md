---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 場所の設定
description: レートカードの担当業務に属性として割り当てることができるデフォルトの場所を設定できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
source-git-commit: d0464b7f055b9351ba5c3353c7e806c51008e30b
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 26%

---

# 場所を設定

{{preview-fast-release-general}}

レートカードの担当業務に属性として割り当てることができるデフォルトの場所を設定できます。 これにより、評価カードが各場所の市場評価を正確に反映します。

評価カードを使用すると、組織でプロジェクトの請求レートを簡単に管理できます。 詳しくは、[ レートカードの管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)および[ レート属性の定義](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td>ワークフロー Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 場所を追加

{{step-1-to-setup}}

1. 左パネルで、「[!UICONTROL **場所**]」をクリックします。
1. 実稼動環境で、リストの下部にある「[!UICONTROL **さらに場所を追加**]」をクリックします。
   <span class="preview"> プレビュー環境で、リストの下部にある&#x200B;[!UICONTROL **新しい行**]&#x200B;をクリックします。</span>

1. 場所の名前と説明を入力します。
1. 行の外側をクリックして、場所を保存します。
1. 実稼動環境の場所を削除するには、リストでその場所を選択し、**削除** アイコン ![削除アイコン ](assets/delete.png)をクリックします。
   <span class="preview"> プレビュー環境で場所を削除するには、リストで場所を選択し、画面下部のアクションバーの&#x200B;[!UICONTROL **削除**]&#x200B;をクリックします。</span>

>[!NOTE]
>
>評価カード上の担当業務に関連付けられている場所は削除できません。

## サブロケーションの追加

既存の場所にサブロケーションを追加できます。 例えば、既に英国のロケーションがある場合、ロンドンはサブロケーションになる可能性があります。

3つのレベルのサブロケーションが許可されています。 国、州または都道府県、および都市は、サブロケーションの一般的な用途です。

各サブロケーションは、トップレベルのロケーションと同じようにレートカードの属性として追加して、そのロケーションの特定のジョブロールのレートを定義できます。

{{step-1-to-setup}}

1. 左パネルで、「[!UICONTROL **場所**]」をクリックします。
1. 実稼動環境で、リスト内の既存の場所を選択し、[!UICONTROL **サブ場所を追加**]をクリックします。
   <span class="preview"> プレビュー環境で、リスト内の既存の場所を選択し、画面下部のアクションバーで&#x200B;[!UICONTROL **サブ場所を追加**]&#x200B;をクリックします。</span>

1. 場所の名前と説明を入力します。
1. 入力領域の外側をクリックして、場所を保存します。

   サブロケーションは、トップレベルのロケーションの下にインデントされます。

   実稼動環境のサンプル画像：
   ![場所とサブ場所](assets/locations-sublocations.png)

   <span class="preview"> プレビュー環境のサンプル画像：</span>
   ![場所とサブ場所](assets/locations-sublocations-082526.png)


