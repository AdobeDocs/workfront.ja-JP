---
title: 2025年第 4 四半期リリースの概要
description: このページでは、2025年第 4 四半期リリースに含まれる機能について説明します。これらの機能強化は、その四半期を通じて実稼動動環境で利用できるようになる予定です。
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
source-git-commit: 9be63f4242db71b2e08ae528f39d639f8f59c75c
workflow-type: tm+mt
source-wordcount: '1949'
ht-degree: 17%

---

# 2025年第 4 四半期リリースの概要

このページでは、2025 年 10 月に予定されている 2025 年第 4 四半期リリースに含まれる機能について説明します。

このページの機能強化は、プレビュー環境で利用できます。 このページは、2025 年第 4 四半期のリリースが、予定されている実稼動リリースに近づくにつれて、追加の機能強化を加えて更新されます。


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>月次リリースと四半期リリースは、特に指定がない限り、毎月第 2 週の木曜日に公開される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>25.8 （2025 年 8 月 14 日（Pt））</li><li>25.9 （2025 年 9 月 11 日）</li><li>25.10 （2025 年 10 月 16 日（PT））</li></ul> | <ul><li>25.10 （2025 年 10 月 16 日（PT））</li></ul> |
>
>各四半期の最終リリース（今四半期 25.10）では、迅速リリーススケジュールのユーザーに対して、1 日早いリリース（2025 年 10 月 15 日（PT））が届きます。
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [ダッシュボードの機能強化](#dashboards)
* [ドキュメントとプルーフの機能強化](#document-and-proofing-enhancements)
* [ホームの機能強化](#home-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [リクエストの機能強化](#requests-enhancements)
* [その他の機能強化](#other-enhancements)

### 管理者機能の強化

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> 組織の AI Beta機能を有効にする </a><p></p>
            <p>今後の AI 機能を確認して影響を与えやすくするために、組織でこれらの機能のベータ版を有効にできるようにしました。 システム環境設定から、現在使用可能な 1 つ以上の AI Beta機能を有効にできるようになりました。</p>
        </td>
        <td>2025年8月28日（PT）</td>
        <td>2025年9月11日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr>     
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Workfront ユーザープロファイルの更新 </a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Workfront ユーザープロファイルのルックアンドフィールを、Workfrontの他の領域と一致する最新のデザインに更新しました。 これらの更新は、管理者が 1 つのプロファイルを編集する場合、複数のプロファイルを一括編集する場合、またはユーザーが自分のプロファイルを編集する場合の両方に適用されます。</p>
            <p>現在のユーザープロファイルとは、次のような小さな機能上の違いがあります。</p>
            <ul>
                <li>一部のチェックボックス（ユーザーをアクティブとしてマークするなど）は、切り替えまたはボタンに変更されています。</li>
                <li>環境設定の「自分に割り当てた作業を自分の「作業割り当て」タブに送信」オプションが、非推奨（廃止予定）の機能を参照するので削除されました。</li>
            </ul>
        </td>
        <td>2025年8月28日（PT）</td>
        <td>2025年9月4日（PT）</td>
        <td>2025年9月4日（PT）</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> 複数の値オプションを外部 API からカスタムフォームに追加する </a><p></p>
            <p>新しいフィールドタイプ「複数選択外部検索」がカスタムフォームデザイナーで使用できるようになりました。 外部システムにデータを保存している場合、このフィールドタイプを使用すると、外部 API からオプションを読み込み、カスタムフォーム内の他のフィールド値に基づいてフィルタリングできます。 これは、単一選択の外部検索と同じです。</p>
            <p>フォームがオブジェクトに追加されると、API から返された値がドロップダウンフィールドに表示され、ユーザーは複数の値を選択できます。</p>
        </td>
        <td>2025年7月31日（PT）</td>
        <td>2025年8月14日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr>     
  </tbody>
</table>

### ダッシュボードの機能強化

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-dashboards.md" class="MCXref xref" xrefformat="{para}"> 新しいキャンバスダッシュボードのオープンベータ版 </a>
            <p>新しいキャンバスダッシュボード機能を使用すると、キャンバスにレポートタイプを追加することで、Adobe Workfront データを簡単に視覚化できます。このレポートタイプは、サイズ変更、ドラッグ&amp;ドロップなど、多くの柔軟なレイアウトオプションを提供します。</p>
        </td>
        <td>2025年8月26日（PT）</td>
        <td>2025年8月26日（PT）</td>
        <td>2025年8月26日（PT）</td>
    </tr> 
</table>

### ドキュメントとプルーフの機能強化

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}"> 統合承認の段階的なロールアウト </a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>以前は新規ドキュメント承認と呼ばれていた統合承認を、段階的にロールアウトして有効にしています。 この機能は、今後 6 か月間にWorkfront インスタンスで自動的に有効になります。</p>
            <p>統合された承認は、従来のドキュメント承認に代わり、新しい機能を提供します。 
</p>
        </td>
        <td>2025 年 7 月 17 日（PT）より開始される段階的なロールアウト</td>
        <td>2025 年 7 月 17 日（PT）より開始される段階的なロールアウト</td>
        <td>2025 年 7 月 17 日（PT）より開始される段階的なロールアウト</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}"> 新しいWorkfront AI レビュアー </a><p></p>
            <p>メモ：この機能は現在ベータ版です。</p>
            <p>新しいWorkfront AI レビュアーは、画像ガイドラインから始めて、ブランドガイドラインに照らしてコンテンツを自動的にレビューすることで、画像ブランドのコンプライアンスを確保するのに役立ちます。 承認プロセスを合理化するためのスコアと実用的なフィードバックが提供されます。 </p>
            <p>AI レビュー担当者を承認テンプレートまたは個々のレビューおよび承認リクエストに追加できるので、ブランド標準を維持しながら、コンテンツをより迅速に制作できます。</p>
        </td>
        <td>2025年8月14日（PT）</td>
        <td>2025年8月14日（PT）</td>
        <td>2025年8月14日（PT）</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Adobe Expressの新しいプルーフ統合 </a><p></p>
            <p>Adobe ExpressとWorkfront Proofの新しい統合についてお知らせします。</p>
            <ul>
            <li>クリエイティブチーム、法務チーム、コンプライアンスチーム間の共同作業を効率化し、管理を維持しながら公開までの時間を短縮します</li>
            <li>描画マークアップ、注釈、Workfront プルーフビューアを使用したコメントを使用して、詳細なレビューを行います</li>
            <li>電子署名と完全な監査ログにより、企業のコンプライアンス基準に対応</li>
            <li>Express ブランド・テンプレートからの再混在ファイルに対する承認が必要</li>
            <li>高度なプルーフテンプレートを使用した、複数ステージのレビューと承認のワークフローへの高速テンプレートのマッピング</li>
            </ul>
        </td>
        <td>2025年7月28日（PT）</td>
        <td>2025年7月28日（PT）</td>
        <td>2025年7月28日（PT）</td>
    </tr>     
  </tbody>
</table>

### ホームの機能強化

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}"> ホームのマイリクエストウィジェットのアップデート </a><p></p>
            <p>WorkfrontとWorkfront Planning の間でよりシームレスなエクスペリエンスを作り出すために、ホームのマイリクエスト ウィジェットのデザインを一新しました。 新しいウィジェットの特徴は次のとおりです。
            <ul>
                <li>リクエスト情報のレイアウトと編成の改善</li>
                <li>強化されたフィルタリングおよび並べ替えオプション</li>
                <li>Workfront Planning との統合による資源配分の可視化</li>
            </ul>
            </p>
        </td>
        <td>2025年8月21日（PT）</td>
        <td>2025年9月11日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr>     
  </tbody>
</table>

### プロジェクトの強化

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>機能</strong>
        </td>
        <td><strong>プレビュー</strong></td>
        <td><strong>迅速リリース</strong></td>
        <td><strong>四半期ごと</strong></td>
    </tr>
      <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Create project intake forms in Workfront</a>
            <p>To make it easier to create requested projects without converting from issues, we've created Project intake forms. You can configure these intake forms with specific fields, templates, and custom forms, and set approvers for project creation. Then, when a user uses this form, the project is configured to your specifications and sent for approval.</p>
        </td>
        <td>August 21, 2025</td>
        <td>September 11, 2025</td>
        <td>October 16, 2025</td>
    </tr> -->
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Planning の式フィールドおよびWorkfrontの計算カスタム・フィールドに追加された新しい式 </a><p><p>[!BADGE Off schedule]{type=Neutral}</p></p>
            <p>Workfront Planning の式フィールドとWorkfrontの計算カスタムフィールドに、次のように使用する新しい式を追加しました。</p>
            <ul>
            <li>REMOVEACCENTS （string）：入力文字列内のすべてのアクセント記号付き文字から発音区別符号を削除します。</li>
            <li>REPLACEPATTERN （string, pattern, replacement string）：指定したパターンの一致を置換文字列で置き換えます。</li>
            <li>PASCAL （string）：各単語の最初の文字を大文字にし、すべてのスペースを削除して、入力文字列を PascalCase に変換します。</li>
            </ul>
        </td>
        <td>2025年8月7日（PT）</td>
        <td>2025年8月7日（PT）</td>
        <td>2025年8月7日（PT）</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}"> リストから高度な割り当てにアクセスする追加の方法 </a><p></p>
            <p>リストの割り当てに <b> 詳細 </b> ボタンが使用できるようになり、「詳細な割り当て」ページにアクセスできるようになりました。 「詳細な割り当て」に移動するための <b> 人物 </b> アイコンは、リストの割り当てでも使用できます。</p>
        </td>
        <td>2025年8月7日（PT）</td>
        <td>2025年9月11日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr> 
  </tbody>
  </table>

