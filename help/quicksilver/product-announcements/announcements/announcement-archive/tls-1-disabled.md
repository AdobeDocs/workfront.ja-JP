---
content-type: reference
navigation-topic: announcements
title: Adobe Workfront で必要な TLS 1.2
description: 最適なセキュリティを提供するために、Adobe Workfront では、TLS 1.0 以前に依存するすべてのブラウザー接続と API 統合を、TLS 1.2 を使用するようにアップグレードする必要があります。プレビュー環境では、TLS 1.0 はすでに無効になっています。
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: ht
source-wordcount: '367'
ht-degree: 100%

---

# Adobe Workfront で必要な TLS 1.2

最適なセキュリティを提供するために、Adobe Workfront では、TLS 1.0 以前に依存するすべてのブラウザー接続と API 統合を、TLS 1.2 を使用するようにアップグレードする必要があります。プレビュー環境では、TLS 1.0 はすでに無効になっています。

Workfront は TLS 1.0 のサポートを 2018年3月（PT）に正式に終了しました。TLS 1.0 を利用したすべての統合は、2019年1月9日（PT）をもって機能しなくなりました。TLS 1.1 は 2019年第 4 四半期に無効化されます。

以下の節では、これらの重要なマイルストーンの詳細と、組織内でこのアップグレードに備える方法を説明します。

## Workfront は TLS 1.0 の正式なサポートを終了します（2018年3月5日（PT））

Workfront は 2018年3月（PT）に TLS 1.0 の公式サポートを終了しました。

TLS 1.0 を利用するブラウザー接続と API 統合は、引き続き動作しますが、Workfront は TLS 1.0 に関連する Workfront アプリケーションのイシューを解決しません。

## Workfront TLS 1.0 を使用した統合が無効化（2019年1月9日（PT））

2019年1月9日（PT）に、TLS 1.0 に依存するすべての Workfront ブラウザー接続と API 統合を、TLS 1.1 を使用するようにアップグレードする必要があります。TLS 1.0（インバウンド接続またはアウトバウンド接続）を引き続き利用するブラウザー接続および API 統合は、今回以降、Workfront アプリケーションとの通信ができなくなります。 

## TLS 1.1 は 2019年第 4 四半期に無効化予定

実稼動環境では、TLS 1.1 は 2019年10月21日（PT）に無効になりました。この後は、TLS 1.1 を使用するすべての統合は機能しなくなります。

この変更は、組織がシャットオフに備えるのに役立つように、8月7日（PT）にプレビュー環境とサンドボックス環境で有効になります。

## TLS アップグレードの準備

* [ブラウザーを介して Workfront にアクセスする場合](#when-accessing-workfront-via-the-browser)
* [API を介して Workfront に接続する場合](#when-connecting-to-workfront-via-the-api)

### ブラウザーを介して Workfront にアクセスする場合 {#when-accessing-workfront-via-the-browser}

組織内のユーザーが、サポートされているブラウザーを介して Workfront にアクセスしていることを確認します。（サポートされているブラウザーについて詳しくは、[Adobe Workfront ブラウザーの要件](../../../workfront-basics/workfront-browser-requirements.md)を参照してください。）

Workfront でサポートされているすべてのブラウザーは、TLS 1.2 と互換性があります。

### API を介して Workfront に接続する場合 {#when-connecting-to-workfront-via-the-api}

API（インバウンドまたはアウトバウンド）を介してサードパーティのアプリケーションを Workfront に統合する場合は、統合で TLS 1.2（および TLS 1.2 暗号化プロトコル）が有効になっていることを確認します。
