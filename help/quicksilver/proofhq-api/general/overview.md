---
title: 概要
description: 概要
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 99%

---

# 概要

**Workfront Proof API へようこそ**

Workfront Proof API は、SSL を使用して保護されるシンプルな HTTP サービスです。この API の目的は、アドビのアプリケーションで使用されるすべての機能を提供することにあります。

## サポートされる形式

パブリックインターフェイスは、SOAP 1.1 に準拠しており、WSDL のサポートに対応しています。したがって、すべてのリクエストは HTTPS 経由で XML を使用して実行されます。

## API バージョン管理

既存のクライアント統合との互換性を維持するために、12.1 リリースから API バージョン管理が導入されました。詳細情報は、[API のアップデート](https://api.proofhq.com/new-updates.html)ページを参照してください。メソッドまたはパラメーターにバージョン情報がない場合は、これが標準 API の一部として含まれていることを意味します。以下の「API の概要」の節を参照してください。

## API の概要

API エントリポイントは次の通りです。

`https://soap.proofhq.com/soap`（HTTPS の使用法に注意してください）

WSDL は次の場所にあります。

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**この WSDL には、12.1 リリースまでのすべての変更が含まれています。その後、API バージョン管理が導入されました。様々な WSDL バージョンと今後の変更点に関する詳細情報は、API のアップデートのページを参照してください**

すべての API リクエストにはセッションキーが必要です。このセッションキーは、アクションを実行している Workfront Proof ユーザーを識別するもので、doLogin() メソッドを呼び出し、ユーザーのメールアドレスとパスワードを渡すことで取得されます。doLogin() メソッドは、一連の API リクエストの前に 1 回だけ呼び出す必要があります。セッションキーは、短時間アクティブなままで、メソッド呼び出しのたびに更新されます。*近日中に、トークンベースの認証のサポートが追加されます。*

すべてのリクエストでは、エンベロープ、ヘッダーおよび本文の形式が使用されます。

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

