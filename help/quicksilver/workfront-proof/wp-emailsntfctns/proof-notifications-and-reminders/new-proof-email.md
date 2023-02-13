---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 新しい配達確認 E メール
description: この記事を PiW 向けにより良く機能させます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 新しい配達確認 E メール

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

新しい配達確認または新しいバージョンの配達確認を作成する場合、配達確認に新しい人を追加する場合、または配達確認にワークフローを追加する場合、レビュー担当者に E メールを送信するかどうかを次の記事で説明するように指定できます。

* [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

受信者が受け取る E メールは、 [!UICONTROL 新しい配達確認] 電子メール。 この E メールを制御できるのは、配達確認の作成者と、配達確認にレビュー担当者を追加する権限を持つユーザーだけです。 受信者は無効にできません。

新しい配達確認 E メールには、次の内容が含まれます。

* 個人メッセージ（メッセージを含める場合）
* 常に同じカスタムメッセージをレビュー担当者に送信する場合は、レビュー担当者に保存することをお勧めします [!UICONTROL 個人設定] の下に [!UICONTROL 校正の既定値] タブをクリックします。 詳しくは、を参照してください。
* 配達確認への個人リンク
* **[!UICONTROL 詳細を表示]** 関連する [!DNL Workfront] オブジェクト（プロジェクト、タスク、イシューなど）
* 配達確認画像のサムネール
* 次の配達確認の詳細：

   * プルーフ名
   * バージョン番号

      詳しくは、を参照してください。

   * レビュー担当者と配達確認の進行状況のリスト
   * 他のユーザーと配達確認を共有するためのリンク

      これにより、元のファイルの配達確認 URL やダウンロードリンクを共有できます。 これにより、校閲者を明示的に配達確認に追加することはできず、公開配達確認 URL のみ共有され、受信者は配達確認への読み取り専用アクセス権を受け取ります。

      詳しくは、 [で配達確認を共有 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) を参照してください。

      このリンクを受信者の E メールに表示したくない場合は、 [!UICONTROL 公開共有] 配達確認の設定

      （元のファイルとパブリック URL をダウンロード）。 詳しくは、 [で配達確認の詳細を管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) を参照してください。

## アクティビティログ

の送信 [!UICONTROL 新しい配達確認] レビュー担当者への電子メールが [!UICONTROL アクティビティ] セクション [!UICONTROL 配達確認の詳細] ページ。 詳しくは、  [管理[!UICONTROL  配達確認の詳細] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) を参照してください。 次の項目を確認できます。 [!UICONTROL 新しい配達確認] 配達確認の作成時に電子メールが有効になっていました。

![New_Verson_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* 配達確認の作成者または所有者が [!UICONTROL 作成された配達確認] （個人設定で）デフォルトで無効になっているメールは、何も受信されません [!UICONTROL 作成された配達確認] または [!UICONTROL 新しい配達確認] たとえ [!UICONTROL メールで担当者に通知] 」ボックスが新しい配達確認ページでオンになっている。 詳しくは、を参照してください。
>* 電子メール通知がデフォルトで [!UICONTROL アカウント設定] 配達確認の作成者/所有者は、 [!UICONTROL 作成された配達確認] または [!UICONTROL 新しい配達確認] これが個人設定で有効になっていても、メールは [!UICONTROL 通知] 「新しい配達確認」ページで「 E メール別の担当者」ボックスがオンになっている。 詳しくは、 [この [!UICONTROL 作成された配達確認] 電子メール](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) およびを参照してください。
>




## を有効にします。 [!UICONTROL 新しい配達確認] 電子メールを送信し、カスタムメッセージを含める

配達確認の作成時にレビュー担当者に電子メールアラートを送信するか、配達確認に人を追加する際に送信するかを指定できます。

* [配達確認を作成する際](#when-you-create-a-proof)
* [配達確認にレビュー担当者を追加する場合](#when-you-add-a-reviewer-to-a-proof)

### 配達確認を作成する際 {#when-you-create-a-proof}

新しい配達確認を [!UICONTROL 新しい配達確認] ページの **[!UICONTROL 共有]** 「 」セクションでは、E メールアラートを送信するかどうかを選択できます。

* ここで、 [!UICONTROL メールで担当者に通知] (1) このオプションを選択解除した場合、校正がレビューの準備ができたことを知らせる E メールをレビュー担当者は誰も受け取りません。
* また、電子メール通知にカスタムメッセージを含めることもできます (2)。
* 独自のカスタムメッセージを追加する場合は、カスタマイズした件名行 (3) とメール本文 (4) にメッセージを入れることができます。
* カスタムメッセージを破棄するには、リンクをクリックするだけです (5)。

   >[!NOTE]
   >
   >常に同じカスタムメッセージをレビュー担当者に送信する場合は、レビュー担当者に対して、 [!UICONTROL 校正の既定値] タブをクリックします。 詳しくは、を参照してください。

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### 配達確認にレビュー担当者を追加する場合 {#when-you-add-a-reviewer-to-a-proof}

（上記と同様に）既存の配達確認に追加された新しいレビュー担当者に、配達確認の通知を送信するかどうかを選択できます。

* まず、新しいレビュー担当者を追加するには、 **[!UICONTROL このバージョンを共有]** ボタン **[!UICONTROL 配達確認の詳細]** ページ (1) を参照してください。

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* 新しいレビュー担当者を追加できるボックスが表示されます。 その後、電子メールで通知を受け取るかどうかを決定し (2)、電子メールにカスタムメッセージを追加するかを選択できます (3)。

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* カスタムメッセージを追加する場合は、ボックスが展開し、カスタム件名行 (4) とカスタムテキストを E メールの本文 (5) に入れることができます。 また、リンク (6) をクリックしてカスタムメッセージを破棄することもできます。

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
