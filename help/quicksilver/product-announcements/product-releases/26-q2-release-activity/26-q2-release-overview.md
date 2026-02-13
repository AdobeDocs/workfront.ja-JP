---
title: 2026年第 2 四半期リリースの概要
description: このページでは、2026年第 2 四半期リリースに含まれる機能について説明します。これらの機能強化は、その四半期を通じて本番動環境で利用できるようになる予定です。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 9160a68653999c35de32dd417b18ea8197ef446f
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 31%

---

# 2026年第 2 四半期リリースの概要

このページでは、2026 年 4 月に予定されている 2026 年第 2 四半期のリリースに含まれる機能について説明します。

このページの機能強化は、プレビュー環境で利用できます。 このページは、2026 年第 2 四半期のリリースが、予定されている実稼動リリースに近づくにつれて、追加の機能強化を加えて更新されます。


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>月次リリースと四半期リリースは、特に指定がない限り、毎月第 2 週の木曜日に公開される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>26.2（2026年2月12日（PT））</li><li>26.3（2026年3月12日（PT））</li><li>26.4 （2026 年 4 月 15 日（Pt））</li></ul> | <ul><li>26.1 （2026 年 4 月 16 日）</li></ul> |
>
>各四半期の最終リリース（今四半期 26.4）では、迅速リリーススケジュールのユーザーに対して、1 日早い（2026 年 4 月 15 日（PT））リリースが届きます。
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [その他の機能強化](#other-enhancements)

### 管理者機能の強化

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>機能</strong>
        </td>
        <td><strong>プレビュー</strong></td>
        <td><strong>迅速リリース</strong></td>
        <td><strong>四半期ごと</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> リッチテキストフィールドタイプがカスタムフォームで使用できるようになりました </a><p>カスタムフォームの新しい <b> リッチテキスト </b> フィールドタイプは堅牢なテキストエディターで、太字、斜体、下線、箇条書き、番号付け、ハイパーリンク、ブロック引用の従来のオプションに加えて、上付き文字、下付き文字、見出し、表などの書式設定オプションが用意されています。 文字数の制限は 15,000 のままです。</p>
        </td>
        <td><p>2026年1月29日（PT）</p></td>
        <td><p>2026年2月12日（PT）</p>
            <p>この機能は、2026 年 2 月 13 日（PT）に実稼動環境から一時的に削除されました。</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Workfrontのメール通知用の新しい IP アドレス </a><p></p>
            <p>Workfrontからメール通知を送信するために使用される IP アドレスを更新しています。 メールまたはファイアウォールの許可リストを維持している場合は、以下の新しい IP アドレスを追加して <b>Workfront通知が引き続き配信されるようにする </b> 必要があります）。</p><p>これらの更新は、承認、リマインダー、プルーフ通知、その他のシステムメッセージなど、Workfront アプリケーションで生成されたすべてのアウトバウンドメールに適用されます。</p>
            <ul>
            <li>米国：
            <ul>
            <li>206.55.149.212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>EU: 
            <ul>
            <li>24.110.76.224</li>
            <li>24.110.76.223</li>
            </ul>
            </li>
            </ul> </p>
        </td>
        <td><p>2026年1月15日（PT）</p></td>
        <td><p>2026年1月15日（PT）</p></td>
        <td><p>2026年1月15日（PT）</p></td>
    <tr>
            </tbody>
        </table>

### プロジェクトの強化

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>機能</strong>
        </td>
        <td><strong>プレビュー</strong></td>
        <td><strong>迅速リリース</strong></td>
        <td><strong>四半期ごと</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}"> および単一または一括割り当てのテンプレートタスクのタイミングとエクスペリエンスが更新されました </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> 単一のテンプレートタスクの編集または一括編集を行う際に、「テンプレートタスクを編集」ボックスの「割り当て」セクションを更新しました。  </p>
        </td>
        <td><p>2026年2月5日（PT）</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}"> タスクを単一または一括割り当てした場合のエクスペリエンス </a> 更新されました<p>[!BADGE Off schedule]{type=Neutral}</p><p> 単一のタスクの編集時または一括編集時に、「タスクを編集」ボックスの「割り当て」セクションを更新しました。 </p>
        </td>
        <td><p>2026年1月26日（PT）</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
    </tr>
            </tbody>
        </table>

### その他の機能強化

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>機能</strong>
        </td>
        <td><strong>プレビュー</strong></td>
        <td><strong>迅速リリース</strong></td>
        <td><strong>四半期ごと</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobeの統合エクスペリエンスを、より多くのWorkfront組織で利用できるようになりました </a><p></p>
            <p>Adobe Unified Experience のメリットに企業がアクセスできるように、アドビでは既存のWorkfrontのお客様が利用できるようにするサービスを引き続き提供します。</p>
        </td>
        <td><p>2025年12月11日（PT）</p></td>
        <td><p>2026年2月11日（PT）</p></td>
        <td><p>2026年2月11日（PT）</p></td>
    </tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## その他の領域のリリースノート

### Workfront Fusion の機能強化

Workfront Fusion の新機能は、標準のリリーススケジュール以外の頻度で実稼動環境で使用できます。 最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)を参照してください。

### Workfront計画の機能強化

Workfront Planning の新機能を実稼動環境で使用できます。 最新機能について詳しくは、[Adobe Workfront Planning の 2026 年第 2 四半期リリースアクティビティ ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md) を参照してください。

このリリースの現時点では、次の更新はありません。

* シナリオプランナー
* プルーフ
* Goals

## デスクトッププルーフビューアのアップデート

### バージョン 2.1.54

**すべてのお客様向けの実稼動リリース：2025 年 12 月 11 日**

デスクトッププルーフビューアが 2.1.52 から 2.1.54 にに更新されました。この更新には、内部ツールの更新が含まれていましたが、エンドユーザーの機能には影響しませんでした。

2.1.53 バージョンには、内部ツールの変更も含まれています。

このアップデートは、Macと Windows の両方に対応しています。

## お知らせ

### API バージョン 21

Workfront API バージョン 21 は、2025 年 10 月 23 日（PT）にリリースされました。 API バージョン 21 では、いくつかのリソースとエンドポイントが変更されました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

>[!IMPORTANT]
>
>この API バージョンの変更は、既存の API 呼び出しに影響を与える可能性のある重大な変更を特徴としています。 これは、API バージョン 21 がイベント購読バージョン 2 を使用しているためです。
>
> 複数選択フィールドの場合、イベント購読バージョン 2 は常に配列として送信します。 バージョン 1 では、複数の値が選択されている場合、配列が送信されました。 1 つの値のみが選択された場合、文字列が送信されます。

新機能と更新内容については、[API バージョン 21 の新機能](/help/quicksilver/wf-api/api/new-api-version-21.md)を参照してください。

API バージョンの詳細については、[API のバージョン管理とサポートスケジュール](/help/quicksilver/wf-api/api/api-version-support-schedule.md)を参照してください。

### その他のWorkfront統合の移行

より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、次の統合は **2026 年 2 月 28 日** 以降は利用できなくなります。

* Workfront for G Suite
* Workfront for Jira
* SalesforceのWorkfront。

Google Workspaceを使用した組織の統合のニーズに対しては、Workfront Automation and Integration を使用することをお勧めします。
Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。


### Workfront のメンテナンス更新

2025年第 2 四半期リリースで行われたメンテナンス更新については、[Workfront のメンテナンスアップデート](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja)を参照してください。

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)の「新機能」の節を参照してください。
