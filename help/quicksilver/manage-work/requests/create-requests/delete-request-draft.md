---
product-area: requests
navigation-topic: create-requests
title: 送信されたリクエストの再リクエストドラフトを削除
description: 送信されたリクエストまたはリクエストのドラフトを削除できます。
author: Becky
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: d87df92f548b19901374e982d1759efade644e17
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 39%

---

# 送信されたリクエストまたはリクエストドラフトの削除

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の本番環境でのみ使用できます。</span>

新しいリクエスト用エクスペリエンスで作成した、送信済みのリクエストまたはリクエストドラフトを削除できます。 Workfront管理者と Planning Workspace 管理者は、リクエストを削除することもできます。

従来のリクエストエクスペリエンスでは、リクエストドラフトを削除できます。 送信したリクエストは削除できません。

詳しくは、以下を参照してください。

* [Adobe Workfront リクエストを作成して送信](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [ドラフトからリクエストを作成](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>投稿者以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>自分が作成しなかったリクエストを削除するには、Workfront管理者または Planning Workspace 管理者である必要があります。</p><p>従来のリクエストエクスペリエンスでドラフトを削除するには、イシューへの編集アクセス権が必要です。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>新しいリクエストエクスペリエンスで削除するには、リクエストまたはドラフトを作成している必要があります。</p><p>従来のリクエストエクスペリエンスでドラフトを削除するには、イシューへの編集アクセス権が必要です。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 製品</td> 
   <td> <ul><li>Adobe Workfront</li><li>計画リクエストまたはリクエストフォームを表示するには、Adobe Workfront Planning が必要です。</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


<div class="preview">

## リクエストを削除 <!--or request drafts --> 新しいリクエストエクスペリエンスで

リクエストの削除は、Workfrontのリクエスト エリア、またはホームのマイリクエストウィジェットで実行できます。

* Workfront管理者は <!-- and drafts--> 組織内のリクエストを削除できます。
* Workfront Planning Workspace 管理者は、自身が管理する Planning Workspace に <!--and drafts--> る要求を削除できます。
* ユーザーは、自身が送信したリクエスト <!--and drafts--> 削除できます。

### 3 ドットメニューからのリクエストの削除

1. 「リクエスト」リストにアクセスするには、Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックします。または（利用可能な場合）左上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、「**[!UICONTROL リクエスト]**」をクリックします。

1. ホームのリクエスト ウィジェットにアクセスするには：

   1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
   1. 自分のリクエスト ウィジェットを見つけます。

      マイリクエストウィジェットについて詳しくは、[ マイリクエストウィジェットの使用 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md) を参照してください。

1. リクエストリストまたはマイリクエストウィジェットで、削除するリクエスト <!--or draft --> にポインタを合わせます。

   「。..」メニューが表示されます。
   ![](assets/more-menu.png)

1. リクエスト **ージ名の右側にある** 詳細 <!--or draft--> メニューをクリックしてから、**削除** をクリックします。

   または

   選択したリクエストを右クリックし、「**削除**」をクリックします。

   >[!TIP]
   >
   >イシューを作成するアクセス権がない場合は、管理者によってリクエストの作成が制限されたという警告が表示されます。

1. 開いたダイアログで、「**削除**」をクリックします。

   リクエスト <!--or draft--> が削除されます。

### 一括削除リクエスト

1. 「リクエスト」リストにアクセスするには、Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックします。または（利用可能な場合）左上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、「**[!UICONTROL リクエスト]**」をクリックします。

1. ホームのリクエスト ウィジェットにアクセスするには：

   1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
   1. 自分のリクエスト ウィジェットを見つけます。

      マイリクエストウィジェットについて詳しくは、[ マイリクエストウィジェットの使用 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md) を参照してください。

1. リクエスト リストまたは自分のリクエスト ウィジェットで、削除する各リクエストの左側にあるボックスをクリックします。
1. ページ下部の青いバーで、「**削除**」をクリックします。

   >[!NOTE]
   >
   >青いバーに「削除」オプションが表示されない場合は、選択した 1 つ以上のリクエストを削除する権限がありません。

</div>

## 従来のリクエストエクスペリエンスでのリクエストドラフトの削除

ドラフトされたリクエストがドラフトとして保存された後、関連性がなくなった場合は削除できます。削除されたドラフトリクエストを回復することはできません。

### リクエストドラフトを削除するための前提条件

リクエストのドラフトを削除する前に、以下を行う必要があります。

* リクエストの作成を開始します。これにより、リクエストがドラフトとして「ドラフト」セクションに自動的に保存されます。

  リクエストの作成について詳しくは、[Adobe Workfront リクエストの作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

### リクエストのドラフトを削除

{{step1-to-requests}}

1. 左側のパネルで「**ドラフト**」を選択します。

   このリストには、すべてのリクエストキューのすべてのドラフトが表示されます。

1. （オプション）ドラフトのリストの右上隅にある「**リクエストタイプでフィルタリング**」をクリックし、表示するドラフトを含むリクエスト キューを選択します。
1. リストからドラフトを選択し、リストの上部にある&#x200B;**削除**&#x200B;をクリックします。
1. 「**はい、削除します**」をクリックします。

   ドラフトは削除され、復元できなくなりました。