### リソース管理の強化

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}"> ワークロードバランサーをユーザープロファイルで使用できるようになりました </a><p></p>
            <p>すべてのユーザーが、アクセスレベルに関係なく、自分のプロファイルからワークロードバランサーで自分の需要と容量のデータを表示できるようになりました。 Workfront ユーザープロファイルにアクセスすると、ワークロードバランサーが左側のナビゲーションパネルに表示されます。</p>
            <p>ユーザーのワークロードバランサーデータは読み取り専用です。 作業の割り当て、作業の割り当て解除、割り当ての調整をユーザーレベルで行うことはできません。</p>
        </td>
        <td>2025年7月31日（PT）</td>
        <td>2025年8月14日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}"> 役割の割り当ては、ワークロードバランサーに表示されます </a><p></p>
            <p>リソース管理者は、ワークロードバランサーで担当業務の割り当てを確認できるようになりました。 割り当ては、役割が割り当てられているタスクまたはイシューの下の「未割り当ての作業」エリアに表示されます。 ユーザーに割り当てられた作業項目のみが、割り当てられた作業エリアに表示されます。 </p>
            <p>新しいワークロードバランサー設定である「役割の割り当てを表示」で、役割の割り当てを表示するかどうかを決定します。 この設定は、デフォルトで有効になっています。</p>
        </td>
        <td>2025年7月31日（PT）</td>
        <td>2025年8月14日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr>     
  </tbody>
