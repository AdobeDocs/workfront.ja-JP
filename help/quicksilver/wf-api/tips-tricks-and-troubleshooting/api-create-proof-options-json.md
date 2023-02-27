---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API で高度な校正オプションを追加
description: Adobe Workfront API で高度な校正オプションを追加
author: Becky
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Adobe Workfront API を使用して配達確認を作成する際の詳細な校正オプションの追加

Workfront API で配達確認を作成する際に、高度な校正オプションを追加できます。

API を使用して配達確認に校正オプションを追加するには、次のいずれかのワークフローを使用します。

* （推奨）Workfront API を使用して簡単な配達確認を作成し、ProofHQ API を使用して配達確認に高度な校正オプションを追加します

* Workfront API で JSON を使用して高度な校正オプションを使用し、配達確認を作成する

## Workfront API と ProofHQ API を使用した配達確認の作成（推奨） {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

ここでは、Workfront API と ProofHQ API を組み合わせて、Workfront API を使用して高度な校正オプションで配達確認を作成する方法について説明します。

ProofHQ API には、Workfront API では配達確認に使用できない様々なアクションが含まれています。 これらのアクションを使用すると、Workfront API で使用可能な値よりも正確に配達確認を変更または設定できます。

ProofHQ API の概要については、 [PoofHQ の概要](../../proofhq-api/general/overview.md). また、 [ProofHQ ドキュメント](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* Workfront API は REST-ful API です。 ProofHQ API は SOAP API です。
>* ProofHQ API で作成された配達確認は、Workfrontに自動的にリンクされません。 したがって、ProofHQ API を使用して配達確認を更新する前に、Workfront API で配達確認を作成することをお勧めします。
>


### 高度な校正オプションを使用して配達確認を作成する

1. を使用した配達確認の作成 `Document createProof` アクションを使用して、Workfront API で実行できます。

   >[!NOTE]
   配達確認を作成する場合は、 advancedProofingOptions パラメーターに値を指定しないでください。

1. 配達確認を作成した後、ProofHQ API を使用して詳細オプションを追加します。

### 例

この節では、ProofHQ API を使用して実行できる更新例を示します。

**例:**

* [配達確認は、ダウンロードしたり、メッセージを含めたり、公開共有したりできます](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [非公開（必須ではなく）で、1 つの承認のみが必要になるようにステージを更新します](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [主な意思決定者のいない配達確認に 2 人の受信者を追加](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**配達確認は、ダウンロードしたり、メッセージを含めたり、公開共有したりできます**

このエンドポイントのドキュメントは、 [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) ページ。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**非公開（必須ではなく）で、1 つの承認のみが必要になるようにステージを更新します**

このエンドポイントのドキュメントは、 [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) ページ。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**主な意思決定者のいない配達確認に 2 人の受信者を追加**

このエンドポイントのドキュメントは、 [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) ページ。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Workfront API で JSON を使用した配達確認の作成

ここでは、Workfront API で JSON をパラメーター値として使用し、Workfront API で高度な校正オプションを使用して配達確認を作成する方法について説明します

### 高度な校正オプションを使用して配達確認を作成する

Workfront API で配達確認を作成するには、 `Document createProof` アクション。 このアクションは、 `advancedProofingOptions` パラメーターに含まれる値の型 `string`. 高度な校正オプションを `createProof` 「 」アクションの場合は、 `advancedProofingOptions` JSON 形式のパラメーター。

>[!NOTE]
advancedProofingOptions JSON に含めるフィールドの予測は困難な場合があります。 Workfrontでの高度な校正を使用しながら、組織のネットワークデータを調べ、組織で一般的に使用されるフィールドと値に基づいて JSON を設定する必要がある場合があります。
これらのフィールドの予測は困難な場合があるので、Workfront API を使用して配達確認を作成し、ProofHQ API を使用して更新することをお勧めします。 詳しくは、 [Workfront API と ProofHQ API を使用した配達確認の作成（推奨）](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) この記事では、

### 例

この例では、 `advancedProofingOptions` パラメーター。 お使いの `advancedProofingOptions` JSON ファイルに含めるフィールドの数は、ここに示す数よりも多いか少なくなります。

**例:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
