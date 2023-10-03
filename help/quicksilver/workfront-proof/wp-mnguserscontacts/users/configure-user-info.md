---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 次を使用してユーザー情報を設定 [!DNL Workfront Proof]
description: 次を使用してユーザー情報を設定 [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 次を使用してユーザー情報を設定 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

1. ユーザーの作成または編集を開始します ( [次を使用してユーザーを作成 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. 次の情報を指定します。

   * Adobe Analytics の **[!UICONTROL 個人の詳細]** セクション：

      * **電子メールアドレス：** ユーザーの電子メールアドレス。
      * **名：** ユーザーの名。
      * **姓：** ユーザーの姓。
      * **位置：** 会社内でのユーザーの位置。
      * **権限プロファイル：** 配達確認アカウントに対するユーザーの権限です。
      * **言語：** ユーザーの主要言語。
      * **タイムゾーン：** ユーザーのタイムゾーンを選択します。
      * **日付の形式：** ユーザーが希望する日付形式を選択します。
      * **オプトイン — 製品およびマーケティング用電子メール：** 製品およびマーケティング用の E メールでユーザーをオプトインするかどうかを選択します。
      * **API のみ：** ユーザーが API 経由でのみログインできるようにします。

   * Adobe Analytics の **[!UICONTROL ユーザーの詳細]** [ ] セクションで、住所や電話番号など、ユーザの連絡先情報を入力します。
   * Adobe Analytics の **[!UICONTROL デフォルトの配達確認設定]** 「 」セクションでは、ユーザーによる配達確認の作成方法や作業方法に影響する設定を指定します。

      * **デフォルトの配達確認の役割：** ユーザーのデフォルトの配達確認の役割を選択します。 役割のオプションは次のとおりです。 **[!UICONTROL 読み取り専用]**, **[!UICONTROL レビュー担当者]**, **[!UICONTROL 承認者]**, **[!UICONTROL レビュー担当者と承認者]**, **[!UICONTROL 作成者]**&#x200B;または **[!UICONTROL モデレーター]**.

        配達確認の役割について詳しくは、 [での配達確認の役割の管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **すべての決定がおこなわれたら、配達確認をロックします。** 配達確認に対するすべての決定がおこなわれた後、それ以上の変更から配達確認を自動的にロックします。
      * **ログインが必要です。 配達確認は、他のユーザーとのみ共有できます。** を持つユーザーのみが配達確認を使用できるようにします。 [!DNL Workfront Proof] ログイン資格情報。
      * **必要な決定は 1 つだけです。** 配達確認に対する決定を 1 つだけ必要とします。
      * **元のファイルのダウンロード：** 配達確認用に元のファイルをダウンロードできるようにします。 このオプションは、デフォルトで有効になっています。

        元のファイルのダウンロードについて詳しくは、 [に保存されているファイルをダウンロード [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **登録. 担当者は、公開 URL または埋め込みコードを使用して、配達確認にサインアップできます。** 組織外のレビュー担当者が公開 URL で配達確認にサインアップしたり、埋め込みコードを使用したりできるようにします。

        このオプションを選択した場合、 **配達確認にアクセスするには、購読者が E メール内のリンクをクリックする必要があります** はも利用できます。 外部のレビュー担当者が E メール内のリンクをクリックして配達確認にアクセスするように求める場合に、このオプションを選択します。
このオプションは、 **公開共有** 」オプションが選択されている。

      * **新規ゲストレビュー担当者のデフォルトの役割：** ゲストレビュー担当者用のデフォルトの配達確認の役割を選択します。 オプションは、 **デフォルトの配達確認の役割**（モデレーターと作成者を除く）

   * Adobe Analytics の **[!UICONTROL デフォルトのメールアラート設定]** セクション：

      * **デフォルトの電子メールアラート：** ユーザーが電子メールの更新を受け取る頻度を選択します。 選択 **すべてのアクティビティ、自分のコメントに返信、決定、最終決定、時間別概要、日別概要** または **無効**.

        デフォルトの電子メールアラートオプションの詳細については、 [での電子メール通知の設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **新規ゲストレビュー担当者向けのデフォルトの電子メールアラート：** ゲストレビュー担当者が電子メールの更新を受け取る頻度を選択します。 オプションは、 **デフォルトの電子メールアラート。**

      * **配達確認の準備が整ったら E メールを送信します。** 配達確認の準備が整ったら、確認 E メールをユーザーに自動的に送信する場合に選択します。
      * **このユーザーに送信される E メールの形式：** 選択 **[!UICONTROL HTML]** または **[!UICONTROL プレーンテキスト]** を使用します。

   * Adobe Analytics の **[!UICONTROL カスタムメッセージ設定]** 「 」セクション：配達確認テンプレートの設定を作成します。

     テンプレートについて詳しくは、次を参照してください。

      * **配達確認の件名テンプレート：** 配達確認の件名のテンプレートを作成します。
      * **配達確認メッセージテンプレート：** 配達確認メッセージのテンプレートとその形式を作成します。
