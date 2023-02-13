---
title: 暗号化
description: Adobe Workfront Fusion Encryptor モジュールを使用すると、任意のテキストデータを暗号化できます。 現在、AES256 と PGP(OpenPGP) を介したメッセージの暗号化をサポートしています。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 暗号化

[!DNL Adobe Workfront Fusion] [!UICONTROL 暗号化] モジュールを使用すると、任意のテキストデータを暗号化できます。 現在、AES256 および PGP([!UICONTROL OpenPGP]) をクリックします。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## PGP を使用したメッセージの暗号化と復号化

PGP で暗号化および復号化する場合、キーチェーンを使用し、秘密鍵または公開鍵（またはその両方）を作成する必要があります。

公開鍵と秘密鍵について詳しくは、 [の基本用語 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). キーチェーンの詳細については、 [のキー [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL 暗号化] モジュールとそのフィールド

設定時に [!UICONTROL 暗号化] モジュール、以下のフィールドが表示されます。 モジュール内の太字のタイトルは、必須フィールドを示します。

### PGP メッセージを暗号化

このモジュールでは、公開鍵と秘密鍵を使用してメッセージを暗号化できます。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 秘密鍵 ]</td>
        <td>送信者の秘密鍵を入力します。 これにより、送信者の ID を認証できます。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 公開鍵 ]</td>
        <td>受信者の公開鍵を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>暗号化するメッセージを入力します。</td>
    </tr>

### PGP メッセージを復号化

このモジュールでは、公開鍵と秘密鍵を使用してメッセージを復号化できます。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 秘密鍵 ]</td>
        <td>受信者の秘密鍵を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 公開鍵 ]</td>
        <td>受信者の公開鍵を入力します。 これにより、送信者の ID を認証できます。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>復号化するメッセージをマッピングします。</td>
    </tr>
</table>
