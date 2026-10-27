---
title: 2027年第1四半期リリースの概要
description: このページでは、2027年第1四半期リリースに含まれる機能に関する情報を提供します。 これらの機能強化は、その四半期を通じて本番動環境で利用できるようになる予定です。
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3c6235a01af5a18a6ab4b2b80bbdea2c447009aa
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 25%
---

# 2027年第1四半期リリースの概要

このページでは、2027年1月に予定されている2027年第1四半期リリースに含まれる機能に関する情報を提供します。

このページの機能強化は、プレビュー環境で利用できます。 このページは、2027年第1四半期のリリースが予定されている実稼動リリースに近づいたときに、さらに機能強化を加えて更新されます。

>[!IMPORTANT]
>
>
>月次リリースと四半期リリースは、特に指定がない限り、毎月第 2 週の木曜日に公開される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>2026.11 （2026年11月12日（PT））</li><li>2026.12 （2026年12月17日（PT））</li><li>2027.01 （2027年1月21日（PT））</li></ul> | <ul><li>2027.01 （2027年1月21日（PT））</li></ul> |
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [プロジェクトの強化](#project-enhancements)


### プロジェクトの強化

<table>
    <tbody>
        <tr>
            <td><strong>機能</strong>
            </td>
            <td><strong>プレビュー</strong></td>
            <td><strong>迅速リリース</strong></td>
            <td><strong>四半期ごと</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">更新の先頭にスレッドをピン留めする</a></p>
                <p>プロジェクト、タスク、イシュー、またはリクエストの更新領域の上部に最も重要なスレッドを固定して、チームに主要な情報を表示できるようにできるようになりました。</p>
            </td>
            <td><p>2026年10月15日（PT）</p></td>
            <td><p>2026年11月12日（PT）</p></td>
            <td><p>2027年1月21日</p></td>
        </tr>
    </tbody>
</table>

## その他のエリアに関するリリースノート

* [Adobe Workfront Fusion リリース アクティビティ &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。
* [Adobe Workfront計画リリース アクティビティ &#x200B;](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

現時点では、リリースには以下に関するアップデートは含まれていまません。

* シナリオプランナー
* プルーフ
* 目標

## デスクトッププルーフビューアーのアップデート

### バージョン 2.3.0

>[!NOTE]
>
>プレビュー：2026年10月27日（PT）
>すべてのユーザー向けの実稼動リリース：2026年10月28日（PT）

デスクトップ校正ビューアがバージョン 2.3.0に更新されました。 このアップデートには、次の変更が含まれます。

* 複数のバージョンを移動中にスクリーンショットの下のリンクをクリックすると、複数のタブでページが開くインタラクティブプルーフの問題を解決しました。 リンクが1つのタブでページを開くようになりました。

* パフォーマンスとセキュリティを向上させるために、基盤となるフレームワーク（Electron）をChrome バージョン 156で実行される最新バージョンに更新しました。

デスクトップ校正ビューアのダウンロードと更新について詳しくは、[&#x200B; デスクトップ校正ビューアの更新](https://experienceleague.adobe.com/ja/docs/workfront/using/review-and-approve-work/proofing/use-the-desktop-proofing-viewer/update-the-desktop-proofing-viewer)を参照してください。

## お知らせ

### 担当業務リストビューの従来の請求および原価率フィールドの廃止

時間の経過とともに、レート情報を維持するためのより包括的でスケーラブルなアプローチを提供する、強化されたレート管理機能と専用のジョブロール体験が導入されました。 そのため、料金管理は、リストベースの管理ワークフローではなく、専用のエクスペリエンスに移行しています。

2027年1月のリリースでは、従来のフィールド **Billing Per Hour**&#x200B;および&#x200B;**Cost Per Hour**&#x200B;は、Workfront APIまたはフィルター/ビュー/グループ化の設定（ダイレクト参照とテキストモードの計算列の両方）を含むジョブロールリストビューでは使用できなくなります。

レポートの代わりに、推奨されるテキストモードコードを使用できます（必要に応じて`costRates`または`billingRates`を使用してください）。

    &quot;&#39;
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested （costRates）.lists
    type=iterate
    valueexpression=CONCAT （{startDate},&quot; - &quot;,{endDate},&quot;: &quot;,{value}） 
    valueformat=HTML
    &quot;&#39;

担当業務率を管理およびレビューするには、専用の率管理エクスペリエンスを使用します。

* 担当業務/料金ページから担当業務の料金に直接アクセスして管理できます。
* レートレポートを使用して、役職をまたいでレート情報をレビュー、分析、レポートします。

変更に備えるためのアクションは必要ありません。 ただし、ジョブロールのリストビューに現在&#x200B;**時間当たりの請求**&#x200B;および&#x200B;**時間当たりのコスト** フィールドを表示している管理者は、上記の推奨レート管理エクスペリエンスを使用するようにワークフローを更新する必要があります。

担当業務率について詳しくは、[担当業務の作成と管理](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja).

-->

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。 詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)の「新機能」の節を参照してください。
