---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: での承認決定オプションの設定 [!DNL Workfront Proof]
description: で作成されるすべての配達確認に対して、承認の決定オプションを設定できます [!DNL Workfront Proof] 組織内のユーザー。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# での承認決定オプションの設定 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] 管理者は、エディションプランを選択またはプレミアムを使用して、次の方法で、 [!DNL Workfront Proof] 組織内のユーザー：

* 決定の名前を変更
* 校正ビューアに表示される決定の順序を変更する
* 表示する決定を決定する

この記事では、次の点について説明します。

## 決定の設定

1. クリック **[!UICONTROL アカウント設定]**.
1. を開きます。 **[!UICONTROL 決定]** タブをクリックします。
1. 次の変更を行います。

   * 決定を非表示にするには、 **[!UICONTROL 非表示]** を選択します。
   * 決定の名前を変更するには、決定名をクリックして編集し、ボックスの外側をクリックします（または Enter キーを押します）。 [!DNL Workfront Proof] は、システム内の既存のすべての配達確認に関する決定の名前を更新します。

     >[!IMPORTANT]
     >
     >決定のロジックは、名前を変更する際に保持します。 例えば、デフォルトの決定「却下」を「新しいバージョンが必要」に変更することはできますが、「プリンターに送信」に変更しないでください )。

     次のページに戻りたい場合： [!DNL Workfront Proof] デフォルト値に設定する場合は、「デフォルトの決定を復元」をクリックできます。

>[!NOTE]
>
>* 決定の背後にあるロジックは、様々なレベルの複数の決定がある場合に、配達確認ワークフローの全体的なステータスを計算するために使用されます。
>* 自動ワークフローの次の段階で、「承認済み」および「変更により承認済み」のトリガーが表示されます。
>* 決定の名前を変更し、ロジックを検証する場合は、「 **[!UICONTROL アクティビティ]** 左側のナビゲーションパネルで、元の決定が括弧で囲まれて表示されるアクティビティログを確認します。
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## 決定理由の作成

判定の理由は、配達確認に関する追加の判定情報を取得する良い方法です。

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL アカウント設定]**.

1. を開きます。 **[!UICONTROL 決定]** タブをクリックします。
デフォルトでは、理由は配達確認に関するすべての意思決定者に提供されますが、プライマリの意思決定者にのみ制限できます。
要件に応じて、複数の理由を選択できます。また、単一の選択リストにすることもできます。 また、理由を必須にすることもできます。これは、レビュー担当者が配達確認に対する決定を保存する前に、理由を選択する必要があることを意味します。
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. Adobe Analytics の **[!UICONTROL 理由]** セクションで、 **[!UICONTROL 新しい理由]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. の下に表示されるボックスに理由セクションのタイトルを入力します。 **[!UICONTROL 理由]**.
1. テキストボックスを含める場合は、 **[!UICONTROL 「含める」テキストボックス]**.
1. 「**[!UICONTROL 保存]**」をクリックします。
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
最も重要な手順は、理由を表示する必要がある決定を選択することです。 それを忘れた場合、理由は配達確認に表示されません。

1. 次の項目のチェックボックスをオンにします。 **[!UICONTROL 理由を表示]** 」列がページ上部の決定リストに表示されます。 理由に応じて、1 つ以上の決定を選択できます。
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## 決定後メッセージの作成

レビュー担当者が配達確認に対する決定を保存した後に表示する、決定後のメッセージを作成できます。

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL アカウント設定]**.

1. を開きます。 **[!UICONTROL 決定]** タブをクリックします。
1. Adobe Analytics の **[!UICONTROL 決定メッセージを投稿]** セクションで、 **[!UICONTROL 編集]** ～の終わりに **[!UICONTROL メッセージ]** 行。
メッセージをすべての意思決定者に表示するか、メッセージの意思決定者に制限するかを決定することもできます。
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. Adobe Analytics の **[!UICONTROL メッセージを表示]** 列に、このメッセージを表示する決定を指定します。
1 つ以上の決定を選択しない場合、配達確認にメッセージは表示されません。 この列で、少なくとも 1 つのボックスをオンにしてください。
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
