---
content-type: release-notes
title: Adobe Workfrontの2026年第2四半期のリリースアクティビティの制限付き機能
description: これは、2026年第2四半期のAdobe Workfrontの制限付き機能のリリースアクティビティです。
author: Lisa
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 32c616b2-5bba-434e-9918-c27f6518693d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 5%

---

# Adobe Workfront の限定提供機能に関する 2026年第 2 四半期のリリースアクティビティ

この記事では、2026年第2四半期中にリリースされるWorkfront機能の限定提供について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront向けにリリースされたすべての制限付き機能の一覧については、[Adobe Workfront制限付き機能リリースアクティビティ：記事インデックス &#x200B;](/help/quicksilver/product-announcements/product-releases/limited-availability-release-activity/limited-availability-release-activity-article-index.md)を参照してください。

## 制限付き機能のリリースノート

この節には、新機能のリリースノートが含まれています。

### タスクを1回割り当てたり一括割り当てたりする際のエクスペリエンスを更新しました

>[!NOTE]
>
>プロダクションリリース日：2026年2月12日（PT）

単一のタスクを編集したり、一括編集したりする場合は、タスクを編集ボックスの「割り当て」セクションを更新しました。

タスクにリソースを割り当てるための新しいエクスペリエンスがあります。 これは、1つのタスクを編集する場合と、複数のタスクを一括編集する場合の両方で使用できるようになりました。 「割り当て」セクションに次のフィールドを追加しました。

* 割り当て
* 所有者またはタスク所有者
* 割り当て先の役割

詳しくは、[タスクを編集](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

### 人員配置プランの請求率の保持

>[!NOTE]
>
>プロダクションリリース日：2026年3月5日（PT）

スタッフ計画の詳細ページの「財務」セクションに「**請求を保持**」フィールドを追加しました。

このフラグをFalse （off）に設定すると、請求レートは保持されず、請求レートの計算にレート階層が使用されます。

このフラグがTrue （on）に設定されている場合：

* 人員配置プランで割り当てられたリソースの現在の請求レートは保持され、階層内のレートの変更は人員配置プランのリソース領域には反映されません。
* 「リソース」テーブルに新しい行を追加すると、請求料率の階層から得られる初期請求率が保持されます。
* フラグがオンになる前にユーザーが請求レート値を手動で上書きした場合、上書きレートは保持されます。 フラグをオンにすると、手作業による請求レートの上書きは許可されません。

保存が有効になると、オフにすることはできません。

フラグがオンになっているスタッフ配置プランをコピーすると、そのコピーでフラグが自動的にオフになります。 リソース管理者は、新しい人員配置プランで必要な場合は、フラグをオンにする必要があります。

<!--
### Title

>[!NOTE]
>
>Production release date: MONTH DAY, 2026

text
-->

<!--

## Maintenance Updates for limited availability features

This section describes the issues fixed in the weekly Workfront updates for limited availability features.



### Maintenance Updates week of March 1-7, 2026

**Title**

text

### Maintenance Updates week of March 8-14, 2026

**Title**

text

### Maintenance Updates week of March 15-21, 2026

**Title**

text
-->
