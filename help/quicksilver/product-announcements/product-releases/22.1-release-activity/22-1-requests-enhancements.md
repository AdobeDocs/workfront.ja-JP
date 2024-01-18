---
title: 22.1 リクエストの機能強化
description: 22.1 リクエストの機能強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 22.1 リクエストの機能強化

このページでは、プレビュー環境の 2.1 リリースでおこなわれたすべての要求の機能強化について説明します。 これらの機能強化は、実稼動環境で利用できるようになります

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022 年 1 月 17 日の週。

22.1 リリースで使用可能なすべての変更点の一覧については、 [22.1 リリースの概要](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## リクエストを作成するためのアクセス権を持たないユーザーのインターフェイスが改善されました

リクエストを処理する際のユーザーエクスペリエンスを向上させるために、リクエストを作成するアクセス権がないことをログインユーザーに示すインターフェイスが改善されました。 この改善により、イシューを作成するアクセス権を持たないユーザーに対しては、「新しいリクエスト」ボタンが淡色表示になります。 淡色表示のボタンにカーソルを合わせると、Workfront管理者が現在のユーザーのリクエスト作成へのアクセスを制限したことを示すツールヒントが表示されます。

この機能強化以前は、これらのユーザーの「リクエスト」領域に「新しいリクエスト」ボタンが表示されていませんでした。 リクエストを新規としてコピーして送信することも制限されます。

リクエストの作成について詳しくは、 [Adobe Workfront要求の作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md).

## リクエストのコピーと送信

リクエストの送信プロセスを最適化するために、既存のリクエストをコピーして新しいリクエストとして送信できる新しい機能が追加されました。 これは、類似したリクエストを頻繁に送信する場合に役立ちます。 この場合、既存のリクエストを再利用し、いくつか変更を加えて、新しいリクエストとして送信できます。

この変更により、他のユーザーが送信したリクエストを表示できるユーザーも、そのリクエストをコピーして新規として送信できます。 リクエストキュープロジェクトの次の設定を更新すると、この処理を防ぐことができます。同じ会社のユーザーは、すべてのリクエストに対して同じ権限を継承します。

>[!NOTE]
>
>この機能がリリースされる前に、キュートピックのない要求キューに送信された問題をコピーして再送信することはできません。

詳しくは、 [リクエストのコピーと送信](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## リクエスト領域の「Submitted」セクションの Summary パネルエクスペリエンスを更新しました。

>[!NOTE]
>
>この機能は、2021 年 11 月 13 日にプレビュー環境から一時的に削除されました。 後日再度追加されます。

Summary パネルとの表示やインタラクションを改善するために、「Requests」領域の「Submitted」セクションにある「Open Summary」アイコンにラベルを追加しました。 ラベルは動的になり、パネルが開いているか閉じているかに応じて更新されます。

要求を選択せずに概要パネルを開くと、より使いやすい画像が表示され、パネルを開く前に項目を選択するようにユーザーに明確に指示できるようになりました。 詳しくは、 [送信された要求を見つける](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

この変更により、タスク、問題およびドキュメントの概要パネルも更新されました。 概要パネルについて詳しくは、 [概要の概要](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
