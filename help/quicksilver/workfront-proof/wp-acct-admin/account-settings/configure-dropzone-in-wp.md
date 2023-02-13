---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: でのドロップゾーンの設定 [!DNL Workfront Proof]
description: As a [!DNL Workfront Proof] 管理者は、ユーザーのドロップゾーン設定の設定、表示、編集をおこなうことができます。 ドロップゾーンについて詳しくは、「ドロップゾーン」を参照してください。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# でのドロップゾーンの設定 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] 管理者は、ユーザーのドロップゾーン設定の設定、表示、編集をおこなうことができます。 ドロップゾーンについて詳しくは、 [ドロップゾーン](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL アカウント設定]**&#x200B;をクリックし、 **[!UICONTROL ドロップゾーン]** タブをクリックします。

1. 次の変更を **[!UICONTROL ドロップゾーンの詳細]** セクション：

   * **[!UICONTROL Web ドロップゾーン]**:ドロップゾーンを有効または無効にします。
   * **[!UICONTROL Web ドロップゾーン URL]**:ドロップゾーン経由で配達確認を送信するためにブラウザーに入力する必要がある URL です。
   * **[!UICONTROL メールドロップゾーン]**:電子メールドロップゾーンを有効または無効にします。

      >[!NOTE]
      >
      >ドロップゾーンへの電子メールの送信はサポートされなくなりました。

   * **[!UICONTROL ドロップゾーン所有者]**:ドロップゾーンの所有者を設定または編集します。 これは、ドロップゾーンへの新しい送信を通知される人です。 ドロップゾーン所有者に設定するには、スーパーバイザー、管理者、請求管理者、またはアカウント作成者である必要があります。 詳しくは、 [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL 作成者のデフォルトの役割]**:すべての送信者が、この役割がデフォルトとして配達確認に追加されます。
   * **[!UICONTROL すべての作成者に関する電子メール通知]**:配達確認作成者（送信者）向けの E メールアラートの設定をここに設定します。 詳しくは、 [での電子メール通知の設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) 使用可能な様々なアラート設定の詳細

   * **[!UICONTROL 新しいバージョン関数]**:ドロップゾーンで「新しいバージョン」機能を有効または無効にします。 これにより、ユーザーがドロップゾーンを使用して新しいバージョンの配達確認を送信する機能を追加または削除できます。
   * **[!UICONTROL 次の日数後に下書き配達確認を削除]**:ドラフト配達確認を削除するまでの日数を指定します。 ファイルをドロップゾーンにアップロードした後にドロップゾーンの送信が完了しない場合、配達確認はドラフト状態のままです。
   * **[!UICONTROL レビュー担当者の役割を非表示にする]**:ドロップゾーンに人を追加する際に、レビュー担当者の役割フィールドを非表示にします。
   * **[!UICONTROL 有効化時に配達確認メッセージを送信]**:設定 [!DNL Workfront Proof] 配達確認が有効化されたときに、レビュー担当者に配達確認通知 E メールを自動的に送信する場合。
   * **[!UICONTROL 送信時に配達確認を有効化]**:設定 [!DNL Workfront Proof] ：送信時に配達確認を自動的に有効化する場合（手動で有効化する必要はありません）。

   * 配達確認がドロップゾーンから（例えば、アカウント内の別のフォルダーに）移動された場合、ドロップゾーン設定は配達確認に適用されなくなります。 これは、E メールアラート設定に関して特に重要です。

1. 変更を **[!UICONTROL ドロップゾーンフィールド]** セクションを使用して、 [!UICONTROL 配達確認の詳細] 」セクションに表示されます。
1. 内 **[!UICONTROL 許可されているドメイン]** 「 」セクションで、ドロップゾーンの使用を許可するドメインを指定します。

   * 次をクリックできます。 **[!UICONTROL ドメインを追加]** をクリックしてドメインを追加します。 ドメインの詳細の追加が完了したら、 **[!UICONTROL 保存]**.

   * 以下が可能です。 **[!UICONTROL 編集]** および **[!UICONTROL 削除]** 以前に追加した既存のドメイン。

1. の下 **[!UICONTROL 通知する担当者]**、新しい配達確認がドロップゾーンに送信されたときにドロップゾーンの所有者と共に通知を受け取る人を指定します [ドロップゾーン](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * クリック **[!UICONTROL 担当者を追加]**&#x200B;受信者の詳細を入力し、「 **[!UICONTROL 保存]**.

   * **[!UICONTROL 削除]** 以前に追加した担当者。
