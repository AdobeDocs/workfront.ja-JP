---
content-type: reference
navigation-topic: announcements
title: 新しい Adobe Workfront 管理システムでは、リクエストキューの POP メールを 21.1 に置き換える
description: リクエストキューの POP メールオプションを、Adobe Workfront が管理する新しいシステムに置き換えます。 引き続きメールでリクエストを送信できますが、Workfront が管理する新しいメールアドレスをリクエストキューのエリアで設定する必要があります。
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
TQID: https://experienceleague.adobe.com/zzr53eiyA6o-VpZQnFQt-xCXZBKaScZUz8jDmOgX-Ns
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 100%

---

# 新しい Adobe Workfront 管理システムでは、リクエストキューの POP メールを 21.1 に置き換える

リクエストキューの POP メールオプションを、Adobe Workfront が管理する新しいシステムに置き換えます。 引き続きメールでリクエストを送信できますが、Workfront が管理する新しいメールアドレスをリクエストキューのエリアで設定する必要があります。

## POP メールオプションを削除する理由

POP テクノロジーは、信頼性が低く、安全性も低いメールオプションです。 また、特に POP メールに関するお客様の問題も多く見られます。 Workfront が管理するシステムに変更を加えると、より信頼性の高いエクスペリエンスが得られます。

## 実行する必要があるアクション

本番環境で、POP メールで設定したリクエストキューごとに新しいメールアドレスを設定し、必要に応じて新しいメールアドレスを配布する必要があります。 詳しくは、[ユーザーがイシューをリクエストキュープロジェクトにメールで送信できるようにする](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md)を参照してください。

## 移行計画について

2月上旬の 21.1 リリースから、新しく作成した *@intake.workfront.com* のメールアドレスにユーザーを移行するため、60 日の期間が設けられます。 60 日間は、以前使用していた POP メールが引き続き機能します。

## プレビューでテストするには

この変更をプレビューでテストするには、プレビュー環境でメールを有効にする必要があります。 そのためには、[サンドボックスプレビュー環境からのメール配信を有効にする](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)の節にある、プレビューでのメールの管理の手順を参照してください。

>[!IMPORTANT]
>
>ここで設定した内容は、本番環境には引き継がれません。 機能が実稼動環境にリリースされた後、このプロセスを再度実行する必要があります。
