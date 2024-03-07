---
product-area: projects
navigation-topic: approvals
title: Workfrontと Frame.io を接続
description: Workfrontは、レビューと承認のプロセスで Frame.io を使用して、作業を希望する人に会います。 プロジェクトの管理と承認のプロセスはWorkfrontで管理され、レビューのプロセスは Frame.io で実行されます。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 2c1945cdc9f923ea7fdc750f69eeba2a026571ac
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 7%

---


# Workfrontと Frame.io を接続

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

Workfrontは、レビューと承認のプロセスで Frame.io を使用して、作業を希望する人に会います。 プロジェクトの管理と承認のプロセスはWorkfrontで管理され、レビューのプロセスは Frame.io で完了します。 統合を正しく設定するには、次の各節をすべて完了する必要があります。

* [Workfrontグループを Frame.io チームに接続する](#connect-a-workfront-group-to-a-frameio-team)
* [Workfrontプロジェクトを作成し、接続されたグループを追加する](#create-a-workfront-project-and-add-a-connected-group)



## アクセス要件

* この記事で説明する機能を使用するには、組織を手動でオンボーディングする必要があります。 詳しくは、 [Adobe Workfrontと Frame.io のネイティブ統合アルファ：概要](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).


## Workfrontグループを Frame.io チームに接続する

アドビは、この機能を 5 月の一般リリース向けに積極的に改善しています。

### 前提条件

* Frame.io チームを作成して、Workfrontグループにマッピングします。
* チームの API 開発者トークンを見つけます。 詳しくは、 [開発者トークン](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) Frame.io 開発者サイトの

### Workfrontグループを Frame.io チームに接続する

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**」をクリックします。
1. 既存のグループを選択するか、 **グループを作成**.
1. 左側のパネルで、 **Frame.io に接続**.
   ![](assets/connect-frame-group.png)
1. API 開発者トークンを入力します。
1. クリック **接続を開始**.
1. （条件付き）複数の Frame.io アカウントの管理者の場合、使用するアカウントを選択します。

## Workfrontプロジェクトを作成し、接続されたグループを追加する

Workfrontグループを Frame.io チームに接続した後、その接続したグループを持つプロジェクトを作成する必要があります。

### 前提条件

* 前の節で説明したように、Workfrontグループが Frame.io チームと連携している必要があります。

### Workfrontプロジェクトを作成し、接続されたグループを追加する

{{step1-to-projects}}

1. 新しいプロジェクトをゼロまたはテンプレートから作成します。 プロジェクトの作成方法について詳しくは、 [プロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. 左側のパネルで、を探します。 **プロジェクトの詳細**.

1. 次を検索： **グループ化** フィールドを選択し、「デフォルト」グループを削除します。

1. ドロップダウンメニューで、目的のグループを見つけます。 Frame.io に接続されているグループには、 Frame.io アイコンが表示されます。
   ![](assets/add-frame-group.png)

1. その他のプロジェクト設定の変更を行います。

1. 「**変更を保存**」をクリックします。

1. 次の節に進みます。

### タスクを追加し、統合ステータスをアクティブに設定します

>[!NOTE]
>
>サブタスクは、現在、接続された Frame.io プロジェクトではサポートされていません。


1. Frame.io に入力する必要があるタスクを作成します。

1. 必要なタスクを選択し、「 **編集**.

1. をスクロールします。 **カスタムForms** 」セクションに移動して、 Frame.io 統合フォームを探します。

   >[!IMPORTANT]
   >
   >このフォームを表示するには、接続された Frame.io グループを「プロジェクトの詳細」領域に割り当てる必要があります。 詳しくは、 [Workfrontプロジェクトを作成し、接続されたグループを追加する](#create-a-workfront-project-and-add-a-connected-group) 」を参照してください。


1. を有効にします。 **このタスクの統合ステータス** チェックボックスをオンにして、 **アクティブ**.
   ![](assets/frame-custom-form.png)

1. クリック **変更を保存**. プロジェクト名の横に Frame.io アイコンが表示されます。

1. タスクにユーザーまたはチームを割り当てます。

   >[!NOTE]
   >
   >タスクに追加されたユーザーやチームも Frame.io プロジェクトに追加されます。

1. 「プロジェクトドキュメント」領域にドキュメントまたはクリエイティブブリーフをアップロードします。

プロジェクトがまだ接続されていません。統合を完了するには、次の節に進む必要があります。

### Frame.io でのプロジェクトの有効化

1. プロジェクトのステータスを次の場所から変更： **計画** から **現在** または現在の値と等しいカスタムステータス。 これで統合が完了し、Frame.io 内のプロジェクト、タスクおよびすべてのドキュメントが生成されます。

プロジェクト名の横にある Frame.io アイコンは、統合が成功したときの紫色のシグナリングに変わります。 ユーザーには、Frame.io プロジェクトに招待する電子メールが送信されます。

>[!IMPORTANT]
>
>プロジェクトが Frame.io 用に接続されると、プロジェクトグループに対して行われた変更は Frame.io には反映されません。


