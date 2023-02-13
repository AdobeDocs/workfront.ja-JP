---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 配達確認が E メールを送信しました
description: 配達確認作成者の E メールは、配達確認を作成した場合にのみ配達確認の作成者に送信されます。 人物が配達確認を作成し、別の人物を所有者にした場合、新しい所有者のみが配達確認の E メールを受け取ります。 作成者または所有者は、これを取得しません。配達確認作成済みの E メールのみを受け取ります。 新しい配達確認 E メールについて詳しくは、「新しい配達確認 E メール」を参照してください。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# この [!UICONTROL 作成された配達確認] 電子メール

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

A [!UICONTROL 作成された配達確認] 配達確認を作成した場合にのみ、配達確認の作成者に電子メールが送信されます。 人物が配達確認を作成し、別の人物を所有者にした場合、新しい所有者のみがこの [!UICONTROL 作成された配達確認] 電子メール。 作成者または所有者は、これを取得しません。彼らは受け取るのは [!UICONTROL 作成された配達確認] 電子メール。 詳しくは、 [!UICONTROL 新しい配達確認] 電子メール： [[!UICONTROL 新しい配達確認] 電子メール](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

ユーザーは無効にできます [!UICONTROL 作成された配達確認] 以下に説明するように、電子メールをプロファイル設定で送信できます。

>[!NOTE]
>
> 配達確認の作成者または所有者が [!UICONTROL 作成された配達確認] デフォルトで無効になっているメールは、個人設定で受信されません [!UICONTROL 作成された配達確認] または [!UICONTROL 新しい配達確認] 電子メール ( [!UICONTROL メールで担当者に通知] 」ボックスがオンになっている場合、 [!UICONTROL 新しい配達確認] ページ。

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

A [!UICONTROL 作成された配達確認] 電子メールには、個人用メッセージ（メッセージを含む場合）と次の配達確認の詳細が含まれます。

* プルーフ名
* 配達確認への個人リンク
* バージョン番号
* 配達確認のサムネール
* プルーフの進捗状態
* 他のユーザーと配達確認を共有するためのリンク
* これにより、元のファイルの配達確認 URL やダウンロードリンクを共有できます。

>[!NOTE]
>
> 配達確認リンクを共有すると、レビュー担当者を配達確認に明示的に追加できず、公開配達確認 URL のみ共有され、受信者は配達確認への読み取り専用アクセス権を受け取ります。

詳しくは、 [で配達確認を共有 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) を参照してください。

このリンクを受信者の E メールに表示したくない場合は、 [!UICONTROL 公開共有] 配達確認の設定 ([!UICONTROL 元のファイルをダウンロード] および [!UICONTROL パブリック URL]) をクリックします。

## の無効化 [!UICONTROL 作成された配達確認] 電子メール

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**、 **[!UICONTROL 校正の既定値]** 「 」タブで、「 **[!UICONTROL 無効にする]** 次の **[!UICONTROL 配達確認の準備が整ったら確認の電子メールを送信]**.

1. ![Proof_Made_-_proofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. 詳しくは、 [Workfront Proof での電子メール通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) を参照してください。
1. 電子メール通知がデフォルトで [!UICONTROL アカウント設定]に設定されている場合、配達確認の作成者または所有者には [!UICONTROL 作成された配達確認] または [!UICONTROL 新しい配達確認] 電子メール（個人設定で有効になっている場合も含む） [!UICONTROL メールで担当者に通知] 」ボックスがオンになっている場合、 [!UICONTROL 新しい配達確認] ページ。
