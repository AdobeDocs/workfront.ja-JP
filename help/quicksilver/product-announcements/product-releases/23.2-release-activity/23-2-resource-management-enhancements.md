---
title: 23.2 リソース管理の強化
description: 23.2 リソース管理の強化
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 23.2 リソース管理の強化

このページでは、プレビュー環境の 23.2 リリースでおこなわれた、リソース管理に関するすべての機能強化について説明します。 これらの機能強化は、23.2 リリースで実稼動環境で利用できるようになります。

23.2 リリースサイクルのこの時点で使用可能なすべての変更点のリストについては、 [23.2 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## ユーザー容量を正確に計算する「作業時間」フィールドの紹介

>[!NOTE]
>
>プレビューリリース：2023 年 2 月 16 日、実稼動予定日：2023 年 3 月 2 日

リソースマネージャが、実際のプロジェクト関連の作業に専念するユーザーとアカウントの可用性を正確に計算できるように、Adobe Workfrontに「作業時間」の概念を導入しました。

各ユーザーのプロファイルを作成または編集する際に、各ユーザーの「作業時間」フィールドの値を定義できます。 詳しくは、 [ユーザーのプロファイルの編集](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

「作業時間」フィールドは、実際の作業に使用できるフルタイム相当 (FTE) 時間の割合を表します。オーバーヘッドは含まれません。 Work Time には 0 ～ 1 の値を持つ 10 進数を指定する必要があります。 例えば、実際の作業時間の 20%の可用性は 0.2 となります。

フィールドのデフォルト値は 1 で、ユーザーが FTE 全体を実際のプロジェクト関連の作業に費やすことを示します。

この更新の結果、Workfrontは、「リソース管理」環境設定領域での選択に応じて、以下の数式を使用してユーザーの可用性を計算します。

* デフォルトのスケジュール：
* ユーザー容量= [（スケジュール時間 — スケジュール例外） * FTE — タイムオフ] *勤務時間
* ユーザーのスケジュール：
* ユーザー能力= （スケジュール時間 — スケジュール例外 — タイムオフ） *勤務時間。

詳しくは、 [設定 [!UICONTROL リソース管理] 環境設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3415608/){target=_blank}
