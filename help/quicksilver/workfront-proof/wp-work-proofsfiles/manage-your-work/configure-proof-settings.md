---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: ' [!DNL Workfront Proof] でのプルーフの設定'
description: 配達確認を作成または編集している場合に、配達確認を設定できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 98%

---

# [!DNL Workfront Proof] でのプルーフの設定の指定

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

次のいずれかの方法で、作成中または編集中のプルーフを設定できます。

>[!NOTE]
>
>作成するすべての新規プルーフに対して、これらの設定を指定できます。詳細情報は、以下を参照してください。

## 最終の校正判断が完了したらプルーフをロック

最終承認者が決定したときに、プルーフの状態をロックするように設定できます。これは、レビュアーがプルーフに戻ってコメントを追加したり、決定を変更したりできないようにしたい場合に役立ちます。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフの生成の説明に従って、新規プルーフを作成します。\
   または\
   [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でプルーフの詳細を管理の説明に従って、既存のプルーフのプルーフの詳細ページを開きます。

1. 新規プルーフの場合は、**[!UICONTROL プルーフの設定]**&#x200B;の下の「**[!UICONTROL 必要な校正判断がすべて完了したらプルーフをロック]**」を選択します。\
   または\
   既存のプルーフの場合は、**[!UICONTROL 設定]**&#x200B;の下の「**[!UICONTROL 校正判断がすべて完了したらプルーフをロック]**」を選択します。

校正判断について詳しくは、[プルーフビューアーでプルーフの校正判断を行う](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を参照してください。

## プルーフをレビューするすべてのユーザーに対してログインをリクエスト

[!DNL Workfront Proof] の素晴らしい機能の 1 つは、誰でもプルーフをレビューでき、レビューをするために独自の [!DNL Workfront Proof] を持つ必要がないことです。受信者は、[!DNL Workfront Proof] にログインする必要がなく、個々の URL が記載されたメールが届き、プルーフページに直接移動します。

ただし、レビューおよび承認プロセスに対してより高いレベルのセキュリティが必要な場合は、プルーフへのログインを必須にすることができます。つまり、[!DNL Workfront Proof] ユーザーのみをプルーフに追加できます。また、アクセスする前に、メールとパスワードを入力する必要があります。

>[!NOTE]
>
>* *ユーザーがプルーフにログインするには（ログイン必須が有効な場合）、そのユーザーがプルーフに追加されている必要があります。*
>* *ログイン必須が有効になっている場合、登録を有効にすることはできません。*

プルーフをレビューするすべてのユーザーに対してログインを必須にするには、次の手順に従います。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフの生成の説明に従って、新規プルーフを作成します。\
   または\
   [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でプルーフの詳細を管理の説明に従って、既存のプルーフに関するプルーフの詳細ページを開きます。

1. 新規プルーフの場合は、**[!UICONTROL プルーフの設定]**&#x200B;の下の「**[!UICONTROL ログインを必須にする]**」を選択します。\
   または\
   既存のプルーフの場合は、**[!UICONTROL 設定]**&#x200B;の下の「**[!UICONTROL ログインを必須にする]**」を選択します。

## プルーフに必要な校正判断を 1 つにする

この設定は、プルーフの校正判断に対して、グループ、部門または会社の 1 人のユーザーのみを必要とする場合に役立ちます。

承認者またはレビュアーおよび承認者の役割を複数のユーザーに割り当てた場合でも、1 人のユーザーがプルーフに対する校正判断を行うと、（その校正判断に従って）プルーフのステータスが更新されます。プルーフのステータスについて詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md) でのプルーフの進捗とステータスの表示を参照してください。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフの生成の説明に従って、新規プルーフを作成します。\
   または\
   [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でプルーフの詳細の管理の説明に従って、既存のプルーフのプルーフの詳細ページを開きます。

1. 新規プルーフの場合は、**[!UICONTROL ワークフロー]**&#x200B;の下の「**[!UICONTROL このステージに必要な校正判断を 1 つにする]**」を選択します。\
   または\
   既存のプルーフの場合は、**[!UICONTROL 設定]**&#x200B;の下の「**[!UICONTROL 必要な校正判断を 1 つにする]**」を選択します。

校正判断について詳しくは、[プルーフビューアーでプルーフの校正判断を行う](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof)を参照してください。

## 校正判断に電子サインを必須にする

プルーフで校正判断をするレビュアーに対して、メールとパスワードの入力して、電子署名する必要があります。レビュアーが校正判断をする場合、メールとパスワードの入力および校正判断の確認を求めるプロンプトが表示されます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md) での電子署名についてを参照してください。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフの生成の説明に従って、新規プルーフを作成します。\
   または\
   [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でのプルーフの詳細の管理の説明に従って、既存のプルーフのプルーフの詳細ページを開きます。

1. 新規プルーフの場合は、**[!UICONTROL プルーフの設定]**&#x200B;の下の「**[!UICONTROL 校正判断に電子サインを必須にする]**」を選択します。\
   または\
   既存のプルーフの場合は、**[!UICONTROL 設定]**&#x200B;の下の「**[!UICONTROL 校正判断に電子サインを必須にする]**」を選択します。

校正判断について詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md) での承認決定オプションの設定を参照してください。

## 元のファイルのダウンロードをユーザーに許可しない

プルーフのレビュアーが、プルーフの作成元のファイルをダウンロードしないようにすることができます。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフの生成の説明に従って、新規プルーフを作成します。\
   または\
   [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でプルーフの詳細を管理の説明に従って、既存のプルーフのプルーフの詳細ページを開きます。

1. 新規プルーフの場合は、**[!UICONTROL プルーフの設定]**&#x200B;の下の「**[!UICONTROL オリジナルファイルをダウンロード]**」の選択を解除します。\
   または\
   既存のプルーフの場合は、**[!UICONTROL 設定]**&#x200B;の下の「**[!UICONTROL オリジナルファイルをダウンロード]**」を選択します。

## 他のユーザーによるプルーフの購読を許可

購読は、プルーフの URL とミニプルーフで機能する詳細設定です。

デフォルトでは、プルーフに特に追加されておらず、プルーフ URL またはミニプルーフを使用してアクセスしているユーザーは、プルーフを読み取り専用モードでのみ表示できます。既にプルーフのレビュアーであるユーザーは、自分のメールアドレスを使用してログインできます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)でのプルーフの役割を管理を参照してください。

プルーフの登録を有効にすると、プルーフに明示的に追加されていないユーザーが、自分自身をプルーフに登録できるようになります（つまり、プルーフに自分自身を追加できるようになります）。その後、登録の設定で選択した役割とメールアドレスのアラートが割り当てられます。

プルーフで「登録」が有効になっている場合、次のフィールドがアクティブになります。

* **[!UICONTROL サブスクライバーの検証が必要です]** - プルーフにアクセスするには、サブスクライバーがメール内のリンクをクリックする必要があります\
   このオプションを選択すると、購読しているユーザーは即座にプルーフにアクセスすることがスできなくなりますが、メールでプルーフへのリンクを取得します。サブスクライバー認証の目的は、ユーザーが正しい、アクセス権を持つメールアドレスを入力したと確認することです。

* **[!UICONTROL 新規サブスクライバーのデフォルトの役割]** - これは、プルーフを登録するすべてのレビュアーに割り当てられるデフォルトのプルーフの役割です。
* **[!UICONTROL 新規サブスクライバー向けのデフォルトのメールアラート]** - これは、プルーフを自分で登録するすべてのレビュアーに割り当てられるデフォルトのメールアラートです。

[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md) でプルーフを登録を参照してください。

他のユーザーにプルーフの登録を許可するには、以下のように行います。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)でプルーフを生成の説明に従って、プルーフを新規作成します。\
   または\
   [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でプルーフの詳細を管理の説明に従って、既存のプルーフのプルーフの詳細ページを開きます。

1. 新規プルーフの場合は、**[!UICONTROL プルーフ設定]**&#x200B;の下の「**[!UICONTROL パブリック URL か埋め込みコードからプルーフに参加]**」の選択を解除します。\
   または\
   既存のプルーフの場合は、**[!UICONTROL 設定]**&#x200B;の下の「**[!UICONTROL 購読]**」を選択します。
