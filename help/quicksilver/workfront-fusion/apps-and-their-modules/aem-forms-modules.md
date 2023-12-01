---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Formsモジュール
description: を使用 [!DNL Adobe Experience Manager Forms] コネクタ [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] アセットのアカウント、作成、アップロードおよび更新、およびフォルダーとアセットのコピーまたは移動をおこなう。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c4e068729d8de4bef4b2018868e3fa020ca61a06
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms] モジュール

を使用 [!DNL Adobe Experience Manager Forms] コネクタ [!DNL Adobe Workfront Fusion]の場合は、 [!DNL Adobe Experience Manager Forms] アカウントを作成します。

フォームは、 [!DNL Adobe Experience Manager Forms] この Webhook にフォーム送信を送信します。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

* 次が必要です： [!DNL Adobe Experience Manager Forms] このモジュールを使用するアカウント。

## Adobe Experience Manager Formsへの接続の作成

の接続を作成するには、以下を実行します。 [!DNL Adobe Experience Manager Forms] モジュール：

1. クリック **[!UICONTROL 追加]** 「接続」ボックスの横に表示されます。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL 接続名 ]</td>
        <td>
          <p>この接続の名前を入力します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 環境 ]</td>
        <td>
          <p>この接続を実稼動環境と非実稼動環境のどちらに接続するかを選択します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL の種類 ]</td>
        <td>
          <p>このアカウントがサービスアカウントか個人用アカウントかを選択します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL インスタンス URL （末尾にスラッシュを含まない）]</td>
        <td>
          <p>アカウントへのアクセスに使用する URL を入力します（最後のスラッシュは使用しません）。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL IMS エンドポイント ]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL クライアント ID]</td>
        <td>を入力します。 [!DNL Adobe] クライアント ID。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
        <td>を入力します。 [!DNL Adobe] クライアントの秘密鍵。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Org ID]</td>
        <td>を入力します。 [!DNL Adobe] 組織 ID。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL テクニカルアカウント ID]</td>
        <td>を入力します。 [!DNL Adobe] テクニカルアカウント ID。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL メタスコープ ]</td>
        <td>適切なメタスコープを入力します。       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 秘密鍵 ]</td>
        <td>
          <p>秘密鍵を入力します。秘密鍵は、 [!DNL Adobe Developer Console]. </p>
          <p>秘密鍵または証明書を抽出するには：</p>
          <ol>
            <li value="1">
              <p>クリック <b>[!UICONTROL 抽出 ]</b>.</p>
            </li>
            <li value="2">
              <p>抽出するファイルの種類を選択します。</p>
            </li>
            <li value="3">
              <p>秘密鍵または証明書を含むファイルを選択します。</p>
            </li>
            <li value="4">
              <p>ファイルのパスワードを入力します。</p>
            </li>
            <li value="5">
              <p>クリック <b>[!UICONTROL 保存 ]</b> をクリックしてファイルを抽出し、接続設定に戻ります。</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. クリック **[!UICONTROL 続行]** 接続を保存し、モジュールに戻ります。

## Adobe Experience Manager Formsモジュールとそのフィールド

現在、Adobe Experience Manager Forms Connector には 1 つのモジュールのみがあります。

### フォームイベントの監視

このインスタントトリガー(Webhook) を使用すると、Adobe Experience Managerフォームで送信アクションが発生したときにシナリオを開始できます。

>[!IMPORTANT]
>
>また、このモジュールは、Adobe Experience Managerでの設定も必要です。 この Webhook を設定したら、Adobe Experience Managerを開き、Webhook に送信するようにフォームを設定する必要があります。
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>ウェブフックの名前を入力</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法については、 [!DNL Adobe Experience Manager] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">への接続の作成 [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

このモジュールは Webhook を作成し、Webhook のアドレスを提供します。このアドレスは、 [!DNL Adobe Experience Manager Forms].











