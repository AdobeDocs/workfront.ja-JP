---
title: プロジェクトコーディネーター共同作業者の使用
content-type: reference
description: すぐに利用できるAI コラボレーターであるプロジェクトコーディネーターを活用して、プロジェクトのステータスを監視し、期限切れのタスクをフォローアップする方法を説明します。
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 8%

---
# プロジェクトコーディネーター共同作業者の使用

{{highlighted-preview-article-level}}

プロジェクトコーディネーターは、プロジェクトを監視し、重要なステータス情報を関係者に通知する、すぐに利用できるAI コラボレーターです。

プロジェクトコーディネーターを使用する場合、Workfront以外で担当者を設定する必要はありません。

プロジェクトコーディネーターの設定の手順については、「AI コラボレーターの設定」の「[&#x200B; プロジェクトコーディネーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)」を参照してください。

AI共同作業者の一般的な詳細については、[AI共同作業者の設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>Select、Prime、またはUltimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>プロジェクトコーディネーターを割り当てるには、プロジェクトの管理権限が必要です。</td> 
  </tr>
  </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Project Coordinatorの概要

プロジェクトコーディネーターは、プロジェクトを監視し、作業を軌道に乗せるのに役立ちます。 プロジェクトに割り当てられると、管理者が設定したスケジュールに基づいてプロジェクトの更新が送信されます。 アップデートには以下が含まれます。

* 進捗の概要
* プロジェクトの正常性
* 期限を過ぎている、またはリスクのあるタスクや承認
* フィールドまたは割り当てがありません

また、プロジェクトコーディネーターは、プロジェクトとそのタスクに関するコメントを追加できます。

管理者は、更新を送信する頻度、送信する時間、および更新を受け取るユーザーを設定します。

また、プロジェクトの更新にプロジェクトコーディネーターに言及して、オンデマンドでプロジェクトコーディネーターを実行することもできます。 プロジェクトコーディネーターは、その時点で実行するようにスケジュールされていない場合でも、指定されたときに実行されます。

>[!NOTE]
>
>プロジェクトコーディネーターの行動は、一般提供される前に変更される場合があります。

## プロジェクト コーディネーターをプロジェクトに追加する

管理者は、最初にプロジェクトコーディネーターを作成し、レイアウトテンプレートのプロジェクトヘッダーに「**プロジェクトコーディネーター**」フィールドを追加する必要があります。 次に、フィールドがプロジェクトヘッダーに表示されます。

詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

プロジェクトにプロジェクトコーディネーターを割り当てるには：

1. プロジェクトコーディネーターを割り当てるプロジェクトに移動します。
1. プロジェクトヘッダーで、「**プロジェクトコーディネーター**」フィールドをクリックします。
1. 割り当てるプロジェクトコーディネーターを選択します。

   ウィンドウには、選択したプロジェクトコーディネーターの説明と、プロジェクトコーディネーターが実行するアクションが表示されます。
1. 「**適用**」をクリックします。

## プロジェクトコーディネーターに言及して実行します

スケジュールされた更新に加えて、プロジェクトに関する更新でプロジェクト コーディネーターを@mentioning定することで、いつでもプロジェクト コーディネーターにトリガーを送ることができます。 プロジェクトコーディネーターは、その時点で実行するようにスケジュールされていない場合でも、記載されているとすぐに実行されます。

プロジェクトコーディネーターについて言及するには：

1. プロジェクトコーディネーターが割り当てられているプロジェクトに移動します。
1. プロジェクトの&#x200B;**更新**&#x200B;領域を開きます。
1. 「更新」フィールドに「**@**」と入力し、プロジェクトコーディネーターを選択します。
1. メッセージを追加してから、更新を投稿します。

   プロジェクトコーディネーターが応答を実行し、投稿します。

>[!NOTE]
>
>@mentionームとプロジェクトをトリガーする前に、プロジェクト コーディネーターをプロジェクトに割り当てる必要があります。

## プロジェクトコーディネーターの設定

プロジェクトコーディネーターの設定の手順については、「AI コラボレーターの設定」の「[&#x200B; プロジェクトコーディネーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)」を参照してください。
