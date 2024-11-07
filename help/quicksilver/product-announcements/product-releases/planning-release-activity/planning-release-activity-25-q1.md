---
content-type: release-notes
title: 25.1 リリースのAdobe Workfront計画リリースアクティビティ
description: これは、2025 年第 1 四半期のAdobe Workfront Planning 製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: f30bed961b339e20c0693a8b5e485f872375b688
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 4%

---

# Adobe Workfront Planning の 2025 年第 1 四半期リリースアクティビティ

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfront からの新しいオファーである Adobe Workfront Planning を説明するものです。
>
>Workfront Planning 機能にアクセスして使用するには、Workfront プランに加えて、Workfront Planning プランを購入する必要があります。
>
>Workfront Planning へのアクセス要件の完全なリストについては、[ アクセスの概要 ](/help/quicksilver/planning/access/access-overview.md) を参照してください。
>Workfront計画の概要については、[Adobe Workfront計画の概要 ](/help/quicksilver/planning/general/planning-overview.md) を参照してください。
>

この記事では、2025 年第 1 四半期のリリースでWorkfront Planning でリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

2024 年 8 月 28 日（PT）の一般リリース後にAdobe Workfront Planning でリリースされたすべての機能のリストについては、[Adobe Workfront Planning リリースアクティビティ：記事索引 ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md) を参照してください。

## リクエストフォームで接続フィールドがサポートされるようになりました

>[!NOTE]
>
>プレビューリリース：2024 年 10 月 31 日（PT）、高速リリースの実稼動：24.11 リリースの実稼動（2024 年 11 月 14 日（PT））、四半期リリースの実稼動：25.1 リリースの実稼動（2025 年 1 月）

レコードタイプのリクエストフォームに、Workfront Planning レコードの接続されたフィールドを追加できるようになりました。

リクエストフォームに、接続検索フィールドやWorkfront オブジェクトの接続フィールドを追加することはできません。

この機能強化が行われるまで、これらのタイプのフィールドは、Workfront Planning のリクエストフォームに追加できませんでした。

詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

## 他のレコードに既にリンクされているレコードを接続する場合の接続警告

>[!NOTE]
>
>プレビューリリース：2024 年 10 月 31 日（PT）、高速リリースの実稼動：24.11 リリースの実稼動（2024 年 11 月 14 日（PT））、四半期リリースの実稼動：25.1 リリースの実稼動（2025 年 1 月）

別の場所で既に接続されていて、[ 一対多 ] または [ 一対一 ] 接続タイプを介して接続されたレコード タイプに属するレコードを接続しようとすると、レコードが既に接続されているという警告が表示されるようになりました。 接続を続行することを確認すると、選択したレコードが元のレコードから削除され、現在編集中のレコードに追加されます。

接続タイプについて詳しくは、[ 接続されたレコードタイプの概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

## 新しい情報アイコンと、レコードの詳細ページのフィールドの説明

>[!NOTE]
>
>プレビューリリース：2024 年 10 月 30 日（PT）、高速リリースの実稼動：24.11 リリースの実稼動（2024 年 11 月 14 日（PT））、四半期リリースの実稼動：25.1 リリースの実稼動（2025 年 1 月）

レコードページのフィールド名の右側に情報アイコンを追加しました。 説明が存在する場合、情報アイコンをクリックすると、フィールドの説明が表示されます。 この機能強化の前は、フィールド名にカーソルを合わせると、フィールドの説明が表示されていました。

詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

## Planning 接続用の新しいWorkfront フィールド タイプ

>[!NOTE]
>
>プレビューリリース：2024 年 10 月 24 日（PT）、高速リリースの実稼動：24.11 リリースの実稼動（2024 年 11 月 14 日（PT））、四半期リリースの実稼動：25.1 リリースの実稼動（2025 年 1 月）

Workfront オブジェクトを引き続きWorkfront Planning レコードにブリッジするために、Workfront カスタムフォームに新しいフィールドタイプを追加しました。このフィールドタイプは「Planning connection」です。 このフィールドタイプをWorkfrontのカスタムフォームに追加し、最終的にWorkfront オブジェクトに追加すると、次の操作を実行できるようになります。

* Workfront オブジェクトに接続されているレコードをカスタムフォームに表示します。

* Workfront Planning レコードをWorkfront オブジェクトから接続して切断します。

すべてのオブジェクトタイプのフォームに新しいフィールドを追加できます。 ただし、フィールドの情報を編集できるのは、Workfront Planning のレコードタイプ（Portfolio、プログラム、プロジェクト、会社、グループ）から接続できるWorkfront オブジェクトに添付されたフォームからのみです。

Workfront オブジェクトの Planning 接続フィールドの一括編集はまだ使用できません。

詳しくは、[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3435633/){target=_blank}