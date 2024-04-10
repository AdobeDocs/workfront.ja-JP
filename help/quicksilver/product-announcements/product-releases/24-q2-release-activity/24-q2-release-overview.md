---
title: 2024 年第 2 四半期リリースの概要
description: このページでは、2024 年第 2 四半期リリースに含まれる機能について説明します。 これらの機能強化は、四半期全体を通じて実稼動環境で利用できるようにする予定です。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bdcfed70-1999-4c40-a38f-12c762c8c1c4
source-git-commit: d463a3878552f926c4b5a5c87e0f87764e60c60d
workflow-type: tm+mt
source-wordcount: '2167'
ht-degree: 19%

---

# 2024 年第 2 四半期リリースの概要

このページでは、2024 年第 2 四半期リリースに含まれる機能について説明します。 これらの機能強化は、四半期全体を通じて実稼動環境で利用できるようにする予定です。

<!--The 24.1 release webinar was on January 11, 2024. You can [register for the webinar to view an on-demand recording here](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview).-->
リリースウェビナーの代わりに、次の操作をお勧めします [Adobe Summitの登録](https://summit.adobe.com/na/) 次のWorkfront セッションを視聴するには：

[Adobe Workfrontの未来](https://reg.adobe.com/flow/adobe/as24/sessions/page/catalog?search=S302) 2024 年 3 月 26 日（PT）に、戦略的計画とワークフローの将来について説明します。 Workfront チームが、マーケティングライフサイクル全体を通じてビジネス能力に対処する計画を立てる方法を説明します。これらはすべて、作業を自動化し、ユーザーエクスペリエンスを簡素化し、生産性を高めるための AI ファーストのアプローチで行われます。

[エンドツーエンドのキャンペーン計画用のマーケティングカレンダーとツールを公開](https://reg.adobe.com/flow/adobe/as24/sessions/page/catalog?search=s304) 2024 年 3 月 28 日（PT）に、組織がエンドツーエンドの運用ライフサイクルを管理および視覚化できるように設計された新製品機能について説明します。

<span class="preview">オフサイクル機能（2024 年第 2 四半期のリリース日より前に実稼動環境にリリースされた機能）は、黄色でハイライト表示されます。</span>

>[!IMPORTANT]
>
>23.3 リリースには、組織を毎月のリリースに移行するオプションが含まれていました。そのため、Workfrontでは、毎月と四半期ごとのリリーストラックの両方を考慮して、リリースの番号付けスキームを変更しました。 最初の数値は年を示し、2 番目の数値はリリースの月を示します。 例：2024 年 4 月のリリースは 24.4 と読み取られます。
>
>月次および四半期ごとのリリースは、特に指定のない限り、月の 2 週目の木曜日に利用できる予定です。
>
>| 毎月のリリース | 四半期リリース |
>|----|----|
>| <ul><li>24.2 （2024 年 2 月 15 日（PT））</li><li>24.3 （2024 年 3 月 14 日（PT））</li><li>24.4 （2024 年 4 月 11 日（PT））</li></ul> | <ul><li>24.4 （2024 年 4 月 11 日（PT））</li></ul> |
>
>迅速リリースプロセスについて詳しくは、[迅速リリースプロセスを有効化または無効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [ドキュメント管理の機能強化](#document-management-enhancements)
* [ホームの機能強化](#home-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [更新ストリームと通知の機能強化](#update-stream-and-notification-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">表示ロジックとスキップロジックが、フォームデザイナーのプレビューモードで使用できるようになりました</a></p>
                        <p>ベータ版のカスタムフォームデザイナーを使用すると、プレビューモードで表示ロジックをテストし、ロジックをスキップできるようになりました。 これまで、ロジックが適用されている場合でも、すべてのフィールドがプレビューに表示されていました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 28 日（PT）</p>
                            </li>
                            <li>
                                <p>お客様向けの実稼動環境：24.4 リリースの場合（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">会社とユーザーは、高度なカスタムフォームフィールドをサポートするようになりました</a></p>
                        <p>外部検索フィールドやWorkfront ネイティブフィールドなどの高度なカスタムフォーム機能が、カスタムフォームを会社またはユーザーに添付する際に使用できるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 14 日（Pt）</p>
                            </li>
                            <li>
                                <p>お客様向けの実稼動環境：24.4 リリースの場合（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいパッケージタイプで JumpSeat 統合を使用できるようになりました</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>既存の JumpSeat 統合は、新しいパッケージタイプ（Select、Prime、Ultimate など）のいずれかを使用しているアカウントで使用できるようになりました。 統合を有効にするには、アクティブな JumpSeat サブスクリプションがまだ必要です。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月26日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfrontのネイティブフィールドは、フォームデザイナーのベータ版で使用できます</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>Workfront固有のフィールドをカスタムフォームに追加できるようになりました。 この新しいフィールドタイプを使用すると、カスタムフィールドで既存のデータを再作成しなくても、論理的な方法でデータを整理してユーザーに表示できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月29日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe IMSに移行した組織で属性マッピングを使用できるようになりました</a></p>
                        <p>[!BADGE In Production ]{type=Informative}</p><p>Workfront システム管理者は、Adobe IMSに移行した組織のユーザー属性マッピングを設定できるようになりました。 これにより、ユーザー情報が組織の SSO （シングルサインオン）プロバイダーからWorkfrontに渡されるので、ユーザーのデータはWorkfrontと SSO プロバイダーの両方に入力される必要がなくなります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月22日</p>
                            </li>
                            <li>
                                <p><span class="preview">すべてのお客様向けの実稼動リリース：2024 年 2 月 22 日（PT）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">スキップロジックと表示ロジックがフォームデザイナーのベータ版で使用できるようになりました</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>フォームデザイナーのベータ版で、既存の表示とスキップロジックを編集し、新しいロジックをカスタムフォームに追加できるようになりました。 使いやすいロジックビルダーを使用して、フォーム内の選択に基づいて、表示またはスキップするフィールドを定義できます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月8日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動：24.2 リリースの場合（2024 年 2 月 15 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの実稼動：未定</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### ドキュメント管理の機能強化

>[!IMPORTANT]
>
>にリストされている機能 **ドキュメント管理の機能強化** は段階的リリースの一部であり、特定の顧客のみが使用できます。

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">ドキュメントのレビューと承認に期限を追加する</a></p>
                        <p>ドキュメントのレビューまたは承認に割り当てられるユーザーまたはチームの期限を指定できるようになりました。 レビュー担当者と承認者は、指定した期限の 72 時間前とその 24 時間前にメール通知を受け取ります。 期限は、新しいホームエリアの承認ウィジェットにも反映されます。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 28 日（PT）</p>
                            </li>
                            <li>
                                <p>お客様向けの実稼動環境：24.4 リリースの場合（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">承認テンプレートの作成と使用</a></p>
                        <p>設定エリアで承認テンプレートを作成して、レビューと承認のプロセスを効率化できるようになりました。 承認テンプレートを使用すると、レビューと承認のプロセスを、次の方法でより繰り返し可能にすることができます
                        <ul>
                            <li>
                                <p>レビュー担当者と承認者の追加</p>
                            </li>
                            <li>
                                <p>期間の設定</p>
                            </li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 28 日（PT）</p>
                            </li>
                            <li>
                                <p>お客様向けの実稼動環境：24.4 リリースの場合（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">すべての承認に関する情報を 1 か所で表示する</a></p>
                        <p>承認リクエストを一目で管理および分析できるように、すべての承認ウィジェットに次の主要業績評価指標を追加しました。
                        <ul>
                            <li>
                                <p>決定による承認</p>
                            </li>
                            <li>
                                <p>平均承認時間</p>
                            </li>
                            <li>
                                <p>保留中の承認</p>
                            </li>
                            <li>
                                <p>期限切れの承認</p>
                            </li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 28 日（PT）</p>
                            </li>
                            <li>
                                <p>お客様向けの実稼動環境：24.4 リリースの場合（2024 年 4 月 11 日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-home-enhancements.md" class="MCXref xref" xrefformat="{para}">レイアウトテンプレートを使用して、新しいホームの管理者コントロールに追加された列オプション</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>管理者は、レイアウトテンプレートを使用して、特定の新しいホームウィジェットでユーザーが使用できる列をカスタマイズできるようになりました。 デフォルトの列の非表示や表示、既存のフィールドを新しい列として追加するオプションなどがあります。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年1月2日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動：24.2 リリースの場合（2024 年 2 月 15 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager統合における自動フォルダー作成ワークフローの機能強化</a></p><p>[!BADGE In Production ]{type=Informative}</p>
                        <p>Adobe Experience Manager フォルダーがニーズをより正確に反映できるように、Adobe Experience Managerにリンクされたフォルダーのワークフローを更新しました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 11 日（Pt）</p>
                            </li>
                            <li>
                                <p>すべてのお客様の実稼働環境：2024 年 3 月 14 日（PT）</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">新規タスク ワークフローにより関連性の高い割り当てが追加されました</a></p>
                        <!-- <p>[!BADGE In production for Fast Release ]{type=Positive}</p> -->
                        <p>プロジェクトおよびプロジェクトタスクリストにタスクを追加する際に、「新規タスク」ボックスの「割り当て」フィールドにより関連性の高いスマート割り当てに対して同じ機能を追加しました。</p>
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
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">より関連性の高いスマート割り当て</a></p>
                        <!-- <p>[!BADGE In production for Fast Release ]{type=Positive}</p> -->
                        <p>Workfrontがタスクのスマート割り当ての計算と提案に使用するアルゴリズムを変更しました。 新しいアルゴリズムは、Workfrontでタスクを割り当てる領域（タスクリスト、タスクヘッダーの「割り当て」領域、ホームおよび概要パネル）に適用されます。</p>
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
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-resource-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">ワークロードバランサーで手動で調整された割り当てのインジケーター</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p><p>ワークロードバランサーでの手動の調整や配分をより明確にするために、手動で調整された時間ごとの割り当てに鉛筆アイコンが表示されるようになりました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年10月12日（PT）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動：24.2 リリースの場合（2024 年 2 月 15 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### 更新ストリームと通知の機能強化

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">従来のコメント領域へのアクセスが削除されました</a></p>
                        <p>プロジェクト、タスク、イシュー、ドキュメントの更新領域の「新規コメント」切替スイッチを削除しました。 新しいコメント機能がデフォルトになり、これらのオブジェクトに使用できる唯一のオプションになりました。 この変更により、従来のコメントエクスペリエンスに戻すことはできなくなります。 さらに、ユーザーのプロファイルにある「更新状態の完了率を表示」設定も削除しました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年4月1日（PT）</p>
                            </li>
                            <li>
                                <p>すべてのお客様の実稼動環境：24.4 リリースの場合（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいホームウィジェットのクイックアクションで新しいコメントストリームを使用できるようになりました</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>新しいホームのマイ作業、マイプロジェクト、マイタスク、マイ問題ウィジェットの「新しい更新を追加」クイックアクションボタンに、新しいコメント機能が追加されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年 3 月 1 日（Pt）</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいコメントエクスペリエンスで利用できる追加のコメントセンター情報</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>新しいコメント機能のエクスペリエンスが次のように強化されました。</p>
                        <ul>
                            <li>
                                <p>コメンテーターの名前をクリックすると、そのコメンテーターの名前、役割、メールアドレスが情報ボックスに表示されます。 この情報は、同じ名前のユーザーが複数ある場合に、正しいユーザーを識別するのに役立ちます。 情報ボックスでコメンテーターの名前をクリックすると、そのコメンテーターのユーザープロファイルが開きます。</p>
                            </li>
                            <li>
                                <p>コメントテキストでメンションを受けると、タグ付けされたコメント内でユーザー名がハイライト表示されます。</p>
                            </li>
                        </ul>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月29日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいコメントエクスペリエンスの「システムアクティビティ」タブが、読み取り専用のコメントをサポートするようになりました</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>従来のコメント機能でシステムアクティビティレコードに追加されたコメントが、新しいコメント機能の「システムアクティビティ」タブに読み取り専用として入力されるようになりました。 新しいコメントエクスペリエンス内のシステムアクティビティレコードに返信することはできません。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月22日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">コメントとシステムアクティビティエントリの両方を取得する新しい「ストリームを更新」タブ</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>コメントとシステムアクティビティログの両方を時系列でまとめるために、すべてのオブジェクトの更新領域に 3 つ目のタブを導入します。 「すべて」タブは、ユーザーコメントとシステムアクティビティコメントの両方を 1 つの包括的なストリームで取得します。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月22日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">概要パネルで新しいコメントストリームを使用できるようになりました。</a></p><p>[!BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>タスクリストとイシューリストの概要パネルに、新しいコメント機能が追加されました。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024年2月22日</p>
                            </li>
                            <li>
                                <p>迅速リリースの実稼動環境：24.3 リリースの場合（2024 年 3 月 14 日（PT））</p>
                            </li>
                            <li>
                                <p>四半期リリースの制作：24.4 リリースと共に（2024 年 4 月 11 日（PT））</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2024 年第 2 四半期のルックアンドフィールの更新</a></p>
                        <p>Adobe Workfront アプリケーションの様々な領域のルックアンドフィールに対する小規模な更新が、2024 年第 2 四半期内に行われています。 特定のリリース日については、個々のリリースノートを確認してください。</p>
                    </td>
                    <td><p><b>公開日：</b></p>
                        <ul>
                            <li>
                                <p>プレビューリリース：2024 年第 2 四半期のリリース期間中</p>
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

Workfront Fusion の新機能は、2024 年第 2 四半期のリリーススケジュール以外の頻度で実稼動環境で使用できます。 最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

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

2024 年第 2 四半期リリースで行われたメンテナンス更新について詳しくは、を参照してください。 [Workfrontのメンテナンス更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja).

### トレーニングの更新

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[Workfront チュートリアルページ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)の「新機能」の節を参照してください。