</table>

### リクエストの機能強化

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}"> 統合リクエストリストの新しい結合ステータス列 </a><p></p>
            <p>統一されたリクエストエクスペリエンスを簡素化するために、ステータス列にリクエストステータスと承認ステータスの両方（特定のリクエストに適用される方）が表示されるようになりました。</p>
        </td>
        <td>2025年8月28日（PT）</td>
        <td>2025年9月11日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr>     
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}"> 依頼内容の更新 </a><p></p>
            <p>WorkfrontとWorkfront Planning でリクエストを行う際のユーザーエクスペリエンスを向上させるために、リクエスト時のエクスペリエンスを更新しました。 次の操作が可能になりました。
            <ul>
                <li>WorkfrontおよびWorkfrontの計画リクエストを 1 つのリストに表示します。</li>
                <li>指定した条件に基づいて送信されたリクエストをフィルタリングします。</li>
                <li>統合されたエクスペリエンスで、Workfront リクエストキューとWorkfront Planning フォームを検索して選択します。</li>
                <li>送信済みリクエストリストの列の非表示と並べ替え</li>
            </ul>
            </p>
        </td>
        <td>2025年8月21日（PT）</td>
        <td>2025年9月11日（PT）</td>
        <td>2025年10月16日（PT）</td>
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
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-other.md" class="MCXref xref" xrefformat="{para}"> 拡張リストの更新 </a><p></p>
            <p>高度なリストのレイアウトを使用すると、フィルターとグループ化を使用して作業を表示し、より適切に整理することができます。 ウィジェットの上に表示される青いドットインジケーターで、次の領域でフィルターまたはグループ化がリストに適用されたことを知らせるようになりました。</p>
            <ul>
                <li>自分の要求ウィジェット</li>
                <li>優先度</li>
            </ul>
        </td>
        <td>2025年8月28日（PT）</td>
        <td>2025年9月11日（PT）</td>
        <td>2025年10月16日（PT）</td>
    </tr>     
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2025 年第 4 四半期のリリース期間中のルックアンドフィールの更新 </a></p>
                        <p>Adobe Workfront アプリケーションの様々な領域のルックアンドフィールに対するマイナーアップデートが、2025 年第 4 四半期のリリース期間内に行われています。 </p>
                    </td>
                    <td><p>2025 年第 4 四半期のリリース期間中<br /></p>
                    <td colspan="2"><p>高速リリース：プレビューへのリリース後 1 週間以上（特に指定しない限り）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## インターフェイスの最新化

