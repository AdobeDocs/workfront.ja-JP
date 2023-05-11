---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: http-modules
title: Adobe Workfront Fusion の HTTP モジュールで相互 TLS を使用
description: Adobe Workfront Fusion HTTP モジュールで相互 TLS を使用すると、情報トランザクションの両側で相手の ID を検証できます。
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: d54a6072524274cf77ee0ca7b7cfa24987c97782
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# の HTTP モジュールでの相互 TLS の使用 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion には、 [!DNL Adobe Workfront Fusion] ライセンスを追加してください。Adobe Workfrontライセンス。

## 相互 TLS の概要

インターネットを介してデータを送信する場合は、データを正しい場所に送信するか、正しい場所から送信し、意図した受信者のみが読み取れるようにすることが重要です。 TLS が有効な場合、クライアント（情報を要求するコンピュータ）は証明書を使用して、サーバー（情報を提供するコンピュータ）の ID を検証します。 これにより、安全な HTTP 接続が可能になります。

相互 TLS を使用すると、この ID 確認が両方の方法で実行できます。 サーバーが証明書を送信してクライアントに ID を検証すると、クライアントの証明書も要求します。 これにより、サーバーが誤用の原因となる情報をサイトやユーザーに送信しなくなります。

>[!INFO]
>
>**例:**
>
>* **TLS**:ユーザーがブラウザに「MyGreatBank.com」と入力すると、銀行情報を誤って使用したり販売したりする可能性のある Web サイトではなく、My Great Bank に移動することを確認したいと考えています。 また、自分の銀行口座情報が暗号化されていることを確認したいと考えています。
   >
   >   ブラウザー（クライアント）が MyGreatBank.com （サーバー）に接続すると、TLS は MyGreatBank.com からの証明書を要求して、その ID を検証します。 証明書は次のような認証局によって提供されます。 [!DNL DigiCert] または [!DNL Thawte]. ブラウザーは認証局を信頼するので、接続を許可します。
>
>* **相互 TLS**:MySoftware.com は、MyGreatBank.com API からの情報を必要とするソフトウェアクライアントです。 MyGreatBank では、信頼できるクライアントだけがサーバに接続できます。 したがって、MyGreatBank.com の ID を確認する通常の TLS に加え、TLS/認証局プロセスも MySoftware.com からの要求を検証します。


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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

&#42;&#42;詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 次の項目を指定： [!DNL Workfront Fusion] 公開証明書


HTTP リクエストを使用して Web サービスに接続する場合、通常、Web サービスには [!DNL Workfront Fusion] 検証用の公開証明書。 これにより、Web サービスは、HTTP 要求で提示された証明書をファイル上の証明書と比較し、証明書が Web サービスの上にあることを確認でき許可リストます。

を参照してください。 [!DNL Adobe Workfront Fusion] 公開証明書を web サービスに送信する場合は、web サービスのドキュメントを参照してください。

>[!NOTE]
>
>証明書に加えて、その他の情報も指定する必要が生じる場合があります。 Web サービスに必要な情報について詳しくは、Web サービスの API ドキュメントを参照してください。

次のリンクを使用して、Workfront Fusion の公開証明書をダウンロードできます。

### 2023 年 5 月 25 日～2024 年 6 月 9 日の証明書

>[!IMPORTANT]
>
>* これら [!DNL Workfront Fusion] 公開証明書の有効期限は 2024 年 6 月 9 日です。 有効期限が切れたら、新しい証明書を Web サービスにアップロードする必要があります。 以下をお勧めします。
   >
   >   * 有効期限をメモしておき、自分で証明書を Web サービスにアップロードするようにリマインダーを設定します。
   >   * 新しい証明書を簡単に見つけるには、このページをブックマークします。
>
* ワイルドカード以外の mTLS 証明書です。
>

* [ダウンロード [!DNL Workfront Fusion] 証明書 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [ダウンロード [!DNL Workfront Fusion] EU 証明書 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

   EU で使用

### 2022 年 11 月 14 日～2023 年 7 月 15 日の証明書

>[!IMPORTANT]
>
>* これら [!DNL Workfront Fusion] 公開証明書の有効期限は 2023 年 7 月 15 日です。
>* ワイルドカード mTLS 証明書です。


* [ダウンロード [!DNL Workfront Fusion] 証明書 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [ダウンロード [!DNL Workfront Fusion] EU 証明書 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   EU で使用

## での相互 TLS の有効化 [!DNL Workfront Fusion] HTTP モジュール

すべて [!DNL Workfront Fusion] [!UICONTROL HTTP] リクエストモジュールで相互 TLS を有効にするオプションがあります。

内で相互 TLS を有効にするには [!UICONTROL HTTP] リクエストモジュール：

1. を追加します。 [!UICONTROL HTTP] リクエストモジュールをシナリオに追加します。
1. モジュールの設定を開始します。

   を設定する手順については、 [!UICONTROL HTTP] リクエストモジュールについては、次の該当する記事を参照してください： [[!UICONTROL HTTP] モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 有効にする **[!UICONTROL 詳細設定を表示]** モジュールの下部付近にある。
1. 有効にする **[!UICONTROL 相互 TLS を使用]**.
