---
product-area: enterprise-scenario-planner-product-area
keywords: プラン, 権限, 共有, イニシアチブ, シナリオ, シナリオ
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Scenario Planner でプランへのアクセス権をリクエスト
description: プランへのリンクが共有されたら、Adobe Workfront Scenario Planner でプランへのアクセス権をリクエストできます。
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 84%

---

# [!DNL Scenario Planner] でプランへのアクセス権をリクエスト

プランへのリンクが共有されたら、[!DNL Adobe Workfront Scenario Planner] でプランへのアクセス権をリクエストできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] プラン*</p> </td> 
   <td> <ul></li>
   <li><p>新規：Ultimate </p></li>
   <p>シナリオプランナーは、新しいWorkfront Select プランまたはWorkfront Prime プランでは使用できません。 </p>
   <li><p>現在：[!UICONTROL Business] 以上</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td> <p>新規：ライト以上</p> 
   <p>現在：[!UICONTROL Review] 以上</p> </td> 
  </tr> 
  <tr> 
   <td>製品* </td> 
   <td> <ul><li><p>新しいWorkfrontプランの場合：</p><p> Adobe Workfront</li></p>
   <li><p>現在のWorkfront プランの場合： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront シナリオプランナー</p></li></ul>

<p>詳しくは、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a> ールの使用に必要なアクセス権」を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>アクセスレベル </td> 
   <td>  <p>[!UICONTROL ビュー ] 以上のユーザーアクセス [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>

*詳しくは、[Workfrontへのアクセス要件ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 前提条件

[!DNL Scenario Planner] でプランへのアクセス権をリクエストする前に、次の項目を有している必要があります。

* プランへのリンク。

>[!NOTE]
>
>[!DNL Scenario Planner] に対するアクセスレベル権限がない場合にリンクからプランにアクセスしようとしても、プランへのアクセス権をリクエストすることはできません。代わりに、[!DNL Workfront] 管理者に連絡するよう通知する画面が表示されます。

## [!DNL Workfront Scenario Planner] でのプランへのアクセス権のリクエスト

プランに対する権限をまだ持っていない場合に、自分と共有しているリンクからプランに移動すると、プランを表示する権限がないことを示す画面が表示されます。プラン作成者に権限をリクエストするように促すプロンプトが表示されます。

>[!TIP]
>
>プランの所有者または作成者に対してのみ、権限をリクエストできます。プランへのアクセス権を持つ他のユーザーに、権限をリクエストすることはできません。

権限をリクエストするには、次の手順に従います。

1. プランへのリンクをクリックします。

   ![ 計画へのアクセスの要求 ](assets/request-access-to-plan-350x277.png)

1. **[!UICONTROL アクセス権をリクエスト]**&#x200B;ドロップダウンメニューで、付与する権限のレベルを指定します。次の中から選択します。

   * [!UICONTROL 表示]
   * [!UICONTROL 管理]

   [!DNL Scenario Planner] へのアクセスレベルよりも高い権限をリクエストすることはできません。例えば、[!DNL Scenario Planner] への表示アクセス権がある場合、[!UICONTROL 管理]権限をリクエストすることはできません。

   様々なレベルの権限について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md) でプランを共有を参照してください。

   Workfront 管理者が [!DNL Scenario Planner] へのアクセスを管理する方法について詳しくは、[ [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md) へのアクセス権を付与を参照してください。

1. （オプション）「**[!UICONTROL コメントを残すボックス]**」にコメントまたはリクエストを入力し、「**[!UICONTROL アクセス権をリクエスト]**」をクリックします。

   次の処理が行われます。

   * [!DNL Workfront] はプラン所有者にメール通知を送信し、プラン所有者はリクエストされた権限を付与できます。\
     ![ アクセスをリクエストするメール通知 ](assets/request-access-to-plan-email-350x156.png)

   * プラン所有者がリクエストされた権限を付与すると、権限が付与されたことを知らせるメールが届きます（[!DNL Workfront] 管理者がシステムで「ユーザー宛オブジェクトの共有」通知を有効にし、ユーザーがプロファイルで「[!UICONTROL 誰かが自分とオブジェクトを共有]」メール通知を有効にしている場合）。

     ![ アクセス権が付与されたメール ](assets/access-granted-to-plan-email-350x172.png)

   * また、[!UICONTROL ホーム]領域と [!DNL Workfront] モバイルアプリからもプランへの権限を付与できます。

   システム通知の有効化について詳しくは、[システムのユーザー全員に対するイベント通知を設定](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

   プロファイルで通知を有効にする方法について詳しくは、[通知：その他の情報](../workfront-basics/using-notifications/notifications-misc-information.md)を参照してください。