ユーザーエクスペリエンスを向上させ、他のAdobe Workfront アプリケーションと統合できるよう、Adobe全体でインターフェイスをアップデートしています。 これらの変更は、標準のリリーススケジュールの範囲外でリリースされます。 これらの変更点のリストについては、[ インターフェイスの最新化 ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md) を参照してください。

## その他の領域のリリースノート

### Workfront Fusion の機能強化

Workfront Fusion の新機能は、標準のリリーススケジュール以外の頻度で実稼動環境で使用できます。 最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)を参照してください。

### Workfront計画の機能強化

Workfront Planning の新機能を実稼動環境で使用できます。 最新機能について詳しくは、[Adobe Workfront Planning の 2025 年第 4 四半期リリースアクティビティ ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md) を参照してください。

このリリースの現時点では、次の更新はありません。

* シナリオプランナー
* プルーフ
* Goals

## デスクトッププルーフビューアのアップデート

### バージョン 2.1.52

**すべてのお客様向けの実稼動リリース：2025 年 7 月 31 日**

デスクトッププルーフビューアがバージョン 2.1.52 に更新され、バグ修正が取り組まれました。

2.1.51 の更新には、内部ツールの更新が含まれていましたが、エンドユーザーの機能には影響しませんでした。

このアップデートは、Macと Windows の両方に対応しています。

## お知らせ

### Microsoft Teams用Workfrontの新しいバージョン

[Microsoftが新しい Teams クライアント ](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) に移行すると、Classic Teams クライアントは 2025 年 7 月 1 日（PT）以降は使用できなくなります。 Microsoft TeamsとWorkfrontなどの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。

更新されたWorkfront統合が利用できるようになり、新しい Teams エクスペリエンスと完全に互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfrontが自動的に表示されます。 そうでない場合は、Microsoft Teams App Storeから手動で統合をインストールできます。 新しい Teams クライアントでWorkfront統合をインストールまたは検証するには、[Microsoft Teams用のインストール  [!DNL Adobe Workfront] ](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) を参照してください。

### Workfront for Microsoft Outlook

[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。

* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**

この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**

### その他のWorkfront統合の移行

より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、次の統合は **2026 年 2 月 28 日** 以降は利用できなくなります。

* Workfront for G Suite
* Workfront for Jira
* SalesforceのWorkfront。

Google Workspaceを使用した組織の統合のニーズに対しては、Workfront Automation and Integration を使用することをお勧めします。
Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。

### API バージョン 20

Workfront API バージョン 20 は、2025 年 5 月 4 日（PT）にリリースされました。 API バージョン 20 では、いくつかのリソースとエンドポイントが変更されました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

新機能と更新内容については、[API バージョン 20 の新機能](/help/quicksilver/wf-api/api/new-api-version-19.md)を参照してください。

API バージョンの詳細については、[API のバージョン管理とサポートスケジュール](/help/quicksilver/wf-api/api/api-version-support-schedule.md)を参照してください。

### Workfront のメンテナンスアップデート

2025年 第 1 四半期リリースで行われたメンテナンス更新については、[Workfront のメンテナンス更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja)を参照してください。

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)の「新機能」の節を参照してください。
