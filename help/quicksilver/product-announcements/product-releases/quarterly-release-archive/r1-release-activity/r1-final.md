---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 最終
description: 次の機能は、現在、プレビューまたはベータ版では使用できませんが、R1 - EDIT ME で実稼動環境にリリース中です。
author: Luke
feature: Product Announcements
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# R1 最終

次の機能は、現在、プレビューまたはベータ版では使用できませんが、R1 の実稼動環境にリリースされています。

## 自分の作業領域 (Workfront) で配達確認の承認を決定する

ユーザーが配達確認に追加し、承認者の役割またはレビュー担当者と承認者の役割 ( スタンドアロンの ProofHQ アプリケーションから、またはWorkfront内の自動ワークフローを使用 ) を許可すると、承認リクエストが「作業」領域の「承認」タブに表示されます。 その後、配達確認を表示し、配達確認に関する承認をWorkfrontから直接決定できます。

自動ワークフローを使用して配達確認にユーザーを追加する方法について詳しくは、 [Adobe Workfront内での配達確認の共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Adobe Workfront内での配達確認の共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

「自分の作業」領域から承認に関する決定を行う方法について詳しくは、 [作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## 自分の作業領域内 (Workfront) の校正承認のレポート

「配達確認の承認」オブジェクトに基づくレポートを作成できるようになりました。 このレポートを使用すると、決定がまだおこなわれていないユーザーの自分の作業領域からの配達確認の承認に関するレポートを作成できます。

配達確認の承認レポートには、次の情報が含まれます。

* 承認用に送信されたドキュメント
* 承認者の名前
* 配達確認のバージョン
* プルーフ
* 配達確認の作成日

この承認にアクセスするには、オブジェクトに基づくレポートを作成する際に、 [カスタムレポートの作成](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

配達確認の承認オブジェクトレポートについて詳しくは、 [Adobe Workfrontのオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) セクション [Adobe Workfrontのオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## ドラッグ&amp;ドロップを使用してドキュメント配達確認の新しいバージョンを自動生成する (Workfront)

ドラッグ&amp;ドロップ操作を使用して、校正が必要な新しいバージョンの文書を追加すると、配達確認が自動的に生成されます。 配達確認には、元の配達確認または以前のバージョンと同じオプションおよびワークフローがあります。

以前は、新しいバージョンのドキュメントを追加した場合、新しいバージョンでは配達確認が自動的に生成されず、新しいバージョンの配達確認を再生成する必要がありました。

「ドキュメントの詳細」メニューを使用して新しいバージョンをアップロードする場合、配達確認は自動的に生成されません。

詳しくは、

## すべての校正ユーザーがWorkfrontインターフェイス (Workfront) から直接 ProofHQ にアクセスできるようにします

これで、システム内のすべての校正ユーザーがWorkfrontインターフェイスから直接 ProofHQ Premium アカウントにシームレスにアクセスできるようになりました。 有効にすると、すべての校正ユーザーに対して、グローバルナビゲーションバーに ProofHQ アイコンが表示され、ProofHQ サイトに移動します。

このオプションは、デフォルトでは有効になっていません。 このオプションを有効にするには、Workfrontテクニカルサポートに連絡し、システムのすべての校正ユーザーにこのアクセス権を要求してください。

詳しくは、 [Adobe WorkfrontからWorkfront Proof にアクセス](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [Adobe WorkfrontからWorkfront Proof にアクセス](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

この変更がおこなわれる前は、Workfront管理者のみがWorkfrontインターフェイスから ProofHQ サイトに直接アクセスできます。

## 送信メール用の TLS Secure Connection (Workfront) の新しいオプション

独自の電子メールサーバーを使用してWorkfront通信を管理することを選択した場合、送信メールで TLS セキュア接続を使用できるようになります。

この機能強化がおこなわれるまでは、SSL セキュア接続を介してのみ送信メールを有効にすることができました。

送信メールの設定について詳しくは、を参照してください。

## プレビューサンドボックス環境で E メールを管理するための新しいフィールド

Workfrontは、プレビューサンドボックス環境とカスタム更新環境からのすべての電子メール通信を無効にするようになりました。 プレビューサンドボックスまたはカスタム更新環境から電子メール通知を受け取る場合は、ユーザー設定でこの機能を有効にする必要があります。

詳しくは、次の情報を参照してください。

* [Adobe Workfrontプレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [Adobe Workfrontプレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* カスタム更新サンドボックスからのメールの受信 [Adobe Workfront Custom Refresh Sandbox 環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook for Office 365 (Workfront)

Outlook 365 用Workfrontアドインが利用できるようになりました。 

アドインの使用方法の詳細については、 [Outlook for Office 365 でのWorkfrontアドインの使用](https://support.workfront.com/hc/en-us/sections/205046167)

## モバイルアプリ (Workfront) での検索

Web アプリケーションでの検索と同様に、モバイルアプリ内でオブジェクトを検索できるようになりました。 新しい検索機能では、最初に「最近使用した項目」リストの項目と、以前にモバイルデバイスにダウンロードされたオブジェクトを検索します。 最近使用した項目の一覧は、Web アプリケーションに表示される一覧と同じです。

>[!NOTE]
>
>この機能は、2017 年 5 月の最初の週に提供されます。

モバイルアプリについて詳しくは、  

## モバイルアプリのヘルプの改善：Tutorials(Workfront)

4 月のモバイルリリースから、モバイルエクスペリエンスを紹介する新しいチュートリアル画面が表示されます。 初めてモバイルアプリにログインし、機能を初めて使用する場合は、この機能の仕組みを説明する簡単なチュートリアルが表示されます。 このチュートリアルは、特定の機能を初めて使用する場合に 1 回だけ表示されます。

モバイルアプリについて詳しくは、を参照してください。

## PDFドキュメントで検索 (ProofHQ)

PDFドキュメント、Office ドキュメント、および静的 Web ページ内で検索を実行できるようになりました。

詳しくは、  [配達確認内のコンテンツを検索](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## 更新されたグローバルナビゲーションバー (ProofHQ)

Workfrontと統合された ProofHQ Premium アカウントで、ProofHQ 内のグローバルナビゲーションバーに対して次の改善が表示されるようになりました。

* 新しいユーザープロファイル画像 
* ルックアンドフィールの更新

## カスタムビューに追加情報を含める (ProofHQ)

カスタムビューに次の追加情報を含めることができるようになりました。

* **受信者レベルのデータ**\
   カスタムビューを設定して、受信者レベルのデータに関連する次の列を含めることができます。役割、位置、E メールアラート、期限、配達確認に追加された日付、および受信者の検索。\
   詳しくは、 [Workfront Proof Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **データの校正**\
   カスタム表示を設定して、校正データに関連する次の列を含めることができます。コメント数（すべてのバージョン）、ディスク上のサイズ、配達確認の種類、バージョンごとのファイル数、コメント添付データ（ディスク上のサイズ、ファイル名）、サブフォルダーでのフィルタリング。\
   詳しくは、 [Workfront Proof Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **自動ワークフローに関連するステージレベルのデータ**\
   カスタムビューを設定して、自動ワークフローの個々のステージに関連する次の列を含めることができます。SOCD ステータス、ステージ期限、アクティブステージ名、次のステージ名、ステージ名、テンプレート。\
   詳しくは、 [Workfront Proof Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## レポート（旧称 Analytics）(ProofHQ) の校正機能の改善

レポート機能（旧称 Analytics）には、次の機能強化が含まれています。

* 新しいデフォルトのレポートタイプ：

   * 配達確認の所要時間
   * 遅延承認の割合
   * 配達確認の最初のアクティビティ時間
   * コメントおよび返信の数

* レポートの印刷
* ルックアンドフィールの更新

## プレビュー環境での ProofHQ 機能の表示 (ProofHQ)

ProofHQ にリリースされた機能は、実稼動環境にリリースする前に、プレビュー環境でテストできるようになります。

実稼働前にプレビュー機能をリリースするこの新しいワークフローにより、ProofHQ 実稼働環境の今後のアップデートに備えることができます。

ProofHQ Preview 環境について詳しくは、 [サンドボックステスト環境のプレビュー — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
