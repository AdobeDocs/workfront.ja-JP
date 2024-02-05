---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API を使用した詳細プルーフオプションの追加
description: Adobe Workfront API を使用した詳細プルーフオプションの追加
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 100%

---


# Adobe Workfront API を使用してプルーフを作成する際の詳細校正オプションの追加

Workfront API でプルーフを作成する際に、詳細プルーフオプションを追加できます。

API を使用してプルーフにプルーフオプションを追加するには、次のいずれかのワークフローを使用します。

* （推奨）Workfront API を使用してシンプルなプルーフを作成したあと、ProofHQ API を使用してプルーフに詳細プルーフオプションを追加する

* Workfront API で JSON を使用して、詳細プルーフオプションを設定したプルーフを作成する

## Workfront API と ProofHQ API を使用したプルーフの作成（推奨） {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

この節では、Workfront API と ProofHQ API を組み合わせて、詳細プルーフオプションを設定したプルーフを作成する方法について説明します。

ProofHQ API には、Workfront API ではプルーフで使用できない様々なアクションが含まれています。これらのアクションを使用すると、Workfront API を使用する場合よりも精度の高いプルーフにすることができます。

ProofHQ API の概要については、[PoofHQ の概要](../../proofhq-api/general/overview.md)を参照してください。また、[ProofHQ ドキュメント](https://api.proofhq.com/home.html)も参照してください。

>[!NOTE]
>
>* Workfront API は REST-ful API です。ProofHQ API は SOAP API です。
>* ProofHQ API で作成されたプルーフは、自動的には Workfront にリンクされません。したがって、ProofHQ API を使用してプルーフを更新する前に、Workfront API でプルーフを作成することをお勧めします。
>

### 詳細プルーフオプションを設定したプルーフを作成

1. Workfront API の `Document createProof` アクションを使用してプルーを作成します。

   >[!NOTE]
   >
   プルーフを作成する際に、`{}` を `advancedProofingOptions` パラメーターの値として設定します。

1. プルーフを作成した後、ProofHQ API を使用して任意の詳細オプションを追加します。

### 例

この節では、ProofHQ API を使用して行える更新の例をいくつか示します。

**例：**

* [プルーフがダウンロード可能で、メッセージを含み、公開される](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [プライベートでも必須でもなく、必要な承認が 1 回のみになるようにステージを更新する](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [主要な校正判断者のいないプルーフに担当者を 2 人追加する](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**プルーフがダウンロード可能で、メッセージを含み、公開される**

このエンドポイントのドキュメントについては、[ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) ページを参照してください。

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

**プライベートでも必須でもなく、必要な承認が 1 回のみになるようにステージを更新する**

このエンドポイントのドキュメントについては、[ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) ページを参照してください。

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

**主要な校正判断者のいないプルーフに担当者を 2 人追加する**

このエンドポイントのドキュメントについては、[ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) ページを参照してください。

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

## Workfront API で JSON を使用したプルーフの作成

この節では、Workfront API で JSON をパラメーター値に使用して、詳細プルーフオプションを設定したプルーフを Workfront API で作成する方法について説明します。

### 詳細プルーフオプションを設定したプルーフを作成

`Document createProof` アクションを使用して、Workfront API でプルーフを作成できます。このアクションは、値のタイプが `string` の `advancedProofingOptions` パラメーターを受け取ります。`createProof` アクションに詳細プルーフオプションを組み込むには、`advancedProofingOptions` パラメーターに JSON 形式でオプションを入力する必要があります。

>[!NOTE]
>
advancedProofingOptions JSON に含めるフィールドの予測は難しい場合があります。Workfront で詳細プルーフを使用しながら組織のネットワークデータを調べ、組織でよく使用されるフィールドと値に基づいて JSON を設定することもできます。
>
これらのフィールドの予測は難しい場合があるので、Workfront API を使用してプルーフを作成したあと、ProofHQ API を使用してプルーフを更新することをお勧めします。詳しくは、この記事の [Workfront API と ProofHQ API を使用したプルーフの作成（推奨）](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended)を参照してください。

### 例

この例では、`advancedProofingOptions` パラメーターの JSON を作成する際に使用できるフィールドと形式を示しています。`advancedProofingOptions` JSON ファイルに含めるフィールドを、ここで示されているよりも増やしたり、減らしたりできます。

**例：**

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
