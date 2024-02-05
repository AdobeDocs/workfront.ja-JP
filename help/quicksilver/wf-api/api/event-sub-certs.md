---
content-type: api
navigation-topic: api-navigation-topic
title: イベント登録証明書
description: イベント登録証明書
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: c547ff323ad9e43472074964ac365447755e4aa5
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 95%

---

# イベント登録用のクライアント TLS の設定

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

クライアント TLS を使用すると、受け取ったイベント登録メッセージが実際に Adobe Workfront から送信されたことを確認できます。この機能を有効にするには、Workfront x509 証明書をリクエストおよび検証するようにサーバーを設定する必要があります。


## Workfront のクライアント証明書を検証

この手順は、サーバーが TLS 接続を受け入れるように設定されていることを前提としています。Workfront は、自己署名証明書をサポートしていません。

一般的に、サーバーのクライアント認証を有効にするには、次の手順が必要です。

1. DigiCert Global Root CA 証明書の PEM バージョンをダウンロードします。
1. クライアント証明書の検証をオンにします。

   手順 1 の CA 証明書を信頼済みとして指定します。

1. 証明書は、DigiCert Global Root CA の中間 CA である DigiCert SHA2 Secure Server CA によって実際に署名されるので、検証の深さを 2 に設定します。
1. 件名のドメイン名を調べることにより、クライアント証明書が実際に Workfront からのものであることを確認します。

## サーバー設定の例

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

詳しくは、[ngx_http_ssl_module に関する NGiNX のドキュメント](https://nginx.org/en/docs/http/ngx_http_ssl_module.html)を参照してください。

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

詳しくは、次を参照してください。

* [Client Authentication and Access Control](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache Module mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## 証明書と環境のマッピング

| WF 環境 | 証明書の共通名 | 証明書の件名（DN） |
| -- | -- | -- |
| 実稼動 | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| プレビュー | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| サンドボックス 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| サンドボックス 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## 証明書のダウンロード

次のリンクをクリックして、クライアント証明書をダウンロードします。

* [クライアント証明書 — 実稼動環境](assets/event_subscription_nov_2023_production.crt)
* [クライアント証明書 — 環境のプレビュー](assets/event_subscription_nov_2023_preview.crt)
* [クライアント証明書 — サンドボックス環境](assets/event_subscription_nov_2023_sandboxes.crt)

>[!NOTE]
>
>両方のサンドボックス環境で同じクライアント証明書を使用できます。
