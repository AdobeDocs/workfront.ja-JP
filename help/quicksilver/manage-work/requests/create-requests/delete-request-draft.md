---
product-area: requests
navigation-topic: create-requests
title: 送信済みリクエストまたはリクエストドラフトの削除
description: Adobe Workfrontでは、送信されたリクエストまたはリクエストドラフトを削除できます。
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 26%

---

# 送信されたリクエストまたはリクエストのドラフトの削除

Adobe WorkfrontまたはAdobe Workfront Planningが送信したリクエストを削除したり、作成したドラフトをリクエストしたり、管理権限を持っている場合は、これらの権限を持つことができます。

Workfront管理者とWorkfront Planningのワークスペース管理者は、作成しなかったリクエストを削除したり、ドラフトをリクエストしたりすることもできます。

従来のリクエストエクスペリエンスでPlanning リクエストを表示することはできません。

この記事では、新しいリクエストエクスペリエンスでリクエストドラフトを削除する方法について説明します。 WorkfrontとPlanningのリクエストまたはそのドラフトの削除は同じです。

詳しくは、以下を参照してください。

* [Adobe Workfront リクエストを作成して送信](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [ドラフトからリクエストを作成](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [Adobe Workfront Planning リクエストを送信して、レコードを作成](/help/quicksilver/planning/requests/submit-requests.md)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意のWorkfrontまたはWorkflow パッケージ</p>

<p>プランニングリクエストを管理するための任意のWorkfrontプランニングパッケージ </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>コントリビューター以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>作成しなかったリクエストを削除するには、Workfront管理者またはPlanning Workspace マネージャーである必要があります。</p><p>イシューへの編集アクセス権が必要です。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストまたはドラフトを作成して新しいリクエストのエクスペリエンスで削除するか、Workfront管理者またはPlanning Workspace マネージャーとして、送信しなかったリクエストのドラフトを削除する必要があります。
   </p><p>削除する問題に対する編集権限が必要です。</p>  </td> 
  </tr>

</tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 新しいリクエストエクスペリエンスでのリクエストまたはリクエストドラフトの削除

次の領域でリクエストとドラフトを削除できます。

* Workfrontのリクエスト領域に
* ホームのマイリクエストウィジェットで
* リクエストページから

次のユーザーは、リクエストドラフトを削除できます。

* Workfront管理者は、自分または他のユーザーが送信したリクエストとドラフトを削除できます。
* Workfront計画ワークスペース管理者は、自分が管理する計画ワークスペースで、リクエストとドラフトを削除できます。
* ユーザーは、送信したリクエストとドラフトを削除できます。

### ホームのリクエスト領域またはマイリクエストウィジェットからリクエストまたはドラフトを削除します

{{step1-to-requests}}

1. **ホーム**&#x200B;の&#x200B;**マイリクエスト** ウィジェットにアクセスするには：

   {{step1-to-home}}

   1. **My Requests** ウィジェットを探します。

      **My Requests** ウィジェットについて詳しくは、[My Requests ウィジェットの使用](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)を参照してください。

1. **リクエスト** リストまたは&#x200B;**ホーム**&#x200B;の&#x200B;**マイリクエスト** ウィジェットで、削除するリクエストまたはドラフトにカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックします

1. 「**削除**」をクリック

   または

   選択したリクエストを右クリックし、**削除**&#x200B;をクリックします。

   >[!TIP]
   >
   >イシューを作成するアクセス権がない場合は、管理者によってリクエストの作成が制限されたという警告が表示されます。

1. 開いたダイアログで、**削除**&#x200B;をクリックします。

   リクエストまたはドラフトが削除されます。

   削除されたリクエストはごみ箱に保存され、Workfront管理者は最大30日間復元できます。 ドラフトは復元できません。

### リストからリクエストを一括削除

{{step1-to-requests}}

1. **ホーム**&#x200B;の&#x200B;**マイリクエスト** ウィジェットにアクセスするには：

   {{step1-to-home}}

   1. **My Requests** ウィジェットを探します。

      マイリクエストウィジェットについて詳しくは、[ マイリクエストウィジェットの使用](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)を参照してください。

1. **リクエスト** リストまたは&#x200B;**マイリクエスト** ウィジェットで、削除する各リクエストの左側にあるボックスをクリックします。
1. ページ下部の青いバーで、**削除**&#x200B;をクリックします。

   >[!NOTE]
   >
   >**削除** オプションが青いバーに表示されない場合、選択した1つ以上のリクエストを削除する権限がありません。

### リクエストドラフトを削除するための前提条件

リクエストドラフトを削除する前に、次の操作を行う必要があります。

* リクエストの作成を開始します。これにより、リクエストがドラフトとして「ドラフト」セクションに自動的に保存されます。

  リクエストの作成について詳しくは、[Adobe Workfront リクエストの作成および送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

## 従来のリクエストエクスペリエンスでのリクエストドラフトの削除

ドラフトされたリクエストがドラフトとして保存された後、関連性がなくなった場合は削除できます。削除されたドラフトリクエストを回復することはできません。

従来のリクエストエクスペリエンスからPlanning リクエストまたはそのドラフトにアクセスすることはできません。

{{step1-to-requests}}

1. 左側のパネルで「**ドラフト**」をクリックします。

   このリストには、すべてのリクエストキューのすべてのドラフトが表示されます。

1. リストからドラフトを選択し、リストの上部にある&#x200B;**削除**&#x200B;をクリックします。
1. 「**はい、削除します**」をクリックします。

   ドラフトは削除され、復元できなくなりました。






