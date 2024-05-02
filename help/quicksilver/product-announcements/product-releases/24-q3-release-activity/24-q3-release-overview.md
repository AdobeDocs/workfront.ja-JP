---
title: 2024 年第 3 四半期リリースの概要
description: このページでは、2024 年第 3 四半期リリースに含まれる機能について説明します。 これらの機能強化は、四半期を通じて本番環境で利用できるようになる予定です。
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 58c6062ef427d1ef615768a11e7dbd4835aafa5e
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 65%

---

# 2024 年第 3 四半期リリースの概要

このページでは、2024 年第 3 四半期リリースに含まれる機能について説明します。 これらの機能強化は、四半期を通じて本番環境で利用できるようになる予定です。

<!--The 24.1 release webinar was on January 11, 2024. You can [register for the webinar to view an on-demand recording here](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview).-->

<span class="preview">オフサイクル機能（2024 年第 3 四半期のリリース日より前に実稼動環境にリリースされた機能）は、黄色でハイライト表示されます。</span>

>[!IMPORTANT]
>
>23.3 リリースには、組織を毎月のリリースに移行するオプションが含まれていました。そのため、Workfront ではリリースのナンバリング方式を変更し、月ごとのリリーストラックと四半期ごとのリリーストラックの両方を考慮するようにしました。最初の数字は年、2 番目の数字はリリースの月を表します。例：2024年4月のリリースは 24.4 となります。
>
>月次リリースと四半期リリースは、特に指定がない限り、毎月第 2 週の木曜日に公開される予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>24.5 （2024 年 5 月 16 日（PT））</li><li>24.6 （2024 年 6 月）</li><li>24.7 （2024 年 7 月）</li></ul> | <ul><li>24.7 （2024 年 7 月）</li></ul> |
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

<!--* [Administrator enhancements](#administrator-enhancements)-->
* [プロジェクトの強化](#project-enhancements)
* [その他の機能強化](#other-enhancements)

<!--
### Administrator enhancements

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Multi-select dropdown field type available on the form designer</a></p>
                        [!BADGE New in Preview ]{type=Negative}
                        <p>To help you define dropdown fields more easily, we have added the Multi-Select Dropdown field to the custom form designer. This field type allows users to choose more than one option from a dropdown list.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: April 18, 2024</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.5 release (May 2024)</p>
                            </li>
                            <li>
                                <p>Production for quarterly release: With the 24.7 release (July 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>
-->

### プロジェクトの強化

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">新規タスク ワークフローにより関連性の高い割り当てが追加されました</a></p>
                        <!-- <p>[!BADGE In production for Fast Release ]{type=Positive}</p> -->
                        <p>プロジェクトやプロジェクトのタスクリストにタスクを追加する際に、関連性の高いスマート割り当てを行うための同じ機能が、「新規タスク」ボックスの「割り当て」フィールドに追加されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月13日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                                <p><span style="color: #ff0000;">この機能は、2024 年 3 月 18 日（PT）に迅速リリースのお客様向けに実稼動環境から削除されました。</span></p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動：未定</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">関連性の高いスマート割り当て</a></p>
                        <!-- <p>[!BADGE In production for Fast Release ]{type=Positive}</p> -->
                        <p>Workfront がタスクのスマート割り当ての計算と提案に使用するアルゴリズムを変更しました。新しいアルゴリズムは、タスク（タスクリスト、タスクヘッダーの割り当てエリア、ホーム、概要パネル）を割り当てる Workfront のエリアに適用されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2023年12月21日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                                <p><span style="color: #ff0000;">この機能は、2024 年 3 月 18 日（PT）に迅速リリースのお客様向けに実稼動環境から削除されました。</span></p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動：未定</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">オブジェクトアクセスが制限されたユーザーの UI エクスペリエンスが向上しました</a></p>
                        <!-- <p>[!BADGE In production for Fast Release ]{type=Positive}</p> -->
                        <p>ユーザーがオブジェクトへのアクセス権を持っていない場合、Workfrontでは、そのオブジェクト名が表示されるすべての場所に「アクセスなし」と表示されます。 この改善されたエクスペリエンスは、Workfront API にも当てはまります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 27 日（Pt）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.5 リリースの場合（2024 年 5 月 16 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリース用の実稼動版：24.7 リリースに併せて </p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2024 年第 3 四半期中のルックアンドフィールの更新</a></p>
                        <p>Adobe Workfront アプリケーションの様々な領域のルックアンドフィールに対する小規模な更新が、2024 年第 3 四半期内に行われています。 特定のリリース日については、個々のリリースノートを確認してください。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年第 3 四半期のリリース期間中</p>
                            </li>
                            <li>
                                <p><span class="preview">実稼動版リリース：リリースノートで日付を確認してください。</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>   
           </tbody>
        </table>



## お知らせ

### Workfront Fusion の機能強化

Workfront Fusion の新機能は、2024 年第 3 四半期のリリーススケジュール以外の頻度で実稼動環境で使用できます。 最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

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

2024 年第 3 四半期リリースで行われたメンテナンス更新について詳しくは、を参照してください。 [Workfrontのメンテナンス更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja).

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)の「新機能」の節を参照してください。
