---
title: 2026年第 2 四半期リリースの概要
description: このページでは、2026年第 2 四半期リリースに含まれる機能について説明します。これらの機能強化は、その四半期を通じて本番動環境で利用できるようになる予定です。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 93c22854ccc405c442331ac392d919d63b8a8aa8
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 40%

---

# 2026年第 2 四半期リリースの概要

このページでは、2026年4月に予定されている2026年第2四半期のリリースに含まれる機能について説明します。

このページの機能強化は、プレビュー環境で利用できます。このページは、2026年第2四半期のリリースが予定されている本番リリースに近づくにつれて、さらに強化された内容で更新されます。


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
* [ドキュメントの機能強化](#document-enhancements)
* [プロジェクトの機能強化](#project-enhancements)
* [レポートの機能強化](#reporting-enhancements)
* [機能強化のリクエスト](#requesting-enhancements)
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
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">プロジェクトの基本設定からユーザー設定の四半期が削除されました</a><p>プロジェクト環境設定セクションからカスタム四半期領域を移動しました。 現在は、設定のスタンドアロンセクションになっています。</p>
        </td>
        <td><p>2026年3月5日（PT）</p></td>
        <td><p>2026年4月15日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> デフォルトでカスタムフォームセクションを折りたたむ </a><p>デフォルトでは、カスタムフォーム上のすべてのセクションは、フォーム自体が展開されると展開されます。 カスタムフォームデザイナーの新しいオプションを使用すると、ユーザーがフォームを開いたときに、デフォルトで折りたたむセクションをマークできます。 このオプションは、フィールドではなくセクションレベルで適用されます。</p>
        </td>
        <td><p>2026年2月26日（PT）</p></td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> リッチテキストフィールドタイプがカスタムフォームで使用できるようになりました </a><p>カスタムフォームの新しい<b>リッチテキスト</b>フィールド型は、強力なテキストエディターで、従来の太字、斜体、下線、箇条書き、番号、ハイパーリンク、およびブロック引用符のオプションに加え、上付き文字や下付き文字、見出し、表などの書式設定オプションを備えています。 文字数の制限は 15,000 のままです。</p>
        </td>
        <td><p>2026年1月29日（PT）</p></td>
        <td><p>2026年2月12日（PT）</p>
            <p>この機能は、2026 年 2 月 13 日（PT）に実稼動環境から一時的に削除されました。</p></td>
        <td><p>未定</p></td>
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

### ドキュメントの機能強化

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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">WorkfrontとFrame.ioを利用した統合レビューと承認</a><p></p>
            <p>WorkfrontとFrame.ioを活用したレビューと承認の統合をご紹介します。これにより、効率的なレビューと承認のエクスペリエンスが実現し、計画、プルーフィング、共同作業が1つのコネクテッドワークフローにまとめられます。
 </p>
        </td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月15日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}"> 統合承認で複数ステージの承認ワークフローを使用できる </a><p></p>
            <p>複数ステージの承認ワークフローが統合承認で使用できるようになりました。これにより、組織は、現実世界での作業のレビュー方法を反映した、構造化された繰り返し可能な承認プロセスを適用できます。 </p>
        </td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月15日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}"> 複数ステージ承認ワークフローテンプレートの設定と使用 </a><p></p>
            <p>複数ステージの承認ワークフローテンプレートを設定して再利用できるようになりました。これにより、繰り返し可能な承認ワークフロー全体で一貫したガバナンスを簡単に適用できます。 </p>
        </td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月15日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
             </tbody>
        </table>


### プロジェクトの機能強化

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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">単一または一括割り当てのテンプレートタスク</a>のエクスペリエンスが更新されました<p>[!BADGE Off schedule]{type=Neutral}</p><p> 単一のテンプレートタスクの編集または一括編集を行う場合は、「テンプレートタスクの編集」ボックスの「割り当て」セクションを更新しました。  </p>
        </td>
        <td><p>2026年2月5日（PT）</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}"> タスクを単一または一括割り当てした場合のエクスペリエンス </a> 更新されました<p>[!BADGE Off schedule]{type=Neutral}</p><p> 単一のタスクの編集時または一括編集時に、「タスクを編集」ボックスの「割り当て」セクションを更新しました。 </p>
        </td>
        <td><p>2026年1月26日（PT）</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
        <td><p>2026 年 2 月 5 日より</p></td>
    </tr>
            </tbody>
        </table>

### レポートの機能強化

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
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">データ接続接続の新しい認証オプション</a><p></p>
            <p>RSAキーまたはPAT（プログラム・アクセス・トークン）接続を使用してデータ接続に対する認証を実行できるようになり、従来のユーザー名/パスワード認証情報に代わる、より安全で柔軟な方法が追加されました。 </p>
        </td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}"> レポートの作成時に表示されるカスタムフィールドラベル </a><p></p>
            <p>レポート作成ツールのフィールド名およびオブジェクトの前にカスタムフィールドラベルが表示されるようになり、フィールドを見つけやすくなりました。 フィールドラベルは、リストでフィルター、ビュー、グループ化を定義する際にも表示されます。</p>
        </td>
        <td><p>2026年2月26日（PT）</p></td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}"> 共有可能な報告書フォルダー </a><p></p>
            <p>共有可能なレポートフォルダーを使用して、レポートを整理および共有できるようになりました。 この新機能により、大量のレポートを管理するチームは、拡張性と一貫性のあるアクセス制御を維持できます。</p>
        </td>
        <td><p>2026年2月26日（PT）</p></td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}"> キャンバスダッシュボードでのグラフのグループ化の日付ラベルを改善しました </a><p></p>
            <p>データを日付別にグループ化するグラフで、より明確で読みやすい日付ラベルが表示されるようになりました。 この更新により、日付ラベルは、選択した「グループ化の基準」オプション（日、週、月、年など）に基づいて動的に調整されるようになり、グラフを一目で読みやすく、解釈しやすくなりました。</p><p>注意： Canvasダッシュボードは現在ベータ版です。</p>
        </td>
        <td><p>2026年2月26日（PT）</p></td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
    </tr>
             </tbody>
        </table>

