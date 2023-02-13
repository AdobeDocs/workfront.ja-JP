---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: バックアップ [!DNL Workfront Proof] データ
description: すべてのデータのバックアップを [!DNL Workfront Proof] バックアップ機能を使用する。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 0%

---

# バックアップ [!DNL Workfront Proof] データ

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

## バックアップの概要

すべてのデータのバックアップを [!DNL Workfront Proof] バックアップ機能を使用する。

バックアップは、.zip ファイルとして配信されます。 これには、すべてのデータ（すべての配達確認のすべてのバージョンに対するコメントと回答を含む）の XML エクスポートが含まれます。ただし、配達確認としてアップロードした元のファイルは含まれません。

ダウンロード用に作成された各バックアップ.zip ファイルには、次のような一意のファイル名が付けられます。

9789_05_05_2011_61703.zip

この例のファイル名は次の情報を提供します。

* 9789 はお客様の [!DNL Workfront Proof] アカウント ID
* 05_05_2011は作成日、2011 年 5 月 5 日
* 61703は、システムに割り当てられた乱数です

この命名規則を使用すると、すべてのバックアップ.zip ファイルをコンピュータ上の 1 か所に簡単に保存でき、各バックアップがいつ作成されたかを正確に把握できます。

この [!UICONTROL バックアップ] 関数を使用して、リソースの使用方法を決定できます。

* アクティブな配達確認やアーカイブした配達確認を失うことなく、ストレージ領域を解放できます。 バックアップをリクエストし、配達確認を削除して、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* 最初にアップロードしたファイルにアクセスできます [!DNL Workfront] 配達確認。 これらは、 [!UICONTROL 元のファイルをダウンロード] 関数を使用して、配達確認を削除する必要があります。

