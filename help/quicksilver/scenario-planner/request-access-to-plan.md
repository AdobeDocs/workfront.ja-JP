---
product-area: enterprise-scenario-planner-product-area
keywords: プラン, 権限, 共有, イニシアチブ, シナリオ, シナリオ
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでのプランへのアクセスをリクエスト
description: プランへのリンクが共有されたら、Adobe Workfront Scenario Planner でプランへのアクセス権をリクエストできます。
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 83%

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
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>WorkfrontUltimate</p>
<p><b>メモ</b></p>
<p>別のWorkfront パッケージをお持ちの場合は、Workfront担当者にお問い合わせください。</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス</p> </td> 
   <td> <p>[!UICONTROL ライト &#x200B;] 以上</p> 
   <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
    <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>[!UICONTROL ビュー &#x200B;] 以上のユーザーアクセス [!DNL Scenario Planner]</p> </td> 
  </tr> 
 </tbody> 
</table>

シナリオプランナーへのアクセスについて詳しくは、[&#x200B; の使用に必要なアクセス  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) を参照してください。

Workfrontのアクセス要件について詳しくは、[Workfrontのドキュメントへのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td>  <p>[!UICONTROL View] or higher access to the [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>-->

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

   ![&#x200B; 計画へのアクセスの要求 &#x200B;](assets/request-access-to-plan-350x277.png)

1. **[!UICONTROL アクセス権をリクエスト]**&#x200B;ドロップダウンメニューで、付与する権限のレベルを指定します。次の中から選択します。

   * [!UICONTROL 表示]
   * [!UICONTROL 管理]

   [!DNL Scenario Planner] へのアクセスレベルよりも高い権限をリクエストすることはできません。例えば、[!DNL Scenario Planner] への表示アクセス権がある場合、[!UICONTROL 管理]権限をリクエストすることはできません。

   様々なレベルの権限について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md) でプランを共有を参照してください。

   Workfront 管理者が [!DNL Scenario Planner] へのアクセスを管理する方法について詳しくは、[&#x200B; [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md) へのアクセス権を付与を参照してください。

1. （オプション）「**[!UICONTROL コメントを残すボックス]**」にコメントまたはリクエストを入力し、「**[!UICONTROL アクセス権をリクエスト]**」をクリックします。

   次の処理が行われます。

   * [!DNL Workfront] はプラン所有者にメール通知を送信し、プラン所有者はリクエストされた権限を付与できます。\
     ![&#x200B; アクセスをリクエストするメール通知 &#x200B;](assets/request-access-to-plan-email-350x156.png)

   * プラン所有者がリクエストされた権限を付与すると、権限が付与されたことを知らせるメールが届きます（[!DNL Workfront] 管理者がシステムで「ユーザー宛オブジェクトの共有」通知を有効にし、ユーザーがプロファイルで「[!UICONTROL 誰かが自分とオブジェクトを共有]」メール通知を有効にしている場合）。

     ![&#x200B; アクセス権が付与されたメール &#x200B;](assets/access-granted-to-plan-email-350x172.png)

   * また、[!UICONTROL ホーム]領域と [!DNL Workfront] モバイルアプリからもプランへの権限を付与できます。

   システム通知の有効化について詳しくは、[システムのユーザー全員に対するイベント通知を設定](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

   プロファイルで通知を有効にする方法について詳しくは、[通知：その他の情報](../workfront-basics/using-notifications/notifications-misc-information.md)を参照してください。
