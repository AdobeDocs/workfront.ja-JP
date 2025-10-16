---
content-type: release-notes
title: Adobe Workfront Planning の 2026 年第 1 四半期リリースアクティビティ
description: これは、2026 年第 1 四半期のAdobe Workfront Planning 製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: fdfb1ecb61fd85fa927fc7c3443c2a7f23409873
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Adobe Workfront Planning の 2026 年第 1 四半期リリースアクティビティ

この記事では、2026 年第 1 四半期のリリースでWorkfront Planning に対してリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront Planning 用にリリースされたすべての機能の一覧については、[Adobe Workfront Planning リリース アクティビティ：記事一覧 &#x200B;](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md) を参照してください。


## グローバルレコードタイプと、既存のレコードタイプとして他のワークスペースに追加する機能

>[!NOTE]
>
>プレビュー：2025 年 10 月 16 日（PT）
>&#x200B;>実稼動高速リリース：2025 年 11 月 13 日（PT）
>&#x200B;>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

共通のワークフローを持つマルチチーム組織にWorkfront プランニングを実装する場合、各チームのワークスペースに追加できる主要なレコードタイプ（キャンペーンや成果物など）の包括的な構造とメタデータを定義して、チームの作業をキャプチャおよび管理する必要がある場合があります。

また、各チームの作業を中央レベルに展開する必要がある場合もあります。

このようなワークフローでは、組織内の全員をすべてのワークスペースに追加しなくても、チーム間の表示をロック解除しながら、チームが一貫して作業をキャプチャできるようにします。 グローバルレコードタイプを使用すると、これを実現できます。

レコードタイプをグローバルに指定し、複数のワークスペースで使用できるようになりました。 ユーザーは、中央のワークスペースで既に設定されているのと同じフィールド構造および接続を使用できます。

詳しくは、次の記事を参照してください。

* [&#x200B; クロスワークスペースレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [&#x200B; レコードタイプのワークスペース間機能の設定 &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [別のワークスペースからの既存のレコードタイプの追加](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## 1 つのレコードタイプの接続フィールドに対する新しい制限

>[!NOTE]
>
>プレビュー：2025 年 10 月 16 日（PT）
>&#x200B;>実稼動高速リリース：2025 年 11 月 13 日（PT）
>&#x200B;>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

各レコードタイプに対して 30 個の接続フィールドという制限が導入されました。

注意：現在、組織に 1 つのレコードタイプに対して 30 を超える接続フィールドがある場合は、30 の制限を超える追加フィールドを保持できます。 ただし、制限を超えるレコードタイプに接続フィールドを追加することはできません。 今後、新しい制限の 30 個の接続フィールドが適用されます。

詳しくは、[&#x200B; 接続されたレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

## 選択タイプのフィールドの選択肢に対して、ユーザーにわかりやすい値を設定します

>[!NOTE]
>
>プレビュー：2025 年 10 月 16 日（PT）
>&#x200B;>実稼動高速リリース：2025 年 11 月 13 日（PT）
>&#x200B;>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

フィールドの選択肢を 1 つまたは複数選択のフィールドに追加する際に、Workfrontで、各選択肢に一意のわかりやすい値を割り当てるようになりました。 この機能向上が行われる前は、Workfrontが生成した英数字の ID は、API 呼び出しやその他の統合環境では理解および使用が困難でした。

この改善により、次の点が考慮されます。

* 新しい値は、新しいフィールドの選択肢に追加されます。 既存のフィールドの選択肢では、英数字の ID が保持されます。

* 選択肢の値は、1 つのフィールドに対して一意ですが、異なるフィールド間で繰り返すことができます。

* 選択肢の名前を変更しても、元の値は更新されません。

* 複数の単語を選択した場合、選択値は小文字で表示され、アンダースコアで区切られます。 同じフィールドに別の選択名として既に使用されているラベルを使用する場合、Workfrontは値に連番を追加します。

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。