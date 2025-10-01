---
product-area: documents
navigation-topic: approvals
title: Frame.io 統合の概要
description: Frame.io 統合の概要
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: 9825f095a7be7debb5150ca4bd50f7cf6fd12295
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---

# Frame.io 統合の概要

Workfrontと Frame.io の統合により、プロジェクトコーディネーターはWorkfrontでプロジェクトを管理し作業を計画できますが、クリエイティブ、マーケター、関係者は Frame.io でアセットをレビューし承認できます。

## Adobe エンタープライズストレージに基づいて構築

この統合の中核となるのは、Adobe エンタープライズストレージです。これは、Workfrontや Frame.io などのAdobe エンタープライズ製品をまたいだアセットの中央リポジトリとして機能するクラウドベースのストレージソリューションです。<!--, and Creative Cloud.-->

Adobe エンタープライズストレージの主なメリットには、次のものがあります。

* クリエイティブおよび作業管理アセット向けの統合ストレージレイヤー
* 安全なアクセス制御を実現する、Adobe IMSを介した一元化された権限
* Workfrontと Frame.io <!--, and Creative Cloud apps --> 間でのアセットのエンドツーエンドの可視性
* 企業のニーズに応える拡張性の高いストレージとクォータ管理

詳しくは、[Adobe エンタープライズストレージの概要 ](/help/quicksilver/review-and-approve-work/esm-overview.md) を参照してください。

## 統一されたレビューと承認

Workfrontと Frame.io の統合では、Workfrontの統合承認機能を使用して、レビューと承認を管理します。 統合承認を使用すると、次のことができます。

* Workfrontから直接レビューと承認を作成および管理する
* レビューと承認のステータスをリアルタイムでトラッキングする
* フィードバックと承認を 1 か所で一元化
* すべての関係者がアセットの最新バージョンにアクセスできることを確認します
* AI レビュー担当者を利用して、ブランドコンプライアンスレビューを自動化します
* その他

詳しくは、[ 統合ドキュメント承認：記事インデックス ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md) を参照してください。


### Frame.io ビューアの使用

また、この統合は Frame.io ビューアとも接続します。 Frame.io ビューアは、

* マークアップ ツールとコメント ツール
* バージョン履歴と比較
* ビデオレビューのタイムスタンプ付きコメント
* 外出先でのレビューや承認のためのモバイルアクセス

詳しくは、[Frame.io 統合の概要 ](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md) を参照してください。

#### ビデオレビューの制限

ビデオプルーフリクエストの年間キャップは、組織のWorkfront ユーザーライセンス（Standard と Light）の合計有料ライセンスの 10% に設定されています。 この上限は組織レベルで適用されます。

使用量が上限の 80% と 100% に達すると、Workfront管理者に通知されます。

この制限は、Frame.io Enterprise のお客様には適用されません。

#### Frame.io ビューアでサポートされるファイルタイプ

Frame.io ビューアは、すべての一般的なビデオ、画像、オーディオ、PDFおよび MS® Office タイプをサポートしています。 サポートされているファイルの詳細なリストについては、[Frame.io のタイプ ](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io) を参照してください。

#### Frame.io ビューアのアクセスとライセンス

Frame.io ビューアは、すべてのWorkfront レビューおよび承認ワークフローのデフォルトビューアです。 これは、有料ライセンスを持つすべてのWorkfront ユーザーに自動的に含まれます。 レビューと承認に Frame.io ビューアを使用する場合、追加の Frame.io ライセンスは必要ありません。

組織がこの統合で利用できる追加の Frame.io 機能（Frame.io のプロジェクトへのアセットの直接アップロードなど）を利用する場合は、Frame.io エンタープライズライセンスを購入できます。 デモのスケジュールを設定し、完全な Frame.io ソリューションのメリットを確認するには、Adobe アカウント担当者にお問い合わせください。

Workfrontのプルーフ機能は、この統合では使用できません。

## Workfrontの強力なプロジェクト管理

Workfrontと Frame.io の統合により、プロジェクトコーディネーターはWorkfrontの強力なプロジェクト管理機能を活用して、作業の計画、トラッキング、管理を行うことができます。

Workfrontのプロジェクト管理について詳しくは、[ プロジェクト：記事のインデックス ](/help/quicksilver/manage-work/projects/create-projects/create-project.md) を参照してください。

### 構造と命名規則の適用

この統合は ESM を使用して構築されるので、プロジェクトとドキュメントを管理する際に注意すべき構造と命名規則がいくつかあります。

* オブジェクト名は一意である必要があり、複製できません
* ESM には、階層ツリー内の同じ親を持つピア・オブジェクトに対して一意の名前が必要
* ドキュメントが同じプロジェクトに属している場合、ドキュメントに同じ名前を付けることはできません

これらの制限を念頭に置いて、Workfrontは、競合を防ぐために必要に応じてオブジェクトまたはドキュメントの名前を自動的に変更します。

### 共有と権限

統合の一環として、ユーザー権限はWorkfrontで制御され、Frame.io に送られます。 つまり、Frame.io のプロジェクトにユーザーを招待したり、Frame.io のユーザー権限を変更したりすることはできません。 これらのアクションは、Workfrontのプロジェクト共有モーダルを介して実行する必要があります。

次の表に、Workfrontの権限が Frame.io 権限にどのようにマッピングされるかを示します。

<table>
<tr>
<th>Workfront ユーザー権限</th>
<th>Frame.io ユーザー権限</th>
</tr>
<tr>
<td>管理</td>
<td>編集と共有</td>
</tr>
<tr>
<td>参加</td>
<td>編集と共有</td>
</tr>
<tr>
<td>表示</td>
<td>コメントのみ</td>
</tr>
</table>



### Workfrontの Document Management

ドキュメントは、この統合でプロジェクトレベルで管理され、現時点ではタスクまたはイシューにアップロードできません。

ドキュメントアクセスは、プロジェクトレベルでも管理されます。 ユーザーがプロジェクトへのアクセス権を持っている場合、そのプロジェクトに関連付けられたすべてのドキュメントにアクセスできます。

### ドキュメントエクスペリエンスの制限

この統合はAdobe エンタープライズストレージを使用して構築されるので、Workfrontでの元のドキュメントエクスペリエンスにはいくつかの制限があります。

#### 制限事項

次の機能は、この統合には含まれません。

<!--* External document providers-->
* Workfrontのプルーフへのアクセス
* Workfrontのドキュメントビューア
* お気に入りのドキュメント
* ドキュメントを要求


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->
