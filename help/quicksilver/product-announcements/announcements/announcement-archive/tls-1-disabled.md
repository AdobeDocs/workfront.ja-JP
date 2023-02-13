---
content-type: reference
navigation-topic: announcements
title: Adobe Workfrontで必要な TLS 1.2
description: 最適なセキュリティを提供するために、Adobe Workfrontでは、TLS 1.2 を使用するために、TLS 1.0 以前に依存するすべてのブラウザー接続および API 統合をアップグレードする必要があります。プレビュー環境では、TLS 1.0 は既に無効になっています。
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Adobe Workfrontで必要な TLS 1.2

最適なセキュリティを提供するために、Adobe Workfrontでは、TLS 1.0 以前に依存するすべてのブラウザー接続および API 統合を TLS 1.2 を使用するようにアップグレードする必要があります。 プレビュー環境では、TLS 1.0 は既に無効になっています。

Workfrontは TLS 1.0 のサポートを 2018 年 3 月に正式に終了しました。 TLS 1.0 を利用したすべての統合は、2019 年 1 月 9 日 (PT) より機能しなくなりました。  TLS 1.1 は 2019 年第 4 四半期に無効化されます。

以下の節では、これらの重要なマイルストーンの詳細と、組織でこのアップグレードに備える方法を説明します。

## Workfrontは TLS 1.0 の正式なサポートを終了します（2018 年 3 月 6 日）

Workfrontは 2018 年 3 月に TLS 1.0 の公式サポートを終了しました。

TLS 1.0 を利用するブラウザー接続と API 統合は、引き続き動作しますが、Workfrontは TLS 1.0 に関連するWorkfrontアプリケーションの問題を解決しません。

## Workfront TLS 1.0 を使用した統合が無効になりました（2019 年 1 月 10 日）

2019 年 1 月 10 日に、TLS 1.1 以降を使用するには、TLS 1.0 を利用するすべてのWorkfrontブラウザー接続および API 統合をアップグレードする必要があります。 TLS 1.0（インバウンド接続またはアウトバウンド接続）を引き続き利用するブラウザー接続および API 統合は、今回以降、Workfrontアプリケーションとの通信はできなくなります。 

## TLS 1.1 は 2019 年第 4 四半期に無効化予定

実稼動環境では、TLS 1.1 が 2019 年 10 月 21 日に無効になりました。 この時間が経過すると、TLS 1.1 を使用するすべての統合は機能しなくなります。

この変更は、8 月 7 日のプレビューとサンドボックス環境で有効になり、組織がシャットオフの準備に役立ちます。

## TLS アップグレードの準備

* [ブラウザーを使用してWorkfrontにアクセスする場合](#when-accessing-workfront-via-the-browser)
* [API を介してWorkfrontに接続する場合](#when-connecting-to-workfront-via-the-api)

### ブラウザーを使用してWorkfrontにアクセスする場合 {#when-accessing-workfront-via-the-browser}

組織内のユーザーが、サポートされているブラウザーを使用してWorkfrontにアクセスしていることを確認します。 ( サポートされているブラウザーについて詳しくは、 [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).)

Workfrontでサポートされているすべてのブラウザーは、TLS 1.2 と互換性があります。

### API を介してWorkfrontに接続する場合 {#when-connecting-to-workfront-via-the-api}

API（インバウンドまたはアウトバウンド）を介してサードパーティのアプリケーションをWorkfrontに統合する場合は、統合で TLS 1.2（および TLS 1.2 暗号化プロトコル）が有効になっていることを確認します。
