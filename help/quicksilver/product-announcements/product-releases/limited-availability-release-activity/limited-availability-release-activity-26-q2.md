---
content-type: release-notes
title: Adobe Workfrontの限定提供機能に関する 2026 年第 2 四半期のリリースアクティビティ
description: これは、2026 年第 2 四半期のAdobe Workfrontの限定提供機能のリリースアクティビティです。
author: Lisa
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 32c616b2-5bba-434e-9918-c27f6518693d
source-git-commit: caad1c709da790e28df39a4a6092ef1ebfa42357
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 5%

---

# Adobe Workfront の限定提供機能に関する 2026年第 2 四半期のリリースアクティビティ

この記事では、2026 年第 2 四半期にリリースされる、Workfrontの限定提供機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront向けにリリースされている限定提供（LA）機能の一覧については、[Adobe Workfront限定提供（LA）機能のリリースアクティビティ：記事インデックス &#x200B;](/help/quicksilver/product-announcements/product-releases/limited-availability-release-activity/limited-availability-release-activity-article-index.md) を参照してください。

## 限定提供の機能のリリースノート

この節では、新機能のリリースノートを示します。

### タスクを単一または一括割り当てする際のエクスペリエンスを更新しました

>[!NOTE]
>
>実稼動リリース日：2026 年 2 月 12 日（PT）

単一のタスクの編集時または一括編集時に、「タスクを編集」ボックスの「割り当て」セクションを更新しました。

タスクにリソースを割り当てる新しいエクスペリエンスが追加されました。 この機能は、1 つのタスクを編集する場合でも、複数のタスクを一括編集する場合でも使用できるようになりました。 「割り当て」セクションに次のフィールドを追加しました。

* 割り当て
* 所有者またはタスク所有者
* 割り当て先の役割

詳しくは、[タスクを編集](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

### スタッフプランの請求レートの保持

>[!NOTE]
>
>実稼動リリース日：2026 年 3 月 5 日（PT）

**請求を保持** フィールドを「スタッフプランの詳細」ページの「財務」セクションに追加しました。

このフラグを False （オフ）に設定すると、請求レートは保持されず、請求レートの計算にレート階層が使用されます。

このフラグを True に設定すると（オン）:

* スタッフ計画に割り当てられたリソースの現在の請求レートは保持され、階層内のレートに対する変更は、スタッフ計画の「リソース」領域には反映されません。
* リソース テーブルに新しい行を追加しても、請求レート階層からの初期請求レートは保持されます。
* フラグをオンにする前にユーザーが請求レート値を手動で上書きした場合、上書きレートは保持されます。 フラグがオンになると、請求レートの手動の上書きは許可されません。

保存機能が有効になると、オフにすることはできません。

フラグがオンになっているスタッフ計画をコピーすると、コピーのフラグは自動的にオフになります。 新しいスタッフ計画でフラグが必要な場合は、リソース管理者がオンにする必要があります。

<!--### Title

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
