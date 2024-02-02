---
title: 暗号化
description: Adobe Workfront Fusion 暗号化モジュールを使用すると、任意のテキストデータを暗号化できます。現在、AES256 と PGP（OpenPGP）を介したメッセージの暗号化をサポートしています。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '334'
ht-degree: 100%

---

# 暗号化

[!DNL Adobe Workfront Fusion] [!UICONTROL 暗号化]モジュールを使用すると、任意のテキストデータを暗号化できます。現在、AES256 と PGP（[!UICONTROL OpenPGP]）を介したメッセージの暗号化をサポートしています。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>レガシーライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront]プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## PGP を使用したメッセージの暗号化と復号

PGP で暗号化および復号する場合、キーチェーンを使用し、秘密鍵または公開鍵（またはその両方）を作成する必要があります。

公開鍵と秘密鍵について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md) の基本用語を参照してください。キーチェーンについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md) のキーを参照してください。

## [!UICONTROL 暗号化]モジュールとそのフィールド

[!UICONTROL 暗号化]モジュールの設定時に、以下のフィールドが表示されます。モジュール内の太字のタイトルは、必須フィールドを示します。

### PGP メッセージを暗号化

このモジュールで、公開鍵と秘密鍵を使用してメッセージを暗号化できます。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>送信者の秘密鍵を入力します。これにより、送信者の ID を認証できます。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>受信者の公開鍵を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>暗号化するメッセージを入力します。</td>
    </tr>

### PGP メッセージを復号化

このモジュールでは、公開鍵と秘密鍵を使用してメッセージを復号できます。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>受信者の秘密鍵を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>受信者の公開鍵を入力します。これにより、送信者の ID を認証できます。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>復号するメッセージをマッピングします。</td>
    </tr>
</table>
