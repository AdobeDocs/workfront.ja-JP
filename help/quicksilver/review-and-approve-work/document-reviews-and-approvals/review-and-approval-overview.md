---
product-area: documents
navigation-topic: approvals
title: アセットのレビューと承認の概要
description: Workfrontでの正式なレビューと承認プロセスについて詳しく説明します。
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 7e970f4f707937a62f68c191a7cbd5dfa26e471c
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# アセットのレビューと承認の概要

新しいアセットのレビューと承認ワークフローは、Workfrontと Frame.io の緊密な統合を中心に構築されています。 この統合は、各製品で提供される機能の最大限のメリットを活用し、それを組み合わせて、コンテンツ作成に関わるすべてのユーザーが選択したツールで機能し、両方のシステム間でリアルタイムに同期されるコメント、ファイル、ステータス更新にアクセスできます。

Frame.io の詳細については、 [Frame.io の概要](https://support.frame.io/en/collections/49298-getting-started).

## Workfrontでの作業の開始と計画

Workfront管理者は、Workfrontと Frame.io の統合を有効にします。そのためには、「セットアップ」領域でデフォルトの Frame.io アカウントを設定し、Workfrontで Frame.io ユーザーを指定します。 これにより、コーディネーターは、Workfrontプロジェクトと正式なレビューおよび承認を使用して、作業を計画および開始できます。

### デフォルトの Frame.io アカウントを設定する

Workfrontの管理者は、Workfrontの「セットアップ」領域にデフォルトの Frame.io アカウントを追加して、Workfrontと Frame.io の統合を開始します。 デフォルトの Frame.io アカウントを設定すると、統合によってWorkfrontと Frame.io の間に接続されたプロジェクトが作成されます。

詳しくは、[] を参照してください。

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Frame.io ユーザーを有効にする

Frame.io を定期的に使用するWorkfrontユーザーは、Frame.io ユーザーとしてマークする必要があります。 Workfrontの管理者は、Workfrontユーザープロファイルで Frame.io ユーザーを指定できます。

ユーザーがWorkfrontで Frame.io ユーザーとしてマークされ、プロジェクトに追加された場合、

* Frame.io に共同作業者として追加されます。
* 正式なレビューと承認を得るために、Frame.io からWorkfrontにアセットを送信できます。

>[!TIP]
>
>クリエイティブツールで定期的に作業するユーザーを有効にし、Frame.io ユーザーとしてレビューおよび承認用にアセットをアップロードすることをお勧めします。


詳しくは、[] を参照してください。

![](assets/Frame-enabled-user.png)


### Frame.io と連携するプロジェクトを作成する

デフォルトの Frame.io アカウントを追加し、Frame.io ユーザーを指定すると、プロジェクトコーディネーターは Frame.io に接続されたWorkfrontプロジェクトを作成できます。 接続されたプロジェクトを作成する際に、次の操作を実行できます。

* **タスクに Frame.io ユーザーを割り当て**:Frame.io 対応のユーザーは、タスクに割り当てられると、完了する作業があることを示す通知を電子メールで受け取ります。
* **プロジェクトを Frame.io ユーザーと共有します**:Frame.io と共有されるプロジェクトのユーザーは、Frame.io 内のプロジェクトへのアクセス権を付与します。
* **クリエイティブマテリアルを Frame.io と共有する**：一方向同期プロジェクトフォルダーを使用して、Workfrontからクリエイティブユーザーに Frame.io で直接手順と資料を送信できます。
* **タスクの進行状況の追跡**：クリエイティブは、完了したアセットを送信し、Frame.io を終了することなくタスクを完了とマークできます。

詳しくは、[] を参照してください。

<!--Preassign approval templates to tasks coming in the future-->


## Frame.io でのコンテンツ作成とコラボレーション

クリエイティブは、選択したツールにとどまり、Frame.io 内でピアレビューを作成、繰り返し、実行する自由を持つことができます。

クリエイティブが接続されたプロジェクトに追加されると、Frame.io を離れることなく、次の操作を実行できます。

* プロジェクトコーディネーターからの手順にアクセスする
* 非公式のピアレビューを行う
* 正式なレビューと承認を得るために、完了したアセットをWorkfrontに送信
* タスクのステータスを変更するか、タスクを完了に設定します
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Frame.io でのアセットのレビューについて詳しくは、

## アセットのレビューと承認

クリエイティブが Frame.io からWorkfrontに完了したアセットを送信すると、プロジェクトコーディネーターは、Workfrontで正式なレビューと承認プロセスを開始できます。

承認が作成された後、ユーザーは Frame.io に戻り、アセットにコメントを追加してマークアップします。 また、Frame.io ビューアで承認を決定することもできます。

### Workfrontでの正式なレビューと承認の開始

プロジェクトコーディネーターは、Workfrontの「設定」領域で、1 回限りのレビューと承認または再開可能な承認テンプレートを作成できます。 Frame.io でおこなわれたすべてのレビューと承認アクティビティも、Workfrontで記録されます。

プロジェクトコーディネーターは、レビュー担当者、承認者、またはその両方を割り当てることができます。

* **レビュー担当者** とは、アセットにコメントを付けることができます。 完了したら、レビューが完了したとマークできます。 <!--example of when to add reviewers-->
* **承認者** マークアップアセットにコメントを付けることができます。 承認プロセスを前に進める決定を下す必要があります。



Frame.io でのコメントは、Workfrontの「更新」タブに反映されます。 Workfrontでおこなわれた返信は、Frame.io には反映されません。

「チームのみ」とマークされたコメントは、「Workfrontの更新」タブに表示されません。

レビュー担当者と承認者は、次のように、単一使用または承認テンプレートに追加できます。

<!--can also assign teams and set deadline-->

* **単一使用の承認**：承認期限の設定

* **承認テンプレート**
「Workfrontの設定」領域で、標準ライセンスを持つユーザーは、結果として得られる承認テンプレートを作成できます。 テンプレート内で、ユーザーは期間を指定し、レビュー担当者と承認者を追加できます。 <!--do we want to mention any upcoming plans here? -->

  テンプレートを作成したら、Frame.io から送信されるアセットに適用して、Workfrontでの正式なレビューと承認プロセスを開始できます。
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Workfrontからアセットをアップロードし、レビューおよび承認のためにフレームに送信します。近日公開ですか？

### Frame.io でのアセットの承認

Frame.io 接続されたアセットの関係者は、Frame.io ビューア内で、Workfrontの更新ストリームや決定などに同期したコメントを使用して、確認および承認できます。

<!-- include screenshot from frame.io-->

Frame でのみ作業する場合は、リクエストを電子メールで通知できます。

Workfrontでのみ作業する場合は、自宅で承認ウィジェットを使用できます。

Frame.io ビューアには、作業中はいつでもからアクセスできます。

**Frame.io からのアセットの承認**
通知方法

決定 — 承認、変更を承認、作業を必要とする

**Workfrontからのアセットの承認**
通知方法

ホーム承認待ちウィジェット

E メール — 締切の E メール 72、24、および期限

外部 WF ユーザは、フレームのログインを作成するように求められます。

アセットがフレームに接続されていない場合は、WF でサムネールを表示し、コメントストリームを使用できます。 レビューおよび承認に関する決定は、おこなうことができます。

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### レビューおよび承認指標の追跡

ホームの承認速度レポートのウィジェット？

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## キャンペーンアセット承認ワークフローの例

導入準則？

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
