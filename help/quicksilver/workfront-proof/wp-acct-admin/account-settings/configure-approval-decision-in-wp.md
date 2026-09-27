---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: '[!DNL Workfront Proof] での承認決定オプションの設定'
description: 組織内の[!DNL Workfront Proof] ユーザーが作成したすべてのプルーフに対して、承認決定オプションを設定できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
TQID: 'https://experienceleague.adobe.com/byd7VyLV7IkwQ1YSHoQMHQNXOPAeJvP8-ENhHBvo01A'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 95%
---
# [!DNL Workfront Proof] での承認決定オプションの設定

>[!IMPORTANT]
>
>この記事では、[!DNL Workfront Proof] スタンドアロン製品の機能について説明します。 [!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

セレクトエディションプランまたはプレミアムエディションプランを使用する [!DNL Workfront Proof] 管理者は、組織内の [!DNL Workfront Proof] ユーザーが作成したすべてのプルーフに対して次の方法で承認決定オプションを設定できます。

* 決定の名前を変更する
* プルーフビューアに表示される決定の順序を変更する
* 表示する決定を決める

この記事では以下について説明します。

## 決定設定の指定

1. 「**[!UICONTROL アカウント設定]**」をクリックします。
1. 「**[!UICONTROL 決定]**」タブを開きます。
1. 次のいずれかの変更を加えます。

   * 決定を非表示にするには、不要な決定の右側にある「**[!UICONTROL 非表示]**」をクリックします。
   * 決定の名前を変更するには、決定名をクリックして編集したあと、ボックスの外側をクリックします（または Enter キーを押します）。 システム内のすべての既存プルーフに関する決定の名前を [!DNL Workfront Proof] が更新します。

     >[!IMPORTANT]
     >
     >名前を変更する際には、決定のロジックは保持します。 例えば、デフォルトの決定「却下」を「新しいバージョンが必要」に変更することはできますが、「プリンターへ送信」には変更しないでください。

     [!DNL Workfront Proof] のデフォルトに戻したい場合は、「デフォルトの決定に戻す」をクリックします。

>[!NOTE]
>
>* 様々なレベルの複数の決定がある場合、プルーフワークフローの全体的なステータスを計算するために、決定の背後にあるロジックが使用されます。
>* 「承認済み」および「変更して承認済み」の決定により、自動ワークフローの次のステージがトリガーされます。
>* 決定の名前を変更し、ロジックを確認したい場合は、左側のナビゲーションパネルで「**[!UICONTROL アクティビティ]**」をクリックし、元の決定が角括弧内に表示されているアクティビティログを確認します。
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## 決定理由の作成

決定理由は、プルーフに関する決定の追加情報を取得するのに役立ちます。

1. **[!UICONTROL 設定]**／**[!UICONTROL アカウント設定]**&#x200B;をクリックします。

1. 「**[!UICONTROL 決定]**」タブを開きます。
デフォルトでは、プルーフに関するすべての意思決定者が理由を使用できますが、それを主な意思決定者のみに制限することもできます。
要件に応じて、複数の理由を選択できるようにすることも、単一の選択リストにすることもできます。 理由を必須にすることもできます。つまり、レビュー担当者はプルーフに関する決定を保存する前に理由を選択する必要があります。
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. 「**[!UICONTROL 理由]**」セクションで、「**[!UICONTROL 新しい理由]**」をクリックします。
   ![New_reason.png](assets/new-reason-350x135.png)

1. **[!UICONTROL 理由]**&#x200B;の下に表示されるテキストボックスに「理由」セクションのタイトルを入力します。
1. テキストボックスを含める場合は、「**[!UICONTROL テキストボックスを含める]**」を選択します。
1. 「**[!UICONTROL 保存]**」をクリックします。
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
   最も重要なステップは、理由を表示する必要がある決定を選択することです。 それを忘れると、その理由はプルーフに表示されなくなります。

1. ページ上部にある決定リストの&#x200B;**[!UICONTROL 理由を表示]**&#x200B;列のチェックボックスをオンにします。 理由に対応する決定を 1 つ以上選択できます。
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## 決定後メッセージの作成

レビュー担当者がプルーフに関する決定を保存した後に表示する決定後メッセージを作成できます。

1. **[!UICONTROL 設定]**／**[!UICONTROL アカウント設定]**&#x200B;をクリックします。

1. 「**[!UICONTROL 決定]**」タブを開きます。
1. 「**[!UICONTROL 決定後メッセージ]**」セクションで、**[!UICONTROL メッセージ]**&#x200B;行の最後にある「**[!UICONTROL 編集]**」をクリックします。
また、メッセージをすべての意思決定者に表示するか、主な意思決定者にのみ表示するかを決定することもできます。
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. **[!UICONTROL メッセージを表示]**&#x200B;列で、このメッセージを表示する決定を指定します。
1 つ以上の決定を選択しない場合、メッセージはプルーフに表示されません。 この列の 1 つ以上のボックスを必ずクリックしてください。
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
