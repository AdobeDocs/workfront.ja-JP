---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 ベータ リリースアクティビティ
description: このページでは、2017.2 ベータ 2 リリースに関してプレビュー環境で使用できるすべての変更について説明します。このページの機能は、2017年5月24日（PT）にプレビュー環境で使用できるようになりました。2018年7月下旬から8月上旬（PT）までの間に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 100%

---

# 2017.2 ベータ リリースアクティビティ

このページでは、2017.2 ベータ 2 リリースに関してプレビュー環境で使用できるすべての変更について説明します。このページの機能は、2017年5月24日（PT）にプレビュー環境で使用できるようになりました。2018年7月下旬から8月上旬（PT）までの間に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017.2 に実装されたすべての変更のリストについては、[2017.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)を参照してください。

2017.2 ベータ 2 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け：**

* [API 機能強化：イベント登録](#api-enhancement-event-subscriptions)

**すべてのユーザー向け：**

* [プロジェクトに登録](#subscribe-to-projects)
* [メールから項目を登録解除](#unsubscribe-from-items-from-email)
* [ガントチャートのマイルストーンの表示方法を設定](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [ソースプールのテンプレート](#resource-pools-templates)
* [Workfront 内でプルーフ済みドキュメントのバージョンを表示](#view-versions-of-proofed-documents-within-workfront)
* [プルーフ承認レポートの新規「リクエスター」オブジェクト](#new-requester-object-in-proof-approval-report)

## API 機能強化：イベント登録 {#api-enhancement-event-subscriptions}

イベント登録でサポートされている Workfront オブジェクトでアクションが発生した際に、目的のエンドポイントに応答を送信するように Workfront を設定できるようになりました。これにより、使用中の統合システムと Workfront API をリアルタイムで連携できるようになります。

詳しくは、[イベント登録の API](../../../../wf-api/general/event-subs-api.md) を参照してください。

## プロジェクトに登録 {#subscribe-to-projects}

プロジェクトチームに属していないプロジェクトに対する新しいコメントを登録できるようになりました。このリリース以前は、イシューとタスクに関するコメントのみを登録できました。

項目の登録について詳しくは、[Adobe Workfront で項目に登録](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)を参照してください

## メールからアイテムの登録解除 {#unsubscribe-from-items-from-email}

登録メール内の「登録解除」リンクを使用して、項目を登録解除できます。以前は、Workfront インターフェイスからのみ項目を登録解除できました。

登録中のメールの登録解除について詳しくは、[Adobe Workfront 通知](../../../../workfront-basics/using-notifications/wf-notifications.md)のメール通知のオプトアウトの節を参照してください。

## ガントチャートでのマイルストーンの表示方法を設定 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***修正&#x200B;**：この機能は現在、プレビューサンドボックス環境で使用することはできません。2017年6月中（PT）にリリースされる予定です。*

ガントチャートでマイルストーン情報を表示するオプションは 2 つあります。次のマイルストーンインジケーターのいずれかまたは両方を設定できます。

* マイルストーンダイヤモンド（アイコン）

  このアイコンは、ガントチャートでマイルストーンに関連付けられたタスクの後に表示されます。

* マイルストーン線

  ガントチャートのすべてのタスクにわたって、マイルストーンに関連付けられたタスクの後に線が表示されます。

この変更が行われる前は、ガントチャートにマイルストーンを表示するためのオプション（名称「マイルストーン」）は 1 つのみでした。このオプションでは、マイルストーンのひし形アイコンとの線の両方が有効になりました。これらのインジケーターは分離できませんでした。すべてのプロジェクトリストとレポートを含むすべてのガントチャートで、2 つのオプションを使用できるようになりました。 

ガントチャートにおける情報の表示方法の設定について詳しくは、[ガントチャートでの情報の表示方法を設定](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

## リソースプールのテンプレート {#resource-pools-templates}

テンプレートのリソースプールを指定できるようになりました。このリリース以前は、リソースプールをユーザーおよびプロジェクトにのみ関連付けることができました。

リソースプールについて詳しくは、[リソースプールの概要](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください

## Workfront 内でプルーフ済みドキュメントのバージョンを表示 {#view-versions-of-proofed-documents-within-workfront}

Workfront インターフェース内で、プルーフ済みドキュメントのすべてのバージョンのプルーフを表示できるようになりました。 

この変更が行われる前は、プルーフ済みドキュメントの最新バージョンのみを表示できました。

プルーフライセンスを持たないユーザーは、以下の操作を実行できます。

* プルーフ済みドキュメントの前のバージョンでプルーフを開く

プルーフライセンスを持つユーザーは、以下の操作を実行できます。

* プルーフ済みドキュメントの前のバージョンでプルーフを開く
* プルーフ済みドキュメントの前のバージョンに関するプルーフの詳細を表示

詳しくは、[ドキュメントバージョンを管理](../../../../documents/managing-documents/manage-document-versions.md)にある[ドキュメントバージョンを管理](../../../../documents/managing-documents/manage-document-versions.md)を参照してください。

## プルーフ承認レポートの新規「リクエスター」オブジェクト {#new-requester-object-in-proof-approval-report}

プルーフの承認レポートを作成すると、新しいリクエスターオブジェクトが追加されます。このオブジェクトを使用すると、プルーフの承認をリクエストしたユーザーに関する情報をレポートできます。 

プルーフの承認レポートの新しいリクエスターオブジェクトには、他のタイプのオブジェクトレポートの既存のユーザーオブジェクトで使用できるフィールドがすべて含まれています。

>[!NOTE]
>
>この情報は、この機能がそれぞれのプレビュー環境または実稼動環境に初めて導入された時点からのレポートでのみ入手できます。この機能が導入される前のリクエスターオブジェクトに関するレポートでは、情報は利用できません。

[カスタムレポートを作成](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)で説明されているように、プルーフの承認レポートを作成する際に、リクエスターオブジェクトにアクセスします。

プルーフの承認オブジェクトレポートについて詳しくは、[Adobe Workfront のオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)にある [Adobe Workfront のオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の節を参照してください。
