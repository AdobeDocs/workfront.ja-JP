---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Workfront Proof の配達確認の状態を理解する
description: In [!DNL Workfront Proof]、配達確認は異なる状態で存在します。 これらの状態によって、コメントの作成や決定など、配達確認に対して実行できるアクションが決まります。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Workfront Proof の配達確認の状態を理解する

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

In [!DNL Workfront Proof]、配達確認は異なる状態で存在します。 これらの状態によって、コメントの作成や決定など、配達確認に対して実行できるアクションが決まります。

## 配達確認の状態について

4 つの状態は次のとおりです。

* [アクティブ](#active)
* [ロック済み](#locked)
* [ドラフト（ドロップゾーンのみ）](#draft-dropzone-only)
* [送信済み（ドロップゾーンのみ）](#submitted-dropzone-only)

### アクティブ {#active}

にアップロードされた配達確認 [!DNL Workfront Proof] 新しい配達確認ページまたはドロップゾーンは、処理後、「アクティブ」と表示されます。 配達確認がアクティブな場合、ユーザーは確認、コメントを作成し、配達確認に関する決定をおこなうことができます。

>[!NOTE]
>
>ドロップゾーンを通じてアップロードされた配達確認は、「送信時に配達確認を有効にする」オプションが有効な場合にのみ、「アクティブ」として表示されます。 このオプションが有効になっていない場合は、配達確認を手動で有効にする必要があります。

ドロップゾーンの設定について詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### ロック済み {#locked}

配達確認のレビューが終了したら、配達確認をロックできます。 配達確認をロックすると、配達確認に対するコメントや決定をそれ以上実行できなくなりますが、配達確認を開くことはできます。

配達確認の編集権限を持つユーザーであれば、誰でもロックを解除できます。

権限について詳しくは、 [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>配達確認がロックされたときに電子メール通知が送信されなくなりました。 例えば、配達確認が期限より前にロックされている場合、期限を過ぎると通知 E メールは送信されません。

### ドラフト（ドロップゾーンのみ） {#draft-dropzone-only}

ドロップゾーンから配達確認を送信すると、管理者がアクティブ化する前にドラフト状態になります。 ドラフトゾーンの場合は、配達確認に対して何のアクションも実行できません。

### 送信済み（ドロップゾーンのみ） {#submitted-dropzone-only}

管理者がドラフトを有効にすると、配達確認がドロップゾーンに「送信済み」と表示されます。 送信後、配達確認に対してアクションを実行できます。

## 配達確認の状態の表示と変更

特定の状態でのすべての配達確認のリストの表示（すべてのアクティブな配達確認またはロックされた配達確認の表示など）について詳しくは、 [のビューページで項目を管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 記事内 [のビューページで項目を管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 次にアクセス： [!DNL Workfront Proof] ダッシュボード。

   詳しくは、 [アクセス [!DNL Workfront Proof] Adobe Workfrontから](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. の **[!UICONTROL ダッシュボード]**、 **[!UICONTROL 展開]** 状態を表示または変更する配達確認の横の矢印。

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   この **[!UICONTROL ワークフロープロセス]** セクションが表示されます。

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. 次を表示： **[!UICONTROL 都道府県]** 内 **[!UICONTROL ワークフロープロセス]**.

1. （オプション）状態を変更するには、現在の **[!UICONTROL 都道府県]** をクリックし、ドロップダウンメニューをクリックして、新しい状態を選択します。

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
