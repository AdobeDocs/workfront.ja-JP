---
title: 2024年第 3 四半期リリースの概要
description: このページでは、2024年第 3 四半期リリースに含まれている機能について説明します。これらの機能強化は、四半期を通じて本番環境で利用できるようになる予定です。
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 44%

---

# 2024年第 3 四半期リリースの概要

このページでは、2024年第 3 四半期リリースに含まれている機能について説明します。これらの機能強化は、四半期を通じて本番環境で利用できるようになる予定です。

ライブ 24.7 リリースウェビナーはキャンセルされましたが、引き続き [ こちらから 24.7 の機能のビデオデモをご覧ください ](https://video.tv.adobe.com/v/3430532/%20)。

<span class="preview">オフサイクル機能（2024年第 3 四半期のリリース日より前に実稼動にリリースされるもの）は、黄色でハイライト表示されています。</span>

>[!IMPORTANT]
>
>23.3 リリースには、組織を毎月のリリースに移行するオプションが含まれていました。そのため、Workfront では、月次および四半期次のリリース追跡の両方に対応するように、リリースのナンバリング方式を変更しています。最初の数字は年、2 番目の数字はリリースの月を表します。例：2024年4月のリリースは 24.4 となります。
>
>月次リリースと四半期リリースは、特に指定がない限り、毎月第 2 週の木曜日に公開される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>24.5 （2024 年 5 月 16 日（PT））</li><li>24.6 （2024 年 6 月 13 日（PT））</li><li>24.7 （2024 年 7 月 18 日（PT））</li></ul> | <ul><li>24.7 （2024 年 7 月 18 日（PT））</li></ul> |
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [Financial Management の機能強化](#financial-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> ビジネスルールを利用できるようになりました </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>管理者は、Workfrontの設定エリアでビジネスルールを追加できるようになりました。</p>
                        <p>ビジネス・ルールを使用すると、Workfrontオブジェクトに検証を適用し、特定の条件が満たされた場合にオブジェクトを作成、編集または削除できないようにすることができます。 ルールは、カスタムフォームの計算フィールドに類似した式を使用して作成されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年7月4日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
                            </li>
                        </ul>
                        <p><i>新しいUltimate プランに参加している組織のみが利用できます。</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Adobe Workfrontで一般入手可能なカスタムフォームデザイナー </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>24.7 リリースでは、フォームデザイナーが一般入手可能になり、Adobe Workfrontでカスタムフォームを作成および編集するためのデフォルトのエクスペリエンスになります。 新しいカスタムフォームを作成する場合、または既存のフォームを開く場合、フォームデザイナーのキャンバスタイルワークスペースが表示されます。</p>
                        <p>このリリース以降、従来のフォームビルダーに戻すオプションはなくなります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月19日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> 環境の昇格によるWorkfront環境間でのオブジェクトの移動 </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>環境のプロモーションにより、サンドボックス環境から実稼動環境など、あるWorkfront環境から別の環境にオブジェクトを移動できます。 組織のデータやレコードにリスクを与えることなく、オブジェクトを設定およびテストできます。 その後、これらのオブジェクトを再構成することなく実稼動環境に移動できるため、時間と労力を節約できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.6 リリースでは（2024 年 6 月 13 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> カスタムフォームデザイナーでのカスタムフォームおよびカスタムフィールドの共有 </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>新しいフォームデザイナー内で、カスタムフォームとカスタムフィールドの両方を共有できるようになりました。 これにより、カスタムフォームのユーザー間の共同作業が促進されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p><span class="preview">すべてのお客様向けの実稼動リリース：6 月 13 日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> 「フィールド」領域から新しいカスタムフィールドを追加する </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>カスタムフォームを開いてフィールドを作成することなく、Workfrontの「フィールド」領域から直接新しいカスタムフィールドまたはウィジェットを追加できるようになりました。 これにより、再利用可能なカスタムフィールドをすばやく作成できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> フォームデザイナーで使用できる複数選択ドロップダウンフィールドタイプ </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>ドロップダウンフィールドをより簡単に定義できるように、複数選択ドロップダウンフィールドをカスタムフォームデザイナーに追加しました。 このフィールドタイプを使用すると、ユーザーはドロップダウンリストから複数のオプションを選択できます。</p>
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

### Financial Management の機能強化

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}"> プロジェクトおよびタスクに使用できる請求可能および請求不可の費用フィールド </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>費用タイプをより簡単に確認できるように、費用は、プロジェクトとタスクの請求可能な費用と請求不可な費用に分割されています。 ビューとレポートに追加できるフィールドは以下のとおりです。</p>
                        <ul>
                            <li><p>予定請求可能費用コスト</p></li>
                            <li><p>請求不可の予定費用コスト</p></li>
                            <li><p>実際の請求不可の費用コスト</p></li>
                            <li><p>実際の請求不可の費用コスト</p></li>
                        </ul>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 5 月 10 日（PT）</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront for Experience Manager Assetsと Assets Essentials の機能強化 </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Experience Manager Assetsと Assets Essentials 統合のWorkfrontで次の改善が行われました。</p>
                        <ul>
                            <li><p>この統合では、クラウドサービスプロバイダーとしての GCP がサポートされるようになりました。 以前は、AWSと Azure がサポートされていました。</p></li>
                            <li><p>統合を通じてExperience Managerに送信されるファイルのサイズ上限が 30 GB に増えました。 以前は、上限は 5 GB でした。</p></li>
                        </ul>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月27日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様の実稼動環境：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> ヘッダーまたは「詳細」セクションで、タスクと問題のコミット日および条件を編集します </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>タスクとイシューを簡単に更新できるように、レイアウトテンプレートのタスクとイシューのヘッダーと詳細セクションに追加するオプションとして、「コミット日」フィールドと「条件」フィールドが追加されるようになりました。 ユーザーは、変更されたレイアウトテンプレートに割り当てられたときに、ページのヘッダーまたは詳細セクションからこれらのフィールドを更新できるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 5 月 30 日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動：24.6 リリースの場合（2024 年 6 月 13 日（PT））</p>
                            </li>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">より関連性の高い割り当てを、新規タスクワークフローに追加</a></p>
                        [!BADGE In Production for Fast Release &#x200B;]{type=Positive}
                        <p>プロジェクトやプロジェクトのタスクリストにタスクを追加する際に、関連性の高いスマート割り当てを行うための同じ機能が、「新規タスク」ボックスの「割り当て」フィールドに追加されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月13日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.5 リリースの場合（2024 年 5 月 16 日（PT））</p>
                            </li>
                        </ul>
                    <p><i>この機能は、プレビューおよび迅速リリースの実稼働から削除されました。</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">関連性の高いスマート割り当て</a></p>
                        [!BADGE In Production for Fast Release &#x200B;]{type=Positive}
                        <p>Workfront がタスクのスマート割り当ての計算と提案に使用するアルゴリズムを変更しました。新しいアルゴリズムは、タスクを割り当てる Workfront のエリア（タスクリスト、タスクヘッダーの割り当てエリア、ホーム、概要パネル）に適用されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年12月21日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.5 リリースの場合（2024 年 5 月 16 日（PT））</p>
                            </li>
                        </ul>
                    <p><i>この機能は、プレビューおよび迅速リリースの実稼働から削除されました。</i></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}"> デスクトッププルーフビューアのセキュリティアップデート </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Workfront Proof デスクトッププルーフビューア 2.1.35 セキュリティアップデートは、以前のリリースで特定された脆弱性のセキュリティバグ修正を提供します。</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md"> 休暇がワークロードバランサーに反映されるようになりました </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>タスクのプライマリ担当者が休暇をスケジュールした場合に作業をシームレスに調整するために、プロジェクトタイムラインが再計算される際に、ワークロードバランサーがプライマリユーザーとセカンダリユーザーの両方に時間を再割り当てするようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> 製品内ガイドのバックエンドの変更 </a></p>
                        <p>アドビでは、今後数週間で、製品内ガイドのテクノロジーの変更を実装します。 この移行の影響を最小限に抑えようとしましたが、一部のユーザーには、以前に表示されたガイドが表示される場合があります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>すべてのお客様向けの実稼動環境：2024 年 8 月中旬まで段階的に追加</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobeの統合エクスペリエンスを、より多くのWorkfront組織で利用できるようになりました </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Adobe Unified Experience のメリットに企業がアクセスできるように、既存のWorkfrontのお客様が利用できるようにする準備に着手しました。 </p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月20日（PT）</p>
                            </li>
                            <li>
                                <p>特定のお客様の実稼働環境：24.7 リリースの場合（2024 年 7 月 18 日（PT））</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Adobe統合シェルは、段階的なロールアウトで使用可能になります。 追加の組織は、24.10 および 25.1 リリースでAdobe統合シェルにオンボーディングされます。 </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> メインナビゲーションバーから「ヘルプ」ボタンが削除されました </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>統合シェル以外のユーザーのエクスペリエンスを統一するために、メインナビゲーションバーの「ヘルプ」ボタンが削除されました。 このボタンはWorkfrontのドキュメントにリンクされており、統合シェルのユーザーには表示されず、メインメニューのすべてのユーザーが利用できる同様のヘルプボタンと重複していました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年6月6日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様向けの実稼動リリース：24.7 リリースでは（2024 年 7 月 18 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> オブジェクトアクセスが制限されたユーザーの UI エクスペリエンスが向上 </a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>ユーザーがオブジェクトへのアクセス権を持っていない場合、Workfrontでは、そのオブジェクト名が表示されるすべての場所に「アクセスなし」と表示されます。 この改善されたエクスペリエンスは、Workfront API にも当てはまります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年3月27日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.5 リリースの場合（2024 年 5 月 16 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.7 リリースと（2024 年 7 月 18 日（PT））</p>
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

### Workfront のメンテナンスアップデート

2024年第 3 四半期リリースで行われたメンテナンス更新については、[Workfront のメンテナンスアップデート](https://experienceleague.adobe.com/ja/docs/workfront-known-issues/releases/current-updates)を参照してください。

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/home)の「新機能」の節を参照してください。
