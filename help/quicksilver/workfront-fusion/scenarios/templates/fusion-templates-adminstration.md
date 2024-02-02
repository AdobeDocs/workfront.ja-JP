---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion テンプレートの管理
description: 管理者には、他のユーザーが作成したテンプレートの表示、変更、名前の変更、公開、承認、削除を行う権限があります。これらのアクションは、 [!DNL Adobe Workfront Fusion Administration]  エリアの[!UICONTROL テンプレート]ページから実行できます。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '626'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] テンプレートの管理

管理者には、他のユーザーが作成したテンプレートの表示、変更、名前の変更、公開、承認、削除を行う権限があります。これらのアクションは、[!DNL Adobe Workfront Fusion Administration] エリアの[!UICONTROL テンプレート]ページから実行できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
    <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>組織の Workfront Fusion 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 管理者として [!DNL Workfront Fusion] テンプレートを表示する

作成したすべてのテンプレートとそのステータスの表を表示するには、以下を行います。

1. 左側のナビゲーションパネルで「**[!UICONTROL 管理]**」をクリックして、[!UICONTROL 管理]エリアを開きます。
1. 左側のナビゲーションパネルで「**[!UICONTROL テンプレート]**」をクリックします。

テンプレートの公開ステータスに関連する列が 3 つあります。列内のチェックマークが示す意味は次のとおりです。

* **[!UICONTROL 公開中のアイテム]**：これらのテンプレートは、現在、「[!UICONTROL チームテンプレート]」タブに表示されています。
* **[!UICONTROL 要求された承認]**：これらのテンプレートは承認待ちです。これらは現在、ユーザーインターフェイスの「[!UICONTROL チームテンプレート]」タブに表示されます。
* **[!UICONTROL 承認済み]**：これらのテンプレートは承認済みです。これらは現在、ユーザーインターフェイスの「[!UICONTROL 公開テンプレート]」タブに表示されています。

>[!NOTE]
>
>[!UICONTROL 要求された承認]列と[!UICONTROL 承認済み]列の両方にチェックマークが付いたテンプレートは、既に承認され公開されていますが、承認待ちの新しいバージョンがあります。

## 管理者として [!DNL Workfront Fusion] テンプレートを編集する

1. 左側のナビゲーションパネルで「**[!UICONTROL 管理]**」をクリックして、[!UICONTROL 管理]エリアを開きます。
1. 左側のナビゲーションパネルで「**[!UICONTROL テンプレート]**」をクリックします。
1. 編集するテンプレートの右側にある「**[!UICONTROL 詳細]**」をクリックします。

管理者以外のユーザーとしてテンプレートを編集する場合と同様に、テンプレートを編集できるようになりました。ただし、右上隅の「[!UICONTROL オプション]」には、SVG コードを提供する SVG 図という追加オプションが 1 つあります。また、公開プロセスは標準ユーザーの場合と同じです。詳しくは、テンプレートの公開と共有の節を参照してください。

編集できる特定のテンプレートオプションについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md) でテンプレートを新規作成を参照してください。

テンプレートの公開について詳しくは、[ [!DNL Adobe Workfront Fusion]  のテンプレートを公開して共有](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)を参照してください。

## [!DNL Workfront Fusion] テンプレートを承認または却下する

テンプレートを承認すると、「[!UICONTROL 公開テンプレート]」タブにテンプレートが表示され、すべてのユーザーが利用できます。テンプレートを却下すると、「[!UICONTROL 公開テンプレート]」タブからテンプレートが削除され、作成したチームのみが使用できます。

1. 左側のナビゲーションパネルで「**[!UICONTROL 管理]**」をクリックして、[!UICONTROL 管理]エリアを開きます。
1. 左側のナビゲーションパネルで「**[!UICONTROL テンプレート]**」をクリックします。
1. テンプレートを承認する場合は、テンプレートの右側にある「**[!UICONTROL 承認]**」をクリックします。
1. テンプレートを却下する場合は、テンプレートの右側にある「**[!UICONTROL 却下]**」をクリックします。

>[!NOTE]
>
>以前に承認および編集されたテンプレートを承認する場合は、2 回目の承認で元のテンプレートが上書きされます。

## シナリオをテンプレートとして複製

管理者は、シナリオをテンプレートとして複製できます。

テンプレートとしてシナリオを複製する手順については、[ [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md) で新しいテンプレートを作成にある、[シナリオからテンプレートを作成](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario)を参照してください。
