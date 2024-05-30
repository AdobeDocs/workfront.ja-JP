---
product-area: projects
navigation-topic: approvals
title: Workfront と Frame.io の接続
description: Workfront では、作業への参加を希望する人物に会うためのレビューと承認プロセスで Frame.io を使用します。プロジェクトの管理と承認プロセスは Workfront で管理し、レビュープロセスは Frame.io で行います。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 8529b4d5-9732-4dd6-bf81-191aea1ed68c
source-git-commit: a8a5205616a0bf30c5ba4b27a2ffb9fae4d52ac4
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 95%

---

# Workfront と Frame.io の接続

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

Workfront では、作業への参加を希望する人物に会うためのレビューと承認プロセスで Frame.io を使用します。プロジェクトの管理と承認プロセスは Workfront で管理し、レビュープロセスは Frame.io で行います。統合を正常に設定するには、次の節をすべて完了する必要があります。

* [Workfront グループを Frame.io チームに接続](#connect-a-workfront-group-to-a-frameio-team)
* [Workfront プロジェクトを作成し、接続されたグループを追加する](#create-a-workfront-project-and-add-a-connected-group)



## アクセス要件

* この記事で説明されている機能を使用するには、組織をベータ版に手動でオンボーディングする必要があります。 詳しくは、を参照してください [Adobe Workfrontと Frame.io のネイティブ統合ベータ版](/help/quicksilver/review-and-approve-work/Documents/wf-frame-alpha.md).


## Workfront グループを Frame.io チームに接続

5 月の一般提供に向けて、この機能を積極的に改善しています。

### 前提条件

* Workfront グループにマッピングする Frame.io チームを作成する。
* チームの API 開発者トークンを見つける。詳しくは、Frame.io 開発者サイトの[開発者トークン](https://developer.frame.io/docs/getting-started/authentication#developer-tokens)を参照してください。

### Workfront グループを Frame.io チームに接続

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**」をクリックします。
1. 既存のグループを選択するか、「**グループを作成**」をクリックします。
1. 左側のパネルで、「**Frame.io に接続**」をクリックします。
   ![](assets/connect-frame-group.png)
1. API 開発者トークンを入力します。
1. 「**接続を開始**」をクリックします。
1. （条件付き）複数の Frame.io アカウントの管理者である場合は、使用するアカウントを選択します。

## Workfront プロジェクトを作成し、接続されたグループを追加する

Workfront グループを Frame.io チームに接続したら、その接続されたグループでプロジェクトを作成する必要があります。

### 前提条件

* 前のセクションで説明したように、Workfront グループが Frame.io チームに接続されている必要があります。

### Workfront プロジェクトを作成し、接続されたグループを追加する

{{step1-to-projects}}

1. 新しいプロジェクトを最初から作成するか、テンプレートから作成します。プロジェクトの作成方法については、[プロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project.md)を参照してください。

1. 左側のパネルで、「**プロジェクトの詳細**」を見つけます。

1. 画面の右側にある「**グループ**」フィールドを見つけて、デフォルトグループを削除します。

1. ドロップダウンメニューで、目的のグループを見つけます。Frame.io に接続されているグループには、Frame.io アイコンが表示されます。
   ![](assets/add-frame-group.png)

1. その他のプロジェクト設定を変更します。

1. 「**変更を保存**」をクリックします。

1. 次の節に進みます。

### タスクを追加し、統合ステータスをアクティブに設定する

>[!NOTE]
>
>サブタスクは現在、接続されている Frame.io プロジェクトではサポートされていません。


1. Frame.io に入力する必要があるタスクを作成します

1. 必要なタスクを選択して、「**編集**」をクリックします。

1. 「**カスタムフォーム**」セクションまでスクロールし、Frame.io 統合フォームを見つけます。

   >[!IMPORTANT]
   >
   >このフォームを表示するには、接続された Frame.io グループをプロジェクト詳細エリアに割り当てる必要があります。詳しくは、この記事の [Workfront プロジェクトを作成し、接続されたグループを追加する](#create-a-workfront-project-and-add-a-connected-group)を参照してください。


1. 「**このタスクの統合ステータス**」チェックボックスをオンにし、「**アクティブ**」を選択します。
   ![](assets/frame-custom-form.png)

1. 「**変更を保存**」をクリックします。プロジェクト名の横に Frame.io アイコンが表示されます。

1. タスクにユーザーまたはチームを割り当てます。

   >[!NOTE]
   >
   >タスクに追加されたユーザーまたはチームは、Frame.io プロジェクトにも追加されます。

1. プロジェクトドキュメントエリアに、ドキュメントまたはクリエイティブ概要をアップロードします。

プロジェクトはまだ接続されていません。統合を完了するには、次の節に進む必要があります。

### Frame.io でプロジェクトを有効にする

1. プロジェクトの状態を&#x200B;**計画**&#x200B;から&#x200B;**進行中**、または現在と同等のカスタムステータスに変更します。これで、統合が完了し、Frame.io にプロジェクト、タスクおよびドキュメントが生成されます。

プロジェクト名の横にある Frame.io アイコンが紫色に変わり、統合が成功したことを示します。Frame.io プロジェクトに招待するメールがユーザーに届きます。

>[!IMPORTANT]
>
>プロジェクトが Frame.io に接続されても、プロジェクトグループに加えられた変更は Frame.io には反映されません。
