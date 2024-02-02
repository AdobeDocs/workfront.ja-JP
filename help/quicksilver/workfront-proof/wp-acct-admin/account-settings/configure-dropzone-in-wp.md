---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: ' [!DNL Workfront Proof] にドロップゾーンを設定する'
description: ' [!DNL Workfront Proof]  管理者は、ユーザーのドロップゾーン設定の設定、表示、編集を行うことができます。ドロップゾーンについて詳しくは、ドロップゾーンを参照してください。'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: ht
source-wordcount: '498'
ht-degree: 100%

---

# [!DNL Workfront Proof] でのドロップゾーンの設定

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

[!DNL Workfront Proof] 管理者は、ユーザーのドロップゾーン設定の設定、表示、編集を行うことができます。ドロップゾーンについて詳しくは、[ドロップゾーン](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)を参照してください。

1. **[!UICONTROL 設定]**／**[!UICONTROL アカウント設定]**&#x200B;をクリックし、「**[!UICONTROL ドロップゾーン]**」タブを開きます。

1. **[!UICONTROL ドロップゾーンの詳細]**&#x200B;セクションで次のいずれかの変更を加えます。

   * **[!UICONTROL Web ドロップゾーン]**：ドロップゾーンを有効または無効にします。
   * **[!UICONTROL Web ドロップゾーン URL]**：ドロップゾーン経由でプルーフを送信するためにブラウザーに入力する必要がある URL。
   * **[!UICONTROL メールドロップゾーン]**：メールドロップゾーンを有効または無効にします。

     >[!NOTE]
     >
     >ドロップゾーンへのメールの送信はサポートされなくなりました。

   * **[!UICONTROL ドロップゾーン所有者]**：ドロップゾーン所有者を設定または編集します。これは、ドロップゾーンへの新しい送信の通知を受け取る人です。ドロップゾーン所有者に設定するには、スーパーバイザー、管理者、請求管理者、またはアカウント作成者である必要があります。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) のプルーフ権限プロファイルを参照してください。

   * **[!UICONTROL 作成者のデフォルトの役割]**：すべての送信者は、デフォルトでこの役割を含めてプルーフに追加されます。
   * **[!UICONTROL すべての作成者に関するメール通知]**：プルーフ作成者（送信者）向けのメールアラートの環境設定をここに行います。使用可能な様々なアラート設定について詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) でのメール通知の設定を参照してください。

   * **[!UICONTROL 新しいバージョン関数]**：ドロップゾーンで新しいバージョン関数を有効または無効にします。これにより、ユーザーがドロップゾーンを使用して新しいバージョンのプルーフを送信する機能を追加または削除できます。
   * **[!UICONTROL 指定の日数後にドラフトのプルーフを削除]**：ドラフトのプルーフが削除されてからの日数を指定します。ファイルをドロップゾーンにアップロードした後にドロップゾーンの送信が完了しない場合、プルーフはドラフト状態のままです。
   * **[!UICONTROL レビュアーの役割を非表示にする]**：ドロップゾーンにユーザーを追加する際に、「レビュアーの役割」フィールドを非表示にします。
   * **[!UICONTROL アクティブ化時にプルーフメッセージを送信]**：プルーフのアクティブ化時に、レビュアーにプルーフ通知メールを自動的に送信するように [!DNL Workfront Proof] を設定します。
   * **[!UICONTROL 送信時にプルーフをアクティブ化]**：送信時にプルーフを自動的にアクティブ化するように、[!DNL Workfront Proof] を設定します（手動でアクティブ化する必要はありません）。

   * プルーフがドロップゾーンから（例えば、アカウント内の別のフォルダーに）移動された場合、ドロップゾーン設定はプルーフに適用されなくなります。これは、メールアラートの設定に関して特に重要です。

1. 「**[!UICONTROL ドロップゾーンフィールド]**」セクションを変更して、ドロップゾーン経由でプルーフを送信するときに、ドロップゾーン送信ページの「[!UICONTROL プルーフの詳細]」セクションに表示するフィールドを指定します。
1. 「**[!UICONTROL 許可されているドメイン]**」セクションで、ドロップゾーンの使用を許可するドメインを指定します。

   * 「**[!UICONTROL ドメインを追加]**」をクリックしてドメインを追加します。ドメインの詳細の追加が完了したら、「**[!UICONTROL 保存]**」をクリックします。

   * 以前に追加した既存のドメインは&#x200B;**[!UICONTROL 編集]**&#x200B;および&#x200B;**[!UICONTROL 削除]**&#x200B;できます。

1. **[!UICONTROL 通知するユーザー]**&#x200B;で、新しいプルーフが[ドロップゾーン](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)に送信されたときに、ドロップゾーンの所有者とともに通知を受け取りたいユーザーを指定します。

   * 「**[!UICONTROL ユーザーを追加]**」をクリックし、受信者の詳細を入力して、「**[!UICONTROL 保存]**」をクリックします。

   * 以前に追加したユーザーを&#x200B;**[!UICONTROL 削除]**&#x200B;します。
