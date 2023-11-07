---
content-type: api
navigation-topic: api-navigation-topic
title: イベント購読証明書
description: イベント購読証明書
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 1%

---

# イベント購読用の Client TLS の設定

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

クライアント TLS を使用すると、受け取ったイベント購読メッセージが実際にAdobe Workfrontから送信されたことを確認できます。 この機能を有効にするには、Workfront x509 証明書を要求および検証するようにサーバーを設定する必要があります。


## Workfrontのクライアント証明書を検証

この手順は、サーバーが TLS 接続を受け入れるように設定されていることを前提としています。 Workfrontは、自己署名証明書をサポートしていません。

一般的に、サーバーのクライアント認証を有効にするには、次の手順が必要です。

1. DigiCert グローバルルート CA 証明書の PEM バージョンをダウンロードします。
1. クライアント証明書の検証をオンにします。

   手順 1 の CA 証明書を信頼済みとして指定します。

1. 証明書は、DigiCert Global Root CA の中間 CA である DigiCert SHA2 Secure Server CA によって実際に署名されるので、検証深度を 2 に設定します。
1. クライアント証明書が実際にWorkfrontからのものであることを確認するには、件名ドメイン名を調べます。

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

詳しくは、 [ngx_http_ssl_module に関する NGiNX ドキュメント](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

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

詳しくは、

* [クライアント認証とアクセス制御](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache モジュール mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## 証明書と環境のマッピング

| WF 環境 | 証明書の共通名 | 証明書の件名 (DN) |
| -- | -- | -- |
| 実稼動 | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| プレビュー | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| サンドボックス 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| サンドボックス 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## 証明書をダウンロード

次のリンクをクリックして、クライアント証明書をダウンロードします。

* [クライアント証明書 — 実稼動環境](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [クライアント証明書 — 環境のプレビュー](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [クライアント証明書 — サンドボックス環境](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>両方のサンドボックス環境で同じクライアント証明書を使用できます。
