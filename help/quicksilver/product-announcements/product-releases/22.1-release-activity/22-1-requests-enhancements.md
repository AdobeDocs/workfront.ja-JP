---
title: 22.1 リクエストの機能強化
description: 22.1 リクエストの機能強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
TQID: https://experienceleague.adobe.com/AmKIQPLxnJW4nPNdIEUlnMvUlxMbh4jquWpFYz0k6qY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 456
ht-degree: 100%

---

# 22.1 リクエストの機能強化

このページでは、プレビュー環境の 22.1 リリースで行われたすべてのリクエストの機能強化について説明します。 これらの機能強化は、

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日（PT）の週。

22.1 リリースで使用可能なすべての変更点の一覧については、[22.1 リリースの概要](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md)を参照してください。

## リクエストを作成するためのアクセス権がないユーザー向けのインターフェイスの改善

リクエストを処理する際のユーザーエクスペリエンスを向上させるために、リクエストを作成するためのアクセス権がないことをログインユーザーに示すインターフェイスに改善しました。 この改善により、イシューを作成するためのアクセス権がないユーザーに対しては、「新規リクエスト」ボタンが淡色表示になります。 淡色表示のボタンにポインタを合わせると、Workfront 管理者が現在のユーザーのリクエスト作成へのアクセスを制限したことを示すツールヒントが表示されます。

この機能強化以前は、これらのユーザーのリクエストエリアに「新規リクエスト」ボタンが表示されていませんでした。 リクエストを新規としてコピーおよび送信することも制限されます。

リクエストの作成について詳しくは、[Adobe Workfront リクエストを作成して送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

## リクエストのコピーと送信

リクエストの送信プロセスを最適化するために、既存のリクエストをコピーして新しいリクエストとして送信できる新機能を導入しました。 これは、類似したリクエストを頻繁に送信する場合に役立ちます。 この場合、既存のリクエストを再利用し、いくつか変更を加えて、新しいリクエストとして送信できます。

この変更により、他のユーザーが送信したリクエストを表示できるユーザーも、そのリクエストをコピーして新規として送信できます。 リクエストキューのプロジェクトで、「同じ会社のユーザーはすべてのリクエストに対して同じ権限を継承」の設定を更新すると、この処理を防ぐことができます。

>[!NOTE]
>
>この機能がリリースされる前は、キュートピックのないリクエストキューに送信されたイシューをコピーして再送信することはできません。

詳しくは、[リクエストをコピーして送信](../../../manage-work/requests/create-requests/copy-and-submit-requests.md)を参照してください。

## リクエストエリアの「送信済み」セクションの更新された概要パネルエクスペリエンス

>[!NOTE]
>
>この機能は、2021年11月12日（PT）にプレビュー環境から一時的に削除されました。 後日再度追加される予定です。

視認性と概要パネルのインタラクションを改善するために、リクエストエリアの「送信済み」セクションにある概要を開くアイコンにラベルを追加しました。 このラベルは動的になり、パネルが開いているか閉じているかに応じて更新されます。

先にリクエストを選択せずに概要パネルを開くと、より使いやすい画像が表示され、パネルを開く前に項目を選択するようユーザーに明確に指示するようになりました。 詳しくは、[送信済みリクエストを見つける](../../../manage-work/requests/create-requests/locate-submitted-requests.md)を参照してください。

この変更により、タスク、イシューおよびドキュメントの概要パネルも更新されました。 概要パネルについて詳しくは、[概要の概要](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください。