>[!NOTE]
>
>バックアップを使用する際は、次の点を考慮してください。
>
>* バックアップは、Enterprise プランと Unlimited プランで利用できます。 お問い合わせください [営業チーム](mailto:sales@proofhq.com) 見積もりの
>* データのエンコーディングの種類は、デフォルトで UTF-8 に設定されています。この設定をお勧めします。 これは、インターネットアプリケーションで最も一般的に使用されるエンコーディングタイプです。
>* リクエストできるリクエストは 1 つだけです [!DNL backup] 一度に バックアップ.zip ファイルの処理中に、「バックアップ」タブの「新しいバックアップをリクエスト」リンクが表示されず、表示されるメッセージは変更されません。 バックアップのリクエストについては、 [で新しいデータバックアップをリクエスト [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>




## データのバックアップ

1. クリック **[!UICONTROL アカウント設定]** の右上隅に [!DNL Workfront Proof] インターフェイス。 (1)
1. 次をクリック： **[!UICONTROL バックアップ]** タブをクリックします。 (2)
1. 次をクリック： **[!UICONTROL 新しいバックアップをリクエスト]** リンク (3)

バックアップの準備が整うと、次の処理が行われます。

* 次のメールが届きます： [!DNL Workfront Proof] これを ( [!DNL Workfront Proof] バックアップの準備ができました。」) このメールには、バックアップデータのダウンロードリンクが含まれています。
* この [アカウント設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 「バックアップ」タブには、バックアップデータのダウンロードリンクが表示されます。
* [ バックアップ ] タブに [ 新しいバックアップをリクエスト ] リンク (3) が再び表示されます

これで、データを zip ファイルとしてダウンロードする準備が整います。 バックアップ.zip ファイルは、通知メールまたは [!UICONTROL アカウント設定]を使用できます。

* [電子メール通知からバックアップ.zip ファイルをダウンロードしています](#downloading-your-backup-zip-file-from-your-email-notification)
* [アカウント設定からバックアップ.zip ファイルをダウンロードしています](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## 電子メール通知からバックアップ.zip ファイルをダウンロードしています {#downloading-your-backup-zip-file-from-your-email-notification}

バックアップ.zip ファイルをダウンロードする準備が整ったら、次の宛先から電子メールを受け取ります： [!DNL Workfront Proof] 件名を [!DNL Workfront Proof] バックアップの準備が整いました。」

電子メールからバックアップ.zip ファイルをダウンロードするには：

1. 電子メールのダウンロードリンクをクリックします。\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   現在、 [!DNL Workfront Proof]をクリックすると、新しいブラウザーウィンドウが開き、ログインページが表示されます。

## アカウント設定からバックアップ.zip ファイルをダウンロードしています {#downloading-your-backup-zip-file-from-the-account-settings}

バックアップ.zip ファイルをダウンロードする準備が整ったら、 [!UICONTROL バックアップ] 「 」タブには、ダウンロードリンクが表示され、これが示されます。 また、 [!UICONTROL 新しいバックアップをリクエスト] リンクが再び表示されます。

1. クリック **[!UICONTROL アカウント設定]** の右上隅に [!DNL Workfront Proof] インターフェイス。 (1)
1. 次をクリック： **[!UICONTROL バックアップ]** タブをクリックします。 (2)\
   アカウント内のユーザがバックアップをリクエストしていない場合、 [!UICONTROL バックアップ] [ ] タブには、バックアップが存在しないことが示されます。 ユーザーがバックアップをリクエストした場合、「 」タブには最後のバックアップの作成日とダウンロードリンクが表示されます。

1. 次をクリック： **[!UICONTROL バックアップをダウンロード]** リンク。 (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) 「ファイルのダウンロード」画面が表示され、ダウンロードファイルを開くか、「保存する」かを尋ねられます。

1. クリック **[!UICONTROL 保存]**&#x200B;次に、バックアップ.zip ファイルを保存するコンピュータ上の場所を選択します。\
   最新のバックアップの日付を示すメッセージは、 [!UICONTROL バックアップ] 次にバックアップをリクエストするまでのページ。 「バックアップをダウンロード」リンクは、最後のバックアップに適用されます。 常に [!UICONTROL 新しいバックアップをリクエスト] リンクが表示されたら、クリックして別のバックアップをリクエストできます。

## バックアップ.zip ファイル内のファイルについて

バックアップ.zip ファイルには、データがバックアップされた時点までのアクティブな配達確認とアーカイブされた配達確認の情報を含む 7 つの CSV（コンマ区切り値またはコンマ区切り）ファイルが含まれています。

* comments.csv — 配達確認に関するコメントを含めます
* comment_replies.csv — 配達確認に対するコメントへの応答を含みます。 organization.csv — 数値識別子と組織の名前（アカウント）が含まれます。
* contacts.csv — 各連絡先の数値識別子、名前、組織が含まれます。
* files.csv — 配達確認の詳細ページまたはファイルの詳細ページからの情報や、にアップロードされた配達確認またはファイルに関する情報が含まれます。 [!DNL Workfront Proof]
* recipients.csv — レビュー担当者、レビュー担当者、承認者などとして指定された各人の数値識別子、役割、決定が含まれます。これらの人は、に関するレビュー用に配達確認がアップロードされたときに実行されます。 [!DNL Workfront Proof]
* users.csv — 数値識別子とアカウント内のすべてのユーザーの名前が含まれます。

これらのファイルは、任意の zip ユーティリティを使用してバックアップ.zip ファイルから抽出し、コンピュータ上の任意の場所に保存することができます。 zip ファイルを保存し、個々の CSV ファイルを抽出した後、内部記録の保持に必要に応じて情報を操作できます。

リクエストで作成された各バックアップ.zip ファイルには、バックアップ作成日を含む固有の名前が付けられますが、各バックアップ.zip ファイルに含まれる CSV ファイルには、常に同じ名前が付けられます。 バックアップファイルが互いに異なる状態に保たれるように、次のいずれかの方法を使用できます。

* 各バックアップ.zip ファイルと、そのファイルから抽出した CSV ファイルに対して新しいフォルダを作成します。
* 個々の CSV ファイルの名前を変更し、zip ファイルから抽出したバックアップ日を含めます。

>[!NOTE]
>
>If [!DNL Microsoft Excel] がコンピュータにインストールされている場合、抽出ユーティリティは、個々の CSV ファイルのファイルタイプを [!DNL Microsoft Office Excel] コンマ区切り値ファイル。 抽出した CSV ファイルを開くには、 [!DNL Excel] ファイルを [!DNL Excel] ワークブック (&#42;.xlsx) またはその他のファイルタイプ。
