---
title: 2024年第 3 四半期リリースの概要
description: このページでは、2024年第 3 四半期リリースに含まれている機能について説明します。これらの機能強化は、四半期を通じて本番環境で利用できるようになる予定です。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 45%

---

# 2024年第 3 四半期リリースの概要

このページでは、2024年第 3 四半期リリースに含まれている機能について説明します。これらの機能強化は、四半期を通じて本番環境で利用できるようになる予定です。

ライブ 24.7 リリースウェビナーはキャンセルされましたが、24.7機能のデモ動画は[こちらから見ることができます](https://video.tv.adobe.com/v/3430532/%20)。

<span class="preview">オフサイクル機能（2024年第 3 四半期のリリース日より前に実稼動にリリースされるもの）は、黄色でハイライト表示されています。</span>

>[!IMPORTANT]
>
>23.3 リリースには、組織を毎月のリリースに移行するオプションが含まれていました。そのため、Workfront では、月次および四半期次のリリース追跡の両方に対応するように、リリースのナンバリング方式を変更しています。最初の数字は年、2 番目の数字はリリースの月を表します。例：2024年4月のリリースは 24.4 となります。
>
>月次リリースと四半期リリースは、特に指定がない限り、毎月第 2 週の木曜日に公開される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>24.5 （2024年5月16日（PT））</li><li>24.6 （2024年6月13日（PT））</li><li>24.7 （2024年7月18日（PT））</li></ul> | <ul><li>24.7 （2024年7月18日（PT））</li></ul> |
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [財務管理の強化](#financial-management-enhancements)
* [統合の機能強化](#integration-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [プルーフ機能の強化](#proofing-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> ビジネスルールが利用可能になりました</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>管理者は、Workfrontの「設定」エリアにビジネスルールを追加できるようになりました。</p>
                        <p>ビジネスルールを使用すると、Workfront オブジェクトに検証を適用し、特定の条件が満たされた場合にオブジェクトを作成、編集または削除できないようにすることができます。 ルールは、カスタムフォームの計算フィールドと同様の数式を使用して作成されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年7月4日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                        </ul>
                        <p><i>新しいUltimate プランの組織でのみ使用できます。</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> カスタムフォームデザイナーは、一般にAdobe Workfrontで利用できます</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>24.7 リリースでは、フォームデザイナーが一般公開され、Adobe Workfrontでカスタムフォームを作成および編集するためのデフォルトのエクスペリエンスになります。 新しいカスタムフォームを作成するか、既存のフォームを開くと、フォームデザイナーのカンバススタイルのワークスペースが表示されます。</p>
                        <p>このリリース以降、従来のフォームビルダーに戻すオプションは提供されなくなります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月19日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">環境プロモーションを使用してWorkfront環境間でオブジェクトを移動</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>環境プロモーションを使用すると、サンドボックス環境から実稼動環境など、あるWorkfront環境から別の環境にオブジェクトを移動できます。 組織のデータやレコードにリスクを与えることなく、オブジェクトを設定してテストすることができます。 その後、再設定しなくても、これらのオブジェクトを実稼動環境に移動できるため、時間と労力を節約できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.6 リリース（2024年6月13日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> カスタムフォームデザイナーでカスタムフォームとカスタムフィールドを共有する</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>新しいフォームデザイナーで、カスタムフォームとカスタムフィールドの両方を共有できるようになりました。 これにより、カスタムフォームを使用したユーザー間のコラボレーションが促進されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">すべてのユーザー向けの実稼動リリース：6月13日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> フィールド領域から新しいカスタムフィールドを追加</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>カスタムフォームを開いてフィールドを作成することなく、Workfrontのフィールド領域から新しいカスタムフィールドまたはウィジェットを直接追加できるようになりました。 これにより、再利用可能なカスタムフィールドをすばやく作成できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> フォームデザイナーで使用可能な複数選択ドロップダウンフィールドタイプ </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>ドロップダウンフィールドをより簡単に定義できるように、カスタムフォームデザイナーに「複数選択」ドロップダウンフィールドを追加しました。 このフィールドタイプを使用すると、ユーザーはドロップダウンリストから複数のオプションを選択できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月4日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2024年6月4日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 財務管理の強化

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}"> プロジェクトとタスクで使用できる請求可能な経費フィールドと請求不可の経費フィールド </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>費用タイプをより簡単に表示できるように、プロジェクトとタスクの費用は請求可能な費用と請求不可の費用に分けられました。 ビューやレポートに追加できるフィールドは次のとおりです。</p>
                        <ul>
                            <li><p>予定請求可能費用コスト</p></li>
                            <li><p>予定非請求費用コスト</p></li>
                            <li><p>実際の請求不可の費用コスト</p></li>
                            <li><p>実際の請求不可の費用コスト</p></li>
                        </ul>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年5月10日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2024年5月10日（PT）</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Experience Manager AssetsおよびAssets Essentials向けWorkfrontの機能強化</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Workfront for Experience Manager AssetsとAssets Essentialsの統合に関して、次の改善が行われました。</p>
                        <ul>
                            <li><p>統合で、クラウドサービスプロバイダーとしてのGCPがサポートされるようになりました。 以前は、AWSとAzureがサポートされていました。</p></li>
                            <li><p>統合を通じてExperience Managerに送信されるファイルのサイズ制限が30 GBに増加しました。 以前は、制限は5 GBでした。</p></li>
                        </ul>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月27日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動：24.7 リリース（2024年7月18日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> ヘッダーまたは詳細セクションからタスクを編集し、コミット日と条件を発行</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>タスクとイシューを簡単に更新できるように、レイアウトテンプレートのタスクとイシューのヘッダーおよび詳細セクションに追加するオプションとして、「コミット日と条件」フィールドを追加しました。 ユーザーは、変更されたレイアウトテンプレートに割り当てられたときに、ページのヘッダーまたは詳細セクションからこれらのフィールドを更新できるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年5月30日（PT）</p>
                            </li>
                            <li>
                                <p>高速リリースの実稼動：24.6 リリース（2024年6月13日（PT））</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">より関連性の高い割り当てを、新規タスクワークフローに追加</a></p>
                        [!BADGE In production for Fast Release &#x200B;]{type=Positive}
                        <p>プロジェクトやプロジェクトのタスクリストにタスクを追加する際に、関連性の高いスマート割り当てを行うための同じ機能が、「新規タスク」ボックスの「割り当て」フィールドに追加されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月13日</p>
                            </li>
                            <li>
                                <p>高速リリースの実稼動：24.5 リリース（2024年5月16日（PT））</p>
                            </li>
                        </ul>
                    <p><i>この機能は、プレビューおよび高速リリースの実稼動から削除されました。</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">関連性の高いスマート割り当て</a></p>
                        [!BADGE In production for Fast Release &#x200B;]{type=Positive}
                        <p>Workfront がタスクのスマート割り当ての計算と提案に使用するアルゴリズムを変更しました。新しいアルゴリズムは、タスクを割り当てる Workfront のエリア（タスクリスト、タスクヘッダーの割り当てエリア、ホーム、概要パネル）に適用されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年12月21日（PT）</p>
                            </li>
                            <li>
                                <p>高速リリースの実稼動：24.5 リリース（2024年5月16日（PT））</p>
                            </li>
                        </ul>
                    <p><i>この機能は、プレビューおよび高速リリースの実稼動から削除されました。</i></p>
                    </td>
                 </tr>
           </tbody>
        </table>

### プルーフ機能の強化

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}"> デスクトップ校正ビューアのセキュリティ更新プログラム </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Workfront Proof Desktop Proofing Viewer 2.1.35 セキュリティ更新プログラムには、以前のリリースで特定された脆弱性に対するセキュリティ バグ修正が含まれています。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年7月4日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版（すべてのお客様向け）：2024年7月4日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### リソース管理の強化

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">休暇がワークロードバランサーに反映されました</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>タスクのプライマリ担当者が休暇をスケジュールしている場合に作業をシームレスに調整するために、ワークロードバランサーは、プロジェクトタイムラインの再計算時に、プライマリユーザーとセカンダリユーザーの両方に時間を再割り当てするようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.7 リリース（2024年7月18日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">製品内ガイドへのバックエンド変更</a></p>
                        <p>今後数週間、製品内ガイドのテクノロジーを変更する予定です。 今回の移行による影響を最小限に抑えようと試みましたが、一部のユーザーは以前に見たガイドに遭遇する可能性があります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>すべての顧客の生産：2024年8月中旬まで増分</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience がより多くの Workfront 組織で利用可能に</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Adobe Unified Experienceのメリットを企業が利用できるようにするため、Workfrontの既存のお客様が利用できるようにしました。 </p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月20日（PT）</p>
                            </li>
                            <li>
                                <p>特定のお客様向けの実稼動：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Adobe Unified Shellは段階的なロールアウトで利用できます。 その他の組織は、24.10および25.1 リリースでAdobe Unified Shellにオンボーディングされます。 </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> ヘルプボタンがメインナビゲーションバーから削除されました</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>統合シェルを使用していないユーザーのエクスペリエンスを統合するために、メインナビゲーションバーの「ヘルプ」ボタンが削除されました。 このボタンは、Unified Shell上のユーザーには存在せず、Workfrontのドキュメントにリンクされており、メインメニューのすべてのユーザーが使用できる同様のヘルプボタンが冗長でした。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのユーザー向けの実稼動リリース：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> オブジェクトへのアクセスが制限されているユーザーのUI エクスペリエンスを改善</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>ユーザーがオブジェクトにアクセスできない場合、Workfrontにオブジェクト名が表示される場所に「アクセス不可」が表示されます。 この改善されたエクスペリエンスは、Workfront APIにも適用されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年3月27日（PT）</p>
                            </li>
                            <li>
                                <p>高速リリースの実稼動：24.5 リリース（2024年5月16日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの実稼動：24.7 リリース（2024年7月18日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2024年第 3 四半期の期間におけるルックアンドフィールのアップデート</a></p>
                        <p>Adobe Workfront アプリケーションの様々なエリアのルックアンドフィールに対する小規模なアップデートが、2024年第 3 四半期の期間内に行われます。特定のリリース日については、個々のリリースノートを確認してください。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年第 3 四半期のリリース期間中</p>
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

Workfront Fusion の新機能は、2024年第 3 四半期のリリーススケジュールから外れた頻度で、実稼動において利用可能になります。最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)を参照してください。

### Workfront シナリオプランナーの機能強化

リリースの現時点では、シナリオプランナーの更新はありません。このエリアは、アップデートが利用可能になると更新されます。

### Workfront Proof の機能強化

リリースの現時点では、Workfront Proof の更新はありません。このエリアは、アップデートが利用可能になると更新されます。

### Workfront Goals の強化

リリースの現時点では、Workfront Goals の更新はありません。このエリアは、アップデートが利用可能になると更新されます。

### API バージョン 18

API バージョン 18 では、いくつかのリソースとエンドポイントが変更されました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

新機能と更新内容については、[API バージョン 18 の新機能](/help/quicksilver/wf-api/api/new-api-version-18.md)を参照してください。

API バージョンの詳細については、[API のバージョン管理とサポートスケジュール](/help/quicksilver/wf-api/api/api-version-support-schedule.md)を参照してください。

### Workfront のメンテナンス更新

2024年第 3 四半期リリースで行われたメンテナンス更新については、[Workfront のメンテナンスアップデート](https://experienceleague.adobe.com/ja/docs/workfront-known-issues/releases/current-updates)を参照してください。

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/home)の「新機能」の節を参照してください。
