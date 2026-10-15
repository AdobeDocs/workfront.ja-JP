---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Adobe クラウドストレージのロールアウト計画
description: Adobeクラウドストレージをユーザーに表示する方法を選択し、1つのグループで試験運用し、作業の順序を決めて、レビュー担当者、承認者、プロジェクトオーナーに驚きを与えないようにします。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# Adobe クラウドストレージのロールアウト計画

Adobe クラウドストレージがユーザーにリーチするタイミングと方法を決定します。 Workfront管理者がAdobe クラウドストレージを設定領域のデフォルトのストレージオプションとして設定するまで、何も変わらないので、誰かが作業する前にエクスペリエンスをテストし、チームを準備する時間があります。

この記事では、選択できるロールアウト設定、単一グループでの試験運用の方法、作業の推奨の順序について説明します。

## Adobe クラウドストレージのロールアウト方法の選択

2つの設定があり、1つは組織全体または特定のWorkfront グループに適用できます。 Adobe クラウドストレージで作成されるすべてのプロジェクトでは、デフォルトで統合承認とFrame.io ビューアが使用されます。

詳細な手順については、[組織のAdobe クラウドストレージを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)を参照してください。

### 設定オプション

* **Adobe クラウドストレージのみ**：新しいプロジェクトでは、デフォルトでAdobe クラウドストレージが使用されます。 ユーザーはレガシープロジェクトを作成できません。
* **Adobe クラウドストレージと従来のWorkfront ストレージ**：ユーザーがプロジェクトを作成する際に、Adobe クラウドストレージ（「新しいプロジェクト」）と従来のWorkfront ストレージ（「従来のストレージ」）のどちらかを選択します。 このオプションは、設定領域で「**ユーザーがストレージプロバイダー**」チェックボックスを選択することで有効になります。

>[!TIP]
>
>Adobe クラウドストレージを小規模なチームの前に配置するには、いずれかの設定を1つのWorkfront グループに適用します。 これにより、より広範に展開する前に、ターゲットを絞った試験運用を実施できます。 制御されたペーシングのグループレベルのロールアウトから始め、パイロットグループがエクスペリエンスを検証したら、組織全体に展開することをお勧めします。

既存のオブジェクトは、作成されたストレージモデルを保持します。 デフォルトのストレージ環境設定を変更しても、既存のオブジェクトは変更されません。

設定](assets/storage-preference-groups.png)の![ ストレージ環境設定

## ロールアウトの計画

Workfrontの環境は、それぞれ異なります。 Adobe クラウドストレージをユーザーのデフォルトとして設定する前に、ロールアウトの成功を計画する時間を確保してください。 以下の提案は正確なチェックリストではありませんが、独自の計画の出発点です。

### パイロットグループの選定

グループスコープのロールアウトでは、Adobeクラウドストレージをより小さなチームの前に置き、フィードバックを集め、より広範なロールアウトの前に調整することができます。 作業パターンが、早い段階で把握したい課題を表面化するのに十分な代表性を有するグループを選択します。

### 本番稼働前にテストする

Adobeクラウドストレージは、Workfrontサンドボックス環境で利用できるため、本番稼働前に多くのエクスペリエンスを検証できます。 Frame.io ビューアはサンドボックスでは利用できないので、実稼動環境での完全なレビューと承認のエクスペリエンスをパイロットグループで検証します。 詳しくは、[組織でAdobe クラウドストレージを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)を参照してください。

### 変更をエンドユーザーに伝える

レビュー担当者、承認者、プロジェクトオーナーにとって最も大きな変更点は、新しいドキュメント領域と、Adobe クラウドストレージプロジェクトのレビューと承認を強化するFrame.io ビューアです。 これらの機能の導入方法を計画することで、Adobeクラウドストレージプロジェクトを初めて体験した際に、何を期待できるかをユーザーに伝えることができます。 [統一されたレビューと承認の開始](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)記事は、エンドユーザー向けの資料を作成する際に便利な出発点です。

### 権限とガバナンスの確認

Adobe クラウドストレージプロジェクトでは、管理と投稿の両方がFrame.ioで編集と共有にマッピングされ、これには外部共有が含まれます。 Adobeのクラウドストレージにチームを導入する前に、共有パターンを確認し、それが自社のガバナンスモデルに適合するかどうかを判断してください。 詳しくは、[Adobe クラウドストレージの違い](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping)を参照してください。

### 監査テンプレートと命名

Adobe クラウドストレージでは、厳密な命名ルールが適用され、Workfrontでは、これらのルールと競合するオブジェクトの名前が自動的に変更されます。 テンプレートからプロジェクトを作成する場合は、作成したテンプレートの名前と構造がルールに合うようにレビューします。 詳しくは、[Adobe クラウドストレージの違い](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules)を参照してください。

### Workfront Fusionに関する計画

既存のプルーフベースのFusion シナリオは、引き続き従来のプロジェクトで機能しますが、Adobe クラウドストレージプロジェクトに対しては自動的に機能しません。 これらのシナリオに依存するチームをAdobe クラウドストレージに取り込む前に、各シナリオを「編集」、「再構築」、「廃止」に分類します。 詳しくは、[統一されたレビューと承認のためのWorkfront Fusion シナリオの更新](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)を参照してください。

### レポートの変更計画

統合された承認ワークフローのデータとレポートは、Canvas ダッシュボードに表示されます。 従来の承認レポートは自動的に引き継がれないので、パイロットチームが必要とする前に代替ダッシュボードを設定します。 詳しくは、[ レビューと承認用のレポートダッシュボードの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)を参照してください。

## 推奨シーケンス

この順序をテンプレートとして使用し、環境に合わせて調整します。

1. サンドボックスおよび本番環境のパイロットグループでエクスペリエンスをテストします。
2. Fusion シナリオを分類および更新し、Canvas ダッシュボードのレポートを作成します。
3. テンプレートを監査し、権限と共有モデルを確認します。
4. 変更を使用するレビュー担当者、承認者、プロジェクトオーナーに変更を伝える。
5. Adobe クラウドストレージをパイロットグループのデフォルトとして設定し、パイロットがエクスペリエンスを検証したら、より多くのグループまたは組織全体に展開します。
