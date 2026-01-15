---
product-area: requests
navigation-topic: create-requests
title: 送信されたリクエストの再リクエストドラフトを削除
description: 送信されたリクエストまたはリクエストのドラフトを削除できます。
author: Becky
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: b58814d68d582a08457d1d4685d110c2bdd2087c
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# 送信されたリクエストまたはリクエストドラフトの削除

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

## 新しいリクエストエクスペリエンスでのリクエストまたはリクエストドラフトの削除

リクエストの削除は、Workfrontのリクエスト エリア、またはホームのマイリクエストウィジェットで実行できます。

* Workfront管理者は、組織内のリクエストとドラフトを削除できます。
* Workfront Planning Workspace 管理者は、自身が管理する Planning Workspace の要求および草案を削除できます。
* ユーザーは、送信したリクエストとドラフトを削除できます。

### 3 ドットメニューからのリクエストの削除

{{step1-to-requests}}

1. ホームのリクエスト ウィジェットにアクセスするには：

   {{step1-to-home}}

   1. 自分のリクエスト ウィジェットを見つけます。

      マイリクエストウィジェットについて詳しくは、[&#x200B; マイリクエストウィジェットの使用 &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md) を参照してください。

1. リクエストリストまたはマイリクエストウィジェットで、削除するリクエストまたはドラフトにポインタを合わせます。

   「。..」メニューが表示されます。
   ![](assets/more-menu.png)

1. リクエスト名またはドラフト名の右側にある **詳細** メニューをクリックしてから、「**削除**」をクリックします。

   または

   選択したリクエストを右クリックし、「**削除**」をクリックします。

   >[!TIP]
   >
   >イシューを作成するアクセス権がない場合は、管理者によってリクエストの作成が制限されたという警告が表示されます。

1. 開いたダイアログで、「**削除**」をクリックします。

   リクエストまたはドラフトが削除されます。

### 一括削除リクエスト

{{step1-to-requests}}

1. ホームのリクエスト ウィジェットにアクセスするには：

   {{step1-to-home}}

   1. 自分のリクエスト ウィジェットを見つけます。

      マイリクエストウィジェットについて詳しくは、[&#x200B; マイリクエストウィジェットの使用 &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md) を参照してください。

1. リクエスト リストまたは自分のリクエスト ウィジェットで、削除する各リクエストの左側にあるボックスをクリックします。
1. ページ下部の青いバーで、「**削除**」をクリックします。

   >[!NOTE]
   >
   >青いバーに「削除」オプションが表示されない場合は、選択した 1 つ以上のリクエストを削除する権限がありません。

</div>

## 従来のリクエストエクスペリエンスでのリクエストドラフトの削除

ドラフトされたリクエストがドラフトとして保存された後、関連性がなくなった場合は削除できます。削除されたドラフトリクエストを回復することはできません。

### リクエストドラフトを削除するための前提条件

リクエストドラフトを削除するには、次の手順を実行する必要があります。

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
