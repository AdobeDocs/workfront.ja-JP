---
title: 23.2 リソース管理の機能強化
description: 23.2 リソース管理の機能強化
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '271'
ht-degree: 100%

---

# 23.2 リソース管理の機能強化

このページでは、プレビュー環境の 23.2 リリースで行われたリソース管理のすべての機能強化について説明します。これらの機能強化は、23.2 リリースで実稼動環境での利用ができるようになります。

23.2 リリースサイクルの、現時点で利用可能なすべての変更点のリストについては、[23.2 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md)を参照してください。

## ユーザー処理能力を正確に計算する「作業時間」フィールドの紹介

>[!NOTE]
>
>プレビューリリース：2023年2月16日（PT）、実稼動環境リリース予定日：2023年3月2日（PT）

リソース管理者が、ユーザーの空き時間や、ユーザーが実際のプロジェクト関連作業に費やした時間を正確に計算できるように、Adobe Workfront に作業時間の概念を導入しました。

各ユーザーのプロファイルを作成または編集する際に、「作業時間」フィールドの値を定義できます。詳しくは、[ユーザーのプロファイルの編集](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

「作業時間」フィールドは、ユーザーが実際の作業に使用できる（オーバーヘッドを含まない）フルタイム相当の（FTE）時間の割合を表します。作業時間 には 0 と1 の値で 10 進数を指定する必要があります。例えば、実際の作業可能時間が 20%の場合は 0.2 になります。

フィールドのデフォルト値は 1 で、これはユーザーが FTE 時間全体を実際のプロジェクト関連の作業に費やすことを示します。

この更新の結果、Workfront は、リソース管理環境設定エリアでの選択に応じて、以下の数式を使用してユーザーの空き時間を計算します。

* デフォルトのスケジュール:
* ユーザー処理能力 = [（スケジュール時間 – スケジュール例外） * FTE - 休暇] * 作業時間
* ユーザーのスケジュール：
* ユーザー処理能力 = （スケジュール時間 - スケジュール例外 - 休暇） * 作業時間。

詳しくは、[[!UICONTROL リソース管理]環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3415608/){target=_blank}
