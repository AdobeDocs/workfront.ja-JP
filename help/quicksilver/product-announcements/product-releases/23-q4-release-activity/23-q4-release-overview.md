---
title: 2023年第 4 四半期リリースの概要
description: 2023年第 4 四半期リリースの概要
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '2773'
ht-degree: 99%

---

# 2023年第 4 四半期リリースの概要

このページでは、2023年第 4 四半期リリースに含まれる機能について説明します。これらの機能強化は、2023年10月26日（PT）および 2023年10月27日（PT）の 23.10 リリースで、すべてのお客様が本番環境で利用できるようになる予定です。

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

23.10 リリースウェビナーは 2023年10月5日（PT）に開催されました。[こちら](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes)でウェビナーに登録してオンデマンド録画を視聴できます。

<span class="preview">オフサイクル機能（2023年第 4 四半期のリリース日より前に実稼動環境にリリースされる機能）は、黄色でハイライト表示されます。</span>

>[!IMPORTANT]
>
>23.3 リリースには、組織を毎月のリリースに移行するオプションが含まれていました。そのため、Workfront では、月次および四半期次のリリース追跡の両方に対応するように、リリースの採番方式を変更しています。
>
>* **迅速リリース（毎月）**&#x200B;トラックを使用している場合、23.3 以降のリリースは、2023年8月31日（PT）の **23.8** です。
>* **四半期**&#x200B;リリーストラックを使用している場合、23.3 以降のリリースは、2023年10月26日（PT）の週の **23.10** です。
> 
> 四半期リリースには、3 つの月別リリースの機能が含まれます。例えば、23.10 の四半期リリースには、23.8、23.9、および 23.10 の月別リリースでリリースされた機能が含まれます。
>
>毎月および四半期のリリースは、月の最終木曜日に提供される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>23.8（2023年8月31日（PT））</li><li>23.9（2023年9月28日（PT））</li><li>23.10（2023年10月26日（PT））</li></ul> | <ul><li>23.10（2023年10月26日（PT）の週）</li></ul> |
>| <ul><li>リリースなし（2023年11月）</li><li>リリースなし（2023年12月）</li><li>24.1（2024年1月）</li></ul> | <ul><li>24.1（2024年1月）</li></ul> |
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [ボードの機能強化](#boards-enhancements)
* [財務管理の機能強化](#financial-management-enhancements)
* [ホームの機能強化](#home-enhancements)
* [統合の機能強化](#integration-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [その他の機能強化](#other-enhancements)

### 管理者機能の強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">従来のライセンスモデルのお客様への利用可能なプルーフとドキュメントの決定</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しい Adobe Workfront ライセンスモデルにまだ移行していない従来のお客様は、月ごとのユーザーあたりのプルーフとドキュメントに関する決定数を含むデータを、単一のレポートで表示できるようになりました。このデータは、ユーザーの決定レポートを実行する際に使用できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2023年10月12日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>            
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームの計算フィールドで、$$USER ワイルドカードを使用できるようになりました。</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいフォーム designer で、計算カスタムフィールドと外部ルックアップフィールドで $$USER ワイルドカードを使用できるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月5日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">外部 API からカスタムフォームに値オプションを追加</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいフィールドタイプ「<strong>外部ルックアップ</strong>」をカスタムフォーム designer で使用できるようになりました。データを外部システムに保存している場合、このフィールドタイプを使用すると、外部 API からオプションを読み込み、カスタムフォーム内の他のフィールド値に基づいてフィルタリングできます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年9月14日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.9 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### ボードの機能強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront ボードでサブタスクを利用できるようになりました。</a></p><p>[!BADGE In production ]{type=Informative}</p><p>接続されたカードを Workfront タスクのボードに追加すると、既存のサブタスクがカード上に取り込まれます。また、接続されているカードでサブタスクを作成すると、サブタスクが Workfront タスクに追加されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）</p>
                            </li>
                            <li>
                                <p>ボード先行アクセス用の実稼動版：該当なし</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版：該当なし</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">ボードとカードでのユーザー割り当ての機能強化</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Adobe Workfront ボードでユーザーをボードやカードに追加する際の柔軟性を高める機能強化が利用できるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月21日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2023年8月24日（PT）</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">接続されたカード上でのドキュメントの追加</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Adobe Workfront ボードの接続されたカードにドキュメントを添付できるようになりました。カードに追加したドキュメントは、接続されたタスクまたはイシューの「ドキュメント」タブで使用でき、両方の領域で同じファイルタイプがサポートされます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月21日（PT）</p>
                            </li>
                            <li>
                                <p>ボードの早期アクセスの実稼働版：2023年8月24日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版：該当なし</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">ドキュメントが接続カードで表示専用として使用可能</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Adobe Workfront ボードの接続カードで、画像や PDF などのドキュメントを表示できるようになりました。ドキュメントは、ブラウザーでプレビューするか、コンピューターにダウンロードすることができます。 </p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月3日（PT）</p>
                            </li>
                            <li>
                                <p>ボードの早期アクセスの実稼働版：2023年8月10日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版：該当なし</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">プロジェクトのボードビューをイシューで使用可能</a></p><p>[!BADGE In production ]{type=Informative}</p><p>プロジェクトのイシューリストのボードビューにアクセスできるようになりました。かんばんボードを使用すると、イシューの進行状況を、リストで表示するよりも視覚的に追跡できます。 </p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月3日（PT）</p>
                            </li>
                            <li>
                                <p>ボード先行アクセス用の実稼動版：該当なし</p>
                            </li>
                             <li>
                                <p>迅速リリース用の実稼動版：該当なし</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>    
           </tbody>
        </table>

### 財務管理の機能強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">日付上有効なコストと請求レート</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>有効日のコスト率と請求率が、Workfront の会社、ユーザー、および担当業務のオブジェクトで使用できるようになりました。プロジェクトに有効日のレートが適用され、時間がプロジェクトタスクにログオンすると、コストと売上高は各期間の指定されたレートを使用して計算されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年6月29日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### ホームの機能強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">プロジェクトウィジェット、タスクウィジェットおよびイシューウィジェットの作業委任ボタン</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>従来のホームページで要求が多かった機能であり、マイワーク、マイタスク、マイイシューの各ウィジェットに委任ボタンを追加しました。これにより、不在時に作業を簡単に委任できるようになりました。ボタンを表示するには、Workfront 環境で作業の委任を有効にする必要があります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホーム用の新しいボードウィジェット</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいホームで利用可能な作業管理オプションに新しく加わった大きな機能として、ホームページにボードを表示できるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいコントリビューターのデフォルトのランディングページ：新しいホーム</a>  </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいホームが、コントリビューターや依頼者のアカウントのデフォルトのランディングページになりました。このデフォルトの新しいホームページには、コントリビューターがすぐに作業を管理できるように、特に選択された多数のウィジェットが含まれています。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホームでの作業追跡の変更</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>ユーザーからのフィードバックに基づいて、タスクの期限と完了を集計したページ全体の時間範囲フィルターと概要バーを削除しました。プロジェクト、タスクおよびイシューの各ウィジェットには、個々の範囲をカスタマイズできる、ビルトインのフィルタリング機能が備わっています。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年9月13日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.9 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">自分の作業ウィジェット用の新しいクイックアクションボタン</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいホームから直接作業を管理する機能がさらに拡張され、新しいクイックアクションボタンが自分の作業ウィジェットに追加されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年9月13日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.9 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホーム用の新しいフィルターオプション</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいホームの自分の作業ウィジェットで新しいフィルターオプションを利用できるようになりました。オプションには、オブジェクトタイプ（タスク、イシュー、リクエスト）とステータス（準備未完了、開始準備完了、作業中、完了）のフィルターが含まれます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月17日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.8 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホーム用のカスタム用語のサポート</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>組織独自のニーズをより適切に満たすために、新しいホームでは、インスタンスのレイアウトテンプレートで定義されたオブジェクトに対して、カスタム用語を利用するようになりました。例えば、Workfront インスタンスで「プロジェクト」オブジェクトのラベルが「キャンペーン」に変更されている場合、マイプロジェクトウィジェットは代わりに新しいホームのマイキャンペーンとして表示されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月17日（PT）<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2023年8月31日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホームが無効になっているアカウントに対して削除した「新しいホームを試す」ボタン</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>新しいホームが無効になっているアカウントに対して、「新しいホームを試す」ボタンが表示されなくなりました。個々のユーザーが「新しいホームを試す」ボタンを使用できるようにするには、事前にシステム管理者が新しいホームを再度有効にする必要があります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月17日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.8 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホームのデフォルトのウィジェットセットへの変更</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>タスクの作成権限を必要とする To-Do ウィジェットは、標準、プランまたはワークのライセンスタイプを持つユーザー向けのデフォルトのウィジェットセットにのみ存在するようになりました。さらに、ウィジェットは、他のすべてのライセンスタイプを持つユーザーのホームページから自動的に削除されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月17日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 2023年8月17日（PT）</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版： 2023年8月17日（PT）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 統合の機能強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">SharePoint（GraphAPI）にドキュメントを送信する際のエクスペリエンスに対する機能強化</a></p><p>[!BADGE In production ]{type=Informative}</p><p>SharePoint（GraphAPI）フォルダーにドキュメントを送信する際にフォルダーを見つけやすくするために、一部の変更を行いました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月24日（PT）<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2023年8月31日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">ドキュメント統合用のドラッグ＆ドロップへのアップグレード</a></p><p>[!BADGE In production ]{type=Informative}</p><p>リンクされたフォルダーにファイルをドラッグ＆ドロップする際の明確さを高め、ユーザーエラーを削除するために、一部の機能強化を行いました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月24日（PT）<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：23.10 リリース以降</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### プロジェクトの強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                 </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">新規ドキュメント承認</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>このリリースでは、新機能に加え、承認の作成と文書の承認やレビューの両方の承認プロセスが合理化されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">この機能は段階的リリースの一部で、現在は特定のお客様のみが利用できます。</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">タスクリストのリアルタイム更新</a> </p>
                        <p>[!BADGE In production]{type=Informative}</p>
                        <p>タスクリストがリアルタイムで更新されるようになりました。タスクに対して行われた変更はタスクリスト内で更新されるので、タスクリストを表示しているユーザーはページを更新せずに変更を確認できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：該当なし<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：段階的なロールアウト、2023年10月19日（PT）完了</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">プロジェクトに新しいイシューを追加する際にアップデートされたデザイン</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>このアップデートは 23.3 リリースで発表されました。</p>
                        <p>新しいイシューをプロジェクトに送信する際に表示される新しいイシューボックスをアップデートしました。現在のインターフェイスは、新しいリクエストをリクエストキューに送信する際に表示される新しいリクエストボックスと同じです。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023 年 7 月 26 日<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.8 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">フォームでの計算フィールドの動的な再計算</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>ページ上のフォームでの依存値を変更すると、オブジェクトに添付されたフォームでの計算フィールドは、リアルタイムで動的に再計算されるようになりました。これにより、フォームを保存せずに更新された結果を確認できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月17日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.8 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">割り当てのないシンプルな期間タイプを使用した子の定期タスクへの予定時間数の設定</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>割り当てのないシンプルな期間タイプを使用して定期タスクに予定時間数を割り当てる方法を変更しました。ここで、割り当てのないシンプルな期間タイプを使用して新規定期タスクに予定時間数を設定すると、その時間数は個々の繰り返しにも割り当てられます。この変更以前では、親タスクの割り当てが解除されている場合、個々の繰り返しの時間数は保存されませんでした。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年8月17日（PT）<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.8 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### その他の機能強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">機能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">リリース日</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">コントリビューターのメインメニューの変更</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>有料 Workfront ライセンスタイプで利用できる機能を、コントリビューターや依頼者によりわかりやすく伝えるために、利用可能なすべてのオプションがメインメニューに表示されるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年10月12日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版： 23.10 リリースに併せて</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリースに併せて</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">新しいコメントエクスペリエンス（ベータ版の機能強化）</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>更新セクションの機能強化は、ベータ版コメントエクスペリエンスがリリースされる 2023年第 4 四半期の期間内に利用可能になります。これらの機能強化は、2023年第 4 四半期リリース（2023年10月）で、すべてのお客様向けに本番環境で利用できるようになります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023 年第 4 四半期のリリース期間中<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版：23.8 リリース以降</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリース（特に指定がない限り）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">新しいキャンバスダッシュボード（ベータ版の機能強化）</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>キャンバスダッシュボードの機能強化は、現在進行中のベータ版の一部として、2023年第 4 四半期にリリースされます。これらの機能強化は、2023年第 4 四半期リリース（2023年10月）で、すべてのお客様向けに本番環境で利用できるようになります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023 年第 4 四半期のリリース期間中<br /></p>
                            </li>
                            <li>
                                <p>迅速リリース用の実稼動版：23.8 リリース以降</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：23.10 リリース（特に指定がない限り）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2023 年第 4 四半期の期間におけるルックアンドフィールの更新</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Adobe Workfront アプリケーションの様々なエリアのルックアンドフィールに対するマイナーアップデートは、2023 年第 4 四半期の期間内に行われます。特定のリリース日については、個々のリリースノートを確認してください。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023 年第 4 四半期のリリース期間中</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版リリース：リリースノートで日付を確認してください。</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

## お知らせ

### Workfront Fusion の機能強化

Workfront Fusion の新機能は、2023 年第 4 四半期のリリーススケジュールから外れたタイミングで、実稼動環境で利用可能になります。最新の機能について詳しくは、[Adobe Workfront Fusion のリリースアクティビティ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)を参照してください。

### Workfront シナリオプランナーの機能強化

リリースの現時点では、シナリオプランナーの更新はありません。このエリアは、アップデートが利用可能になると更新されます。

### Workfront Proof の機能強化

リリースの現時点では、Workfront Proof の更新はありません。このエリアは、アップデートが利用可能になると更新されます。

### Workfront Goals の強化

リリースの現時点では、Workfront Goals の更新はありません。このエリアは、アップデートが利用可能になると更新されます。

### API バージョン 17

API バージョン 17 は 2023年10月12日（PT）にリリースされました。API バージョン 17 では、いくつかのリソースとエンドポイントが変更されました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

新機能と更新内容については、[API バージョン 17 の新機能](/help/quicksilver/wf-api/api/new-api-version-17.md)を参照してください。

API バージョンの詳細については、[API のバージョン管理とサポートスケジュール](/help/quicksilver/wf-api/api/api-version-support-schedule.md)を参照してください。

### Workfront のメンテナンスアップデート

22.3 リリースで行われたメンテナンスアップデートについて詳しくは、[Workfront メンテナンスのアップデート](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates)を参照してください。

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/home)の「新機能」の節を参照してください。

### Workfront から近日中に削除される機能

次の機能は、近日中に Workfront から削除されます。

#### 23.10 での Proof モバイルアプリの廃止

23.10 リリースでは、Proof モバイルアプリが正式に廃止されます。一般的な Workfront モバイルアプリが新しいプルーフ機能で強化されました（詳しくは、Workfront モバイルの機能強化に関するリリースノートを参照してください）。できるだけ早くプルーフ作業にお使いいただくことをお勧めします。

Workfront モバイルアプリには Workfront へのログインが必要です。外部のユーザーおよびゲストは、引き続きプルーフの作業に Proof アプリを使用できます。ただし、サポートは終了し、23.10 では使用できなくなります。

#### ワークストリームを使用していないアカウントにおけるワークストリームの削除

Adobe Workfront ボードでワークストリームを作成したことがないアカウントについては、2023年10月11日（PT）以降、ボードダッシュボードからワークストリームエリアが削除されました。ワークストリームを使用するアカウントは、引き続きワークストリームにアクセスできます。拡張スクラム機能は、今後のリリースで対処される予定です。

<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
