---
content-type: release-notes
keywords: メモ，四半期，更新，リリース
navigation-topic: 2021-2-release-activity
title: 21.2 校正機能の強化
description: ここでは、プレビュー環境の 21.2 リリースでおこなわれたすべての校正機能の強化について説明します。 これらの機能強化は、2021 年 5 月 10 日の週に実稼動環境で利用可能になる予定です。 21.2 リリースで使用できるすべての変更点の一覧については、 21.2 リリースの概要を参照してください。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 1f82c397-5cb6-4adc-bb84-f5b1e1ed9d5e
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 21.2 校正機能の強化

ここでは、プレビュー環境の 21.2 リリースでおこなわれたすべての校正機能の強化について説明します。 これらの機能強化は、2021 年 5 月 10 日の週に実稼動環境で利用可能になる予定です。 21.2 リリースで使用可能なすべての変更点の一覧については、 [21.2 リリースの概要](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 配達確認の決定がドキュメントリストに表示されるようになりました

>[!NOTE]
>
>新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

配達確認の全体的な決定が、デフォルトのドキュメントリストビューに表示されるようになりました。

この機能強化により、全体的な決定を持つすべての配達確認を、デフォルトのリストビュー内で直接簡単に確認できます。 これにより、別のページに移動する必要なく、配達確認の進行状況を簡単に見つけることができます。

以前は、配達確認の決定全体を表示するには、ドキュメントの詳細と配達確認のワークフローに移動する必要がありました（複数回のクリックが必要）。

配達確認の決定について詳しくは、 [「ドキュメント」領域](../../../documents/managing-documents/documents-area.md).

この機能は、 [新しいWorkfrontエクスペリエンスでの配達確認とバージョンの管理](https://one.workfront.com/s/learningpath3/manage-proofs-and-versions-in-the-new-workfront-experience-MCPBYNLTQSS5H4NG7C27IPCVR5YA) Workfront One の学習パス

## 配達確認の承認レポートの新しいフィールド

有用な校正情報を表面化するために、配達確認の承認レポートに次のフィールドを追加しました。

* **決定日：** 承認者が配達確認を決定した日付が表示されます。 この日付は、配達確認の印刷の概要でも確認できます。
* **承認者ステージ：** 現在のステージ情報を表示します。
* **ワークフローテンプレート：** 配達確認に関連付けられているワークフローテンプレートを表示します。 テンプレートが添付されていない場合、列は空白になります。

これらのフィールドは、デフォルトのレポートには含まれていません。 表示する場合は、追加する必要があります。

この機能は、 [配達確認のシステム設定、パート 2：ワークフロー管理](https://one.workfront.com/s/learningpath3/proof-system-setups-part-2-workflow-management-MCKUF6NTIJ6BGMXHBCXXX6NN53EA) Workfront One の学習パス

## 新しいバージョンを生成する際に既存の配達確認ワークフローを引き継ぐ

>[!NOTE]
>
>この機能は、2021 年 3 月 30 日にプレビュー環境から、2021 年 4 月 1 日に実稼動環境から削除されました。 21.1 リリースには含まれません。

これで、既存の配達確認ワークフローは、生成方法に関係なく、作成した新しいバージョンに引き継がれます。

以前は、Workfrontでの生成場所に応じて、配達確認のワークフローの実行方法に若干の違いがありました。

詳しくは、 [配達確認の新しいバージョンの作成](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/create-new-proof-version.md).