### 機能強化のリクエスト

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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}"> 拡張ビューの更新された共有エクスペリエンス </a><p></p>
            <p>新規リクエスト エリアで、ユーザーと拡張ビューを共有し、ビュー権限を付与すると、ユーザーはビュー要素を変更でき、それらの変更はユーザーの個人環境設定に保存されます。 変更を含むビューのコピーを保存するか、共有ビューを元の設定にリセットするオプションが追加されました。 コピーしたビューを他のユーザーと共有することもできます。 </p>
        </td>
           <td><p>2026年2月26日（PT）</p></td>
        <td><p>2026年3月12日（PT）</p></td>
        <td><p>2026年4月16日（PT）</p></td>
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience がより多くの Workfront 組織で利用可能に</a><p></p>
            <p>組織が Adobe Unified Experience のメリットにアクセスできるように、既存の Workfront のお客様向けに、引き続きサービスを提供します。</p>
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

## その他のエリアに関するリリースノート

### Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境の標準リリーススケジュール以外のサイクルで使用できます。最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)を参照してください。

### Workfront Planning の機能強化

Workfront Planning の新機能は、実稼動環境で使用できます。最新機能について詳しくは、[Adobe Workfront Planning の 2026 年第 2 四半期リリースアクティビティ &#x200B;](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md) を参照してください。

現時点では、リリースには以下に関するアップデートは含まれていまません。

* シナリオプランナー
* プルーフ
* 目標

## デスクトッププルーフビューアーのアップデート

### バージョン 2.1.54

**実稼動版リリース（すべてのお客様向け）：2025年12月11日（PT）**

デスクトッププルーフビューアーが 2.1.52 から 2.1.54 にアップデートされました。このアップデートには、内部ツールのアップデートが含まれていましたが、エンドユーザーの機能には影響しませんでした。

2.1.53 バージョンには、内部ツールの変更も含まれています。

このアップデートは、Mac と Windows の両方に対応しています。

## お知らせ

### Workfront Planning体験版が利用可能になりました

[!BADGE スケジュールから外れる]{type=Neutral}

>[!NOTE]
>
>* すべてのユーザー向けのプレビューと実稼動：2026 年 3 月 2 日（PT）
>* Planning 体験版環境にアクセスするには、お使いの環境で使用可能な体験版契約に同意する必要があります。
>* 試用期間中に Planning Designerを使用する場合、Adobe AI代理店契約書に署名する必要はありません。

Workfront Planning 体験版を、すべてのWorkfront ユーザーが利用できるようになりました。

無料体験版では、Workfrontのお客様に、2026 年 3 月 2 日（PT）以降、Workfront Planning への 60 日間のPrime ライセンスのアクセスが提供されます。 試用期間は 2026 年 5 月 1 日に終了します。

Workfront Planning の無料体験版では、次の機能を利用できます。

* キュレートされた複数ワークスペースの計画環境
* どこから始めればよいかを把握するためのサンプルデータ
* 製品内トレーニングおよびガイダンス
* 特定の役割に合わせて調整された、セットアップ中のマイルストーンを明確に示します。
* Planning Designer – 希望する環境の構築を支援する AI を活用したアシスタント

詳細については、[Adobe Workfront Planningの無料体験版を開始する](/help/quicksilver/planning/general/trial-workfront-planning.md)を参照してください。

### API バージョン 21

Workfront API バージョン 21 は 2025年10月23日（PT）にリリースされました。API バージョン 21 では、いくつかのリソースとエンドポイントが変更されました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

>[!IMPORTANT]
>
>この API バージョンの変更には、既存の API 呼び出しに影響を与える可能性のある重大な変更が含まれています。これは、API バージョン 21 ではイベント登録バージョン 2 が使用されているためです。
>
> 複数選択フィールドの場合、イベントサブスクリプションバージョン2は常に配列として送信します。 バージョン 1 では、複数の値が選択されている場合に、配列が送信されました。1 つの値のみが選択されている場合は、文字列が送信されました。

新機能とアップデートについて詳しくは、[API バージョン 21 の新機能](/help/quicksilver/wf-api/api/new-api-version-21.md)を参照してください。

API バージョンの詳細については、[API のバージョン管理とサポートスケジュール](/help/quicksilver/wf-api/api/api-version-support-schedule.md)を参照してください。

### その他の Workfront 統合の移行

より安定したスケーラブルな統合を実現するために、アドビでは、Workfront の自動処理と統合 （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。この移行プロセスの一環として、次の統合は **2026年2月28日（PT）**&#x200B;以降は利用できなくなります。

* Workfront for G Suite
* Workfront for Jira
* Salesforce 用 Workfront

Google Workspace を使用した組織の統合のニーズに対しては、Workfront の自動処理と統合を使用することをお勧めします。
Workfront の自動処理と統合の概要について詳しくは、[Adobe Workfront Fusion の概要](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。


### Workfront のメンテナンスアップデート

2026年第 2 四半期リリースで行われたメンテナンス更新については、[Workfront のメンテナンスアップデート](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja)を参照してください。

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)の「新機能」の節を参照してください。
