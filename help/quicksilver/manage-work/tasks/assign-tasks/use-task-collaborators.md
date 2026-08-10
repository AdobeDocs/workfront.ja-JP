---
title: タスク共同作業者の使用
content-type: reference
description: Workfront タスクに割り当てることができるタスクコラボレーター、AI コラボレーターの使用方法について説明します。
author: Becky
feature: Work Management, Tasks
source-git-commit: a05312fa1def1db593743e5e6d385da0b393d5d4
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 4%

---

# タスク共同作業者の使用

{{highlighted-preview-article-level}}

タスクコラボレーターは、ドキュメントやアセットのレビューに使用される既存のレビューアータイプのAI コラボレーターに加えて、Workfront タスクに直接割り当てることができるAI コラボレーターです。 他のAI共同作業者と同様に、タスク共同作業者は設定エリアで設定され、ユーザーと同じようにタスクに割り当てられます。

タスクコラボレーターは、MCP サーバーのように、設定したエージェントに接続します。

Workfrontでのタスクコラボレーターの作成について詳しくは、「[ タスクコラボレーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)」の「AI コラボレーターの設定」を参照してください。

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
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* タスクコラボレーターとして使用する前に、Copilot、Claude、またはWriter.aiでエージェントを設定する必要があります。

## タスクコラボレーターの概要

タスクコラボレーターは、MCP エージェントをWorkfrontの特定のタスクに割り当てる方法です。 Copilot Studio、Claude、Writer.aiなどのアプリでエージェントを設定し、そのエージェントをTask CollaboratorとしてWorkfrontに接続します。 その後、ユーザーを割り当てるのと同じように、タスクに割り当てることができます。

ワークフローの例には、次のようなものがあります。

* タスクにアップロードされた画像を検出し、エージェントに与えられた基準に基づいてバリエーションを生成し、新しい画像をタスクにアップロードします。
* タスクの説明からコピーを生成し、エージェントで設定されたガイドラインに照らしてコピーを確認し、更新ストリームにコピーを投稿します。
* イベントの詳細を読み取り、欠けている詳細を特定し、欠けている詳細に関する質問を更新ストリームに投稿します。

>[!NOTE]
>
>* エージェントの責任と機能に関する具体的な詳細は、Workfrontではなく、エージェントが作成されるアプリケーションで設定されます。
>* タスクコラボレーターは現在、Copilot Studio、Claude、およびWriter.aiで作成されたエージェントをサポートしています。
>* Copilot Studioでエージェントを設定する場合、セキュリティを&#x200B;**認証なし**&#x200B;に設定する必要があります。
>* Workfrontでのタスクコラボレーターの作成について詳しくは、「[ タスクコラボレーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)」の「AI コラボレーターの設定」を参照してください。

## タスク共同作業者の開始トリガー

タスク共同作業者がタスクに割り当てられている場合、次のいずれかの状況が発生すると作業が開始されます。

* タスクコラボレーターは、開始準備ができているタスクに割り当てられます。 （例えば、タスクに先行タスクがある場合、先行タスクは完了します）。
* タスクコラボレーターとユーザーがタスクに割り当てられ、タスクコラボレーターが最初に割り当てられます。
* タスクコラボレーターが既に割り当てられているタスクを開始できます。 （例えば、タスクに先行タスクがある場合、先行タスクは完了します）。
* タスクコラボレーターとユーザーが既に割り当てられているタスクを開始する準備が整います。 （例えば、タスクに先行タスクがある場合、先行タスクは完了します）。
* ユーザーとタスクコラボレーターがタスクに割り当てられ、ユーザーが削除されます。
* ユーザーとタスクコラボレーターがタスクに割り当てられ、タスクコラボレーターがタスクのプライマリ担当者として設定されます。

次の状況では、タスクコラボレーターはタスクの作業を開始しません。

* タスク共同作業者は、既にユーザーが割り当てられているタスクに割り当てられます。
* タスクの共同作業者がタスクに@mentionedり込まれます。
* タスクコラボレーターは、既にタスクコラボレーターが割り当てられているタスクに割り当てられます。 この場合、最初に割り当てられたタスクコラボレーターのみがタスクの作業を開始します。
* タスクコラボレーターは、開始準備ができていないタスクに割り当てられています。 （例えば、タスクに先行タスクがある場合、先行タスクはまだ完了していません）。

## タスク共同作業者のタスクへの割り当て

タスク共同作業者は、ユーザーの割り当てと同じようにタスクに割り当てられます。

使用可能な担当者のリストでタスクコラボレーターを検索する場合、タスクコラボレーターの名前は名前のみになります。

手順については、[ タスクの割り当て](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)を参照してください。
