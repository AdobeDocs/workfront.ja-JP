---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Templates 管理
description: 管理者は、他のユーザーが作成したテンプレートの表示、変更、名前の変更、公開、承認、削除をおこなう権限を持っています。 これらのアクションは、 [!UICONTROL テンプレート] ページの [!DNL Adobe Workfront Fusion Administration] 領域
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] テンプレート管理

管理者は、他のユーザーが作成したテンプレートの表示、変更、名前の変更、公開、承認、削除をおこなう権限を持っています。 これらのアクションは、 [!UICONTROL テンプレート] ページの [!DNL Adobe Workfront Fusion Administration] 領域

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
    <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA) </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>組織のWorkfront Fusion 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 表示 [!DNL Workfront Fusion] 管理者としてのテンプレート

作成したすべてのテンプレートとそのステータスの表を表示するには：

1. クリック **[!UICONTROL 管理]** 左側のナビゲーションパネルで、 [!UICONTROL 管理] 領域
1. クリック **[!UICONTROL テンプレート]** をクリックします。

テンプレートのパブリッシュステータスに関連する列が 3 つあります。 列内のチェックマークは次のことを示します。

* **[!UICONTROL 公開済み]**:これらのテンプレートは、現在、 [!UICONTROL チームテンプレート] 」タブをクリックします。
* **[!UICONTROL リクエストされた承認]**:これらのテンプレートは、お客様の承認を待っています。 現在、 [!UICONTROL チームテンプレート] 」タブをクリックします。
* **[!UICONTROL 承認済み]**:これらのテンプレートは承認されました。 現在、 [!UICONTROL 公開テンプレート] 」タブをクリックします。

>[!NOTE]
>
>チェックマークが付いたテンプレートが [!UICONTROL リクエストされた承認] 列と [!UICONTROL 承認済み] 列は既に承認され、公開されていますが、承認を待っている新しいバージョンがあります。

## 編集 [!DNL Workfront Fusion] 管理者としてのテンプレート

1. クリック **[!UICONTROL 管理]** 左側のナビゲーションパネルで、 [!UICONTROL 管理] 領域
1. クリック **[!UICONTROL テンプレート]** をクリックします。
1. クリック **[!UICONTROL 詳細]** をクリックします。

管理者以外のユーザーとしてのテンプレートの編集と同様に、テンプレートを編集できるようになりました。 ただし、 [!UICONTROL オプション] 右上隅には、追加のオプションが 1 つあります。SVGコードを示すSVG図です。 また、公開プロセスは、標準ユーザーの場合と同じです。詳しくは、テンプレートの公開と共有の節を参照してください。

編集できる特定のテンプレートオプションについて詳しくは、 [で新しいテンプレートを作成 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

テンプレートの公開について詳しくは、 [公開して共有 [!DNL Adobe Workfront Fusion] テンプレート](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## 承認または却下 [!DNL Workfront Fusion] テンプレート

テンプレートを承認すると、 [!UICONTROL 公開テンプレート] 」タブに表示され、すべてのユーザーが利用できます。 テンプレートを却下すると、テンプレートが [!UICONTROL 公開テンプレート] 」タブに移動し、作成したチームのみが使用できるようにします。

1. クリック **[!UICONTROL 管理]** 左側のナビゲーションパネルで、 [!UICONTROL 管理] 領域
1. クリック **[!UICONTROL テンプレート]** をクリックします。
1. テンプレートを承認する場合は、 **[!UICONTROL 承認]** を選択します。
1. テンプレートを却下する場合は、 **[!UICONTROL 却下]** を選択します。

>[!NOTE]
>
>以前に承認され編集されたテンプレートを承認する場合は、2 回目の承認で元のテンプレートが上書きされます。

## シナリオをテンプレートとして複製

管理者は、シナリオをテンプレートとして複製できます。

テンプレートとしてシナリオを複製する手順については、 [シナリオからのテンプレートの作成](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [で新しいテンプレートを作成 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
