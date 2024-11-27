---
content-type: release-notes
title: 25.1 リリースのAdobe Workfront計画リリースアクティビティ
description: これは、2025 年第 1 四半期のAdobe Workfront Planning 製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: 8d5006532e93dc687beb79e817b725f18b0c65d3
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 3%

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

この記事では、2025 年第 1 四半期のリリースでWorkfront Planning でリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

2024 年 8 月 28 日（PT）の一般リリース後にAdobe Workfront Planning でリリースされたすべての機能のリストについては、[Adobe Workfront Planning リリースアクティビティ：記事索引 ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md) を参照してください。


## 既存のWorkfront フィールドをWorkfront Planning のレコードタイプにインポート

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

これで、レコードタイプにフィールドを追加する際に、既存のWorkfrontのカスタムフィールドまたはネイティブフィールドを読み込んで、選択したレコードタイプに関連付けることができます。 既存のフィールドを読み込むと、Workfront Planning にWorkfront フィールドのコピーが作成されます。 コピーされたフィールドは、元のバージョンとは無関係です。

この機能強化の前は、すべてのフィールドを手動で作成し、レコードタイプに関連付ける必要がありました。

計算フィールドは現時点ではサポートされていません。

詳しくは、[Adobe Workfrontからのフィールドのインポート ](/help/quicksilver/planning/fields/import-fields-from-workfront.md) を参照してください。

## CSV または Excel ファイルの読み込みによるレコードタイプ、レコード、フィールドの作成

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

CSV または Excel ファイルを読み込むことで、新しいレコードタイプを読み込むことができるようになりました。

次の情報が読み込まれます。

* シートまたはファイルの名前がレコードタイプ名として読み込まれます。

* 各列の最初の行が新しいフィールドとして読み込まれます。 読み込まれた各シートには、最大 500 個のフィールドを含めることができます。

* 各行が新しいレコードとして読み込まれます。 各シートには、最大 10,000 件のレコードを含めることができます。

詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## 数式で循環参照を使用しない

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

式フィールドを編集または作成する際に、その式フィールドまたは共有フィールドへの循環参照が発生する可能性がある警告メッセージを導入しました。 自身を参照する数式フィールド、または計算内で参照されている項目を参照する数式フィールドを保存することはできません。

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

## 接続されたビューページをレコードのページに追加して、接続されたレコードをテーブルビューに表示する

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

レコードの詳細領域にページを追加すると、接続されたレコードをテーブル表示に表示できます。 接続されたレコードごとに 1 ページ追加できます。

追加されたページは読み取り専用です。

詳しくは、[ レコードページレイアウトの管理 ](/help/quicksilver/planning/records/manage-the-record-page.md) を参照してください。

## 「要求」エリアの「送信済み」セクションにある新しい「Workfront」タブと「計画」タブ

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

Workfrontの「リクエスト」エリアの「送信済み」セクションで、Workfront Planning リクエストを確認できるようになりました。 送信済みセクションに次のタブが表示されるようになりました。

* Workfront:Workfrontで送信されたリクエストを表示します。
* 計画：Workfront計画要求フォームを使用して送信された要求を表示します。

Workfront Planning レコードタイプにリクエストを追加するには、リクエスト フォームへのリンクを使用する必要があります。 「Workfrontのリクエスト」領域からのWorkfront計画リクエストの送信は、後日利用できるようになります。

「プランニング」タブを「リクエスト」領域で使用するには、Workfront Planning パッケージを購入する必要があります。

詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

## 追加のフィールドタイプがリクエストフォームでサポートされるようになりました

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

Workfront Planning のレコードタイプリクエストフォームに、次のフィールドタイプを追加できるようになりました。

* ユーザー
* Workfront接続

この機能強化が行われるまで、これらのタイプのフィールドは、Workfront Planning のリクエストフォームに追加できませんでした。

詳しくは、Adobe Workfront Planning でのリクエストフォームの作成と管理（/help/quicksilver/planning/requests/create-request-form.md）を参照してください。

## 特定のフィールドタイプを含むリクエストフォームの公開共有を制限する

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 27 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

フォームに次のフィールドタイプのいずれかが含まれている場合、リクエストフォームを公開で共有できなくなりました。

* 式
* WorkfrontとAEM Assetsの接続
* 参照フィールド
* ユーザー

詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。


## カレンダーにレコードを週別に表示

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 26 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

カレンダービューでレコードを週別に表示できるようになりました。 この機能強化の前は、月別にのみカレンダービューを表示できていました。

詳しくは、[ カレンダー表示の管理 ](/help/quicksilver/planning/views/manage-the-calendar-view.md) を参照してください。

## 削除されたレコードを復元

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 22 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

レコードが削除された後、30 日間一時的に「最近削除された項目」 bin に移動されるようになりました。 最近削除された bin には、レコードタイプのページからアクセスでき、特定のタイプのレコードのみが含まれます。

Workspace管理者は、レコードが削除されてから最大 30 日間、ごみ箱からレコードを復元できます。 接続されたレコードとそのフィールド情報も復元されます。

この機能強化が行われるまで、削除されたレコードは復元できませんでした。

詳しくは、「[ 削除されたレコードの復元 ](/help/quicksilver/planning/records/records-information.md)」を参照してください。

## レコードの詳細領域で使用できるAdobeAI アシスタント

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 21 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

作業を簡単に完了できるように、AdobeAI アシスタントをレコードの詳細プレビューまたはレコードのページに追加しました。 レコードページ内で AI アシスタントを使用すると、レコードに関する情報を更新できます。

詳しくは、[Adobe Workfront計画 AI アシスタントの概要 ](/help/quicksilver/planning/general/planning-ai-assistant-overview.md) を参照してください。

## レコードページにサムネールとカバー画像を追加する際の新しいエクスペリエンス

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 20 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

レコードのプレビューまたはページを開き、レコードにサムネールまたはカバー画像がない場合、ヘッダーのレコード名の上の領域にカーソルを合わせて、レコードにカバーとサムネール画像を追加するオプションを表示する必要があります。 この機能強化の前は、サムネールの空のプレースホルダー画像と、レコード名の上に表示されるカバーが表示されていました。

詳しくは、次の記事を参照してください。

* [レコードへのカバー画像の追加](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [レコードへのサムネール画像の追加](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## テーブル表示でのパーセンテージタイプのフィールドの新しい表示タイプ

>[!NOTE]
>
>プレビューリリース：2024 年 11 月 7 日（PT）、高速リリースの実稼動：24.12 リリース（2024 年 12 月）の場合、四半期リリースの実稼動：25.1 リリース（2025 年 1 月）の場合

テーブルビューで数値を読みやすくするために、以下の選択肢から選択して、テーブルビューでのパーセンテージタイプのフィールドの表示方法を変更できるようになりました。

* 数値
* 棒グラフ
* 円

この表示タイプは、テーブル表示でのみサポートされます。

この機能強化の前は、パーセンテージ値を数値としてのみ表示できていました。

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

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
