---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 承認者の決定がプルーフ承認レポートにハイフンを表示する
description: 「プルーフの承認」レポートの「承認者の決定」フィールドのハイフンは、受信者がプルーフの意思決定の役割に留まっていないことを示します。
author: Courtney
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 25d403b9266c31a39c1dce6c1c45ad96ee90af28
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# 承認者の決定がプルーフ承認レポートにハイフンを表示する

## 問題

「プルーフ承認」レポートでは、「決定日」フィールドに日付が表示され、「決定待ち」フィールドがFalseの場合でも、受信者の「承認者の決定」フィールドにはハイフン（ – ）が表示されます。

![承認者の決定で、プルーフ承認レポートにハイフンが表示される](assets/approver-decision-hyphen.png)

## 原因

「承認者の決定」フィールドのハイフンは、受信者がプルーフの意思決定の役割を果たしていないことを意味します。 これは、次のような場合に発生します。

* 受信者はプルーフに追加され、決定を行い、後でワークフローから削除されました。 受信者がプルーフを再訪問した場合、プルーフシステムは訪問を決定変更として記録します。 受信者が承認者ではなくなったため、新しい決定はハイフンとして記録されます。
* 受信者のプルーフの役割が、レビュー担当者など、承認権限が含まれていない役割に変更されました。 各役割がプルーフに対して実行できるアクションについて詳しくは、[&#x200B; プルーフの役割の概要](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md)を参照してください。
* 受信者が決定を下した後、受信者のプルーフ権限プロファイルがダウングレードされました。

## レポートにおける意味

ハイフンは意図的なものです。 プルーフを承認するためにシステムが受信者を待っていないこと、および受信者がプルーフに関する意思決定の役割を持っていないことが示されます。

「決定日」フィールドには、受信者の最新の決定アクティビティの日付が表示されますが、受信者の決定はレポートでカウントされなくなります。

プルーフ承認レポートの作成と使用について詳しくは、[&#x200B; プルーフ承認レポートの使用](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md)を参照してください。
