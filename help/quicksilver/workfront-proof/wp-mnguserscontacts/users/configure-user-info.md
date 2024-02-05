---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: ' [!DNL Workfront Proof] を使用してユーザー情報を設定'
description: ' [!DNL Workfront Proof] を使用してユーザー情報を設定'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 96%

---

# [!DNL Workfront Proof] を使用してユーザー情報を設定

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md) を使用してユーザーを作成で説明されているように、ユーザーの作成または編集を開始します。
1. 次の情報を指定します。

   * 「**[!UICONTROL 個人の詳細]**」セクション：

      * **メールアドレス：**&#x200B;ユーザーのメールアドレス。
      * **名：**&#x200B;ユーザーの名。
      * **姓：**&#x200B;ユーザーの姓。
      * **位置：**&#x200B;会社内でのユーザーの位置。
      * **権限プロファイル：**&#x200B;プルーフアカウントにおけるユーザーの権限。
      * **言語：**&#x200B;ユーザーの主要言語。
      * **タイムゾーン：**&#x200B;ユーザーのタイムゾーンを選択します。
      * **日付の形式：**&#x200B;ユーザーが希望する日付形式を選択します。
      * **オプトイン - 製品およびマーケティング用のメール：**&#x200B;製品およびマーケティング用のメールでユーザーをオプトインするかどうかを選択します。
      * **API のみ：**&#x200B;ユーザーが API 経由でのみログインできるようにします。

   * 「**[!UICONTROL ユーザーの詳細]**」セクションでは、住所や電話番号など、ユーザーの連絡先情報を入力します。
   * 「**[!UICONTROL デフォルトのプルーフ設定]**」セクションでは、ユーザーによるプルーフの作成方法や作業方法に影響する設定を行います。

      * **デフォルトのプルーフの役割：**&#x200B;ユーザーのデフォルトのプルーフの役割を選択します。役割のオプションは次のとおりです。**[!UICONTROL 読み取り専用]**、**[!UICONTROL レビュアー]**、**[!UICONTROL 承認者]**、**[!UICONTROL レビュアーと承認者]**、**[!UICONTROL 作成者]**、または&#x200B;**[!UICONTROL モデレーター]**。

        プルーフの役割について詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) のプルーフの役割の管理を参照してください。

      * **すべての決定が行われたら、プルーフをロック：**&#x200B;プルーフに対するすべての決定が行われた後、プルーフがそれ以上変更されないように自動的にロックします。
      * **ログインが必要です。プルーフは他のユーザーとのみ共有可能：**[!DNL Workfront Proof] のログイン資格情報を持つユーザーのみがプルーフを利用できるようにします。
      * **1 つの決定のみが必要：**&#x200B;プルーフに対する決定を 1 つだけ必要とします。
      * **元のファイルのダウンロード：**&#x200B;ユーザーがプルーフ用に元のファイルをダウンロードできるようにします。このオプションは、デフォルトで有効になっています。

        元のファイルのダウンロードについて詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md) に保存されているファイルをダウンロードを参照してください。

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **登録。ユーザーは、パブリック URL または埋め込みコードを使用して、プルーフにサインアップ可能：**&#x200B;組織外のレビュアーがパブリック URL または埋め込みコードを介してプルーフにサインアップできるようにします。

        このオプションを選択した場合、**プルーフにアクセスするには、サブスクライバーがメール内のリンクをクリックする必要があります**も利用できます。外部のレビュアーがメール内のリンクをクリックしてプルーフにアクセスするように求める場合に、このオプションを選択します。
**パブリック共有**&#x200B;オプションが選択されている場合、このオプションはデフォルトで有効になります。

      * **新規ゲストレビュアーのデフォルトの役割：**&#x200B;ゲストレビュアー用にデフォルトのプルーフの役割を選択します。オプションは、 **デフォルトの配達確認の役割**（モデレーターと作成者を除く）

   * 「**[!UICONTROL デフォルトのメールアラート設定]**」セクション：

      * **デフォルトのメールアラート：**&#x200B;ユーザーがメールの更新を受け取る頻度を選択します。**すべてのアクティビティ、自分のコメントに返信、決定、最終決定、時間別概要、日別概要、**&#x200B;または&#x200B;**無効**&#x200B;を選択します。

        デフォルトのメールアラートオプションについて詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) でのメール通知の設定を参照してください。

      * **新規ゲストレビュアー用のデフォルトのメールアラート：**&#x200B;ゲストレビュアーがメールの更新を受け取る頻度を選択します。オプションは、**デフォルトのメールの役割**&#x200B;のオプションと同じです。

      * **プルーフの準備が整ったらメールを送信：**&#x200B;プルーフの準備が整ったら、確認メールをユーザーに自動的に送信する場合に選択します。
      * **このユーザーに送信されるメールの形式：**&#x200B;ユーザーに送信されるメールのデフォルト形式として、**[!UICONTROL HTML]** または&#x200B;**[!UICONTROL プレーンテキスト]**&#x200B;を選択します。

   * 「**[!UICONTROL カスタムメッセージ設定]**」セクション：プルーフテンプレートの設定を作成します。

     テンプレートについて詳しくは、次を参照してください。

      * **プルーフの件名テンプレート：**&#x200B;プルーフの件名のテンプレートを作成します。
      * **プルーフメッセージテンプレート：**&#x200B;プルーフメッセージのテンプレートとその形式を作成します。
