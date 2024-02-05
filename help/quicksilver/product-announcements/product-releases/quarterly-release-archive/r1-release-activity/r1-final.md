---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 最終版
description: 2018.3 リリースアクティビティ
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 99%

---

# R1 最終版

次の機能は、現在、プレビューまたはベータ版では使用できませんが、R1 の実稼動環境にリリースされます。

## 担当作業エリアからのプルーフの承認決定（Workfront）

ユーザーからプルーフに追加され、（スタンドアロン ProofHQ アプリケーションから、または Workfront 内の自動化ワークフローを使用して）「承認者」の役割か「レビュアーと承認者」の役割のいずれかが付与されると、承認リクエストが担当作業エリアの「承認」タブに表示されるようになりました。その後、プルーフを確認し、プルーフに関する承認の決定を Workfront から直接行うことができます。

自動化ワークフローを使用してプルーフにユーザーを追加する方法については、[Adobe Workfront 内でのプルーフの共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)で [Adobe Workfront 内でのプルーフの共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)を参照してください。

担当作業エリアから承認の決定を行う方法については、[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)で[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

## 担当作業エリア内でのプルーフ承認に関するレポート（Workfront）

プルーフ承認オブジェクトに基づいて、レポートを作成できるようになりました。このレポートを使用すると、まだ決定が行われていない、ユーザーの担当作業エリアからプルーフ承認に関してレポートできます。

プルーフ承認レポートには、次の情報が含まれています。

* 承認用に送信されたドキュメント
* 承認者の名前
* プルーフのバージョン
* プルーフ ID
* プルーフ作成日

オブジェクトに基づいてレポートを作成する際に、この承認にアクセスします（[カスタムレポートの作成](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照）。

プルーフ承認オブジェクトレポートについて詳しくは、[Adobe Workfront のオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)で [Adobe Workfront のオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の節を参照してください。

## ドラッグ＆ドロップを使用したドキュメントプルーフの新しいバージョンの自動生成（Workfront）

ドラッグ＆ドロップ手法を使用して、プルーフが必要な新しいバージョンのドキュメントを追加すると、プルーフが自動的に生成されます。プルーフには、元のプルーフまたは前のバージョンのプルーフと同じオプションおよびワークフローがあります。

これまでは、新しいバージョンのドキュメントを追加した場合、新しいバージョンに対するプルーフが自動的には生成されず、新しいバージョンのプルーフを再生成する必要がありました。

ドキュメントのその他メニューを使用して新しいバージョンをアップロードする場合、プルーフは自動的には生成されません。

詳しくは、次の節を参照してください。

## すべてのプルーフユーザーが Workfront インターフェイスから ProofHQ に直接アクセスできるようにするオプションを提供（Workfront）

これで、システム内のすべてのプルーフユーザーが、Workfront インターフェイスから直接 ProofHQ プレミアムアカウントに、シームレスにアクセスできるようになりました。有効にすると、すべてのプルーフユーザーに対して、ProofHQ サイトに誘導する ProofHQ アイコンがグローバルナビゲーションバーに表示されます。

このオプションは、デフォルトでは有効になっていません。このオプションを有効にするには、Workfront 技術サポートに連絡し、システムのすべてのプルーフユーザーにこのアクセス権を提供するようにリクエストしてください。

詳しくは、[Adobe Workfront からの Workfront Proof へのアクセス](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)で [Adobe Workfront からの Workfront Proof へのアクセス](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)を参照してください。

この変更以前は、Workfront 管理者のみが Workfront インターフェイスから ProofHQ サイトに直接アクセスできました。

## 送信メール用の新しい TLS セキュア接続オプション（Workfront）

独自のメールサーバーを使用した Workfront 通信の管理を選択した場合、送信メールで TLS セキュア接続を使用できるようになります。

この機能強化以前は、SSL セキュア接続を介した送信メールのみを有効にすることができました。

送信メールの設定について詳しくは、以下を参照してください。

## プレビューサンドボックス環境でメールを管理するための新しいフィールド

Workfront では、プレビューサンドボックス環境とカスタム更新環境からのすべてのメール通信を無効にするようになりました。プレビューサンドボックス環境またはカスタム更新環境からのメール通知を受け取る場合は、この機能をユーザー設定で有効にする必要があります。

詳しくは、以下を参照してください。

* [Adobe Workfront プレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)の [Adobe Workfront プレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

* [Adobe Workfront カスタム更新サンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)の「カスタム更新サンドボックスからのメールの受信」

## Outlook for Office 365（Workfront）

Outlook 365 用の Workfront アドインが利用できるようになりました。 

このアドインの使用について詳しくは、[Outlook for Office 365 での Workfront アドインの使用](https://support.workfront.com/hc/en-us/sections/205046167)を参照してください。

## モバイルアプリでの検索（Workfront）

Web アプリケーションで検索するのと同じように、モバイルアプリ内でオブジェクトを検索できるようになりました。新しい検索機能では最初に、最近使用した項目のリスト内の項目と、以前モバイルデバイスにダウンロードされたオブジェクトが検索されます。最近使用した項目のリストは、web アプリケーションに表示されるリストと同じです。

>[!NOTE]
>
>この機能は、2017年5月の最初の週に利用可能になる予定です。

モバイルアプリについて詳しくは、「モバイルで検索」の節を参照してください。

## モバイルアプリのヘルプの改善：チュートリアル（Workfront）

4月のモバイルリリースから、モバイルエクスペリエンスを紹介する新しいチュートリアル画面が表示されます。初めてモバイルアプリにログインし、機能を初めて使用する場合は、この機能の仕組みを説明する簡単なチュートリアルが表示されます。このチュートリアルは、特定の機能を初めて使用する場合に 1 回だけ表示されます。

モバイルアプリについて詳しくは、次を参照してください。

## PDF ドキュメント内の検索（ProofHQ）

PDF ドキュメント、Office ドキュメントおよび静的 web ページ内で検索を実行できるようになりました。

詳しくは、[プルーフ内のコンテンツの検索](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md)を参照してください。

## アップデートされたグローバルナビゲーションバー（ProofHQ）

Workfront と統合された ProofHQ Premium アカウントで、ProofHQ 内のグローバルナビゲーションバーに対して次の改善が行われました。

* 新しいユーザープロファイル画像
* ルックアンドフィールの更新

## カスタムビューにさらに情報を追加（ProofHQ）

カスタムビューに次の追加情報を含めることができるようになりました。

* **受信者レベルのデータ**\
  カスタムビューを設定して、受信者レベルのデータに関連する列（役割、位置、メールアラート、締め切り日、プルーフに追加された日付、受信者検索）を含めることができます。\
  詳しくは、[Workfront Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)を参照してください。
* **データのプルーフ**\
  カスタムビューを設定して、プルーフデータに関連するコメント数（すべてのバージョン）、ディスク上のサイズ、プルーフタイプ、バージョンごとのファイル数、コメント添付データ（ディスク上のサイズ、ファイル名）、サブフォルダーによるフィルターの列を含めることができます。\
  詳しくは、[Workfront Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)を参照してください。
* **自動ワークフローに関連するステージレベルのデータ**\
  自動ワークフローの個々のステージに関連する列（SOCD ステータス、ステージ期限、アクティブなステージ名、次のステージ名、ステージ名およびテンプレート）を含めるように、カスタムビューを設定できます。\
  詳しくは、[Workfront Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)を参照してください。

## プルーフレポート（旧称 Analytics）における改善（ProofHQ）

レポート機能（旧称 Analytics）には、次の改善が行われています。

* 新しいデフォルトのレポートタイプ：

   * プルーフのターンアラウンド時間
   * 遅延承認の割合
   * プルーフの最初のアクティビティ時間
   * コメントおよび返信の数

* レポートの印刷
* ルックアンドフィールの更新

## プレビュー環境での ProofHQ 機能の確認（ProofHQ）

ProofHQ にリリースされた機能は、実稼動環境にリリースする前に、プレビュー環境でテストできるようになります。

実稼動環境前にプレビュー環境に機能をリリースするこの新しいワークフローにより、ProofHQ 実稼動環境の今後のアップデートにより準備を整えることができます。

ProofHQ プレビュー環境について詳しくは、[プレビューサンドボックステスト環境 - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md) を参照してください。
