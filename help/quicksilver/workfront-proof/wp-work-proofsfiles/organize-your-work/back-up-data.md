---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: ' [!DNL Workfront Proof]  データのバックアップ'
description: バックアップ機能を使用して、 [!DNL Workfront Proof]  のすべてのデータのバックアップをリクエストできます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: ht
source-wordcount: '1046'
ht-degree: 100%

---

# [!DNL Workfront Proof] データのバックアップ

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

## バックアップの概要

バックアップ機能を使用して、[!DNL Workfront Proof] のすべてのデータのバックアップをリクエストできます。

バックアップは、.zip ファイルとして配信されます。これには、すべてのデータ（すべてのプルーフのすべてのバージョンに対するコメントと応答を含む）の XML 書き出しが含まれますが、プルーフとしてアップロードした元のファイルは含まれません。

ダウンロード用に作成された各バックアップ.zip ファイルには、次のような一意のファイル名が付けられます。

9789_05_05_2011_61703.zip

この例のファイル名は次の情報を提供します。

* 9789 は [!DNL Workfront Proof] アカウント ID
* 05_05_2011 は作成日の 2011年5月5日
* 61703 は、システムに割り当てられたランダムな数値

この命名規則を使用すると、すべてのバックアップ.zip ファイルをコンピューター上の 1 か所に簡単に保存でき、各バックアップがいつ作成されたかを正確に把握できます。

[!UICONTROL バックアップ]機能を使用して、リソースの使用方法を決定できます。

* アクティブなプルーフまたはアーカイブされたプルーフを失うことなく、ストレージスペースを確保できます。バックアップをリクエストし、プルーフを削除して、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) のごみ箱のアイテムの復元と完全削除で空にします。
* 最初に [!DNL Workfront] プルーフにアップロードしたファイルにアクセスできます。プルーフを削除する前に、[!UICONTROL 元のファイルをダウンロード]機能を使用してダウンロードできます。

>[!NOTE]
>
>バックアップを使用する際は、次の点を考慮してください。
>
>* バックアップは、Enterprise プランと Unlimited プランで利用できます。見積もりについて詳しくは、[セールスチーム](mailto:sales@proofhq.com)にお問い合わせください。
>* データのエンコーディングタイプは、デフォルトで UTF-8 に設定され、アドビはこの設定をお勧めします。これは、インターネットアプリケーションで最も一般的に使用されるエンコーディングタイプです。
>* 一度に 1 つの [!DNL backup] だけリクエストできます。バックアップ.zip ファイルの処理中は、「バックアップ」タブの「新しいバックアップをリクエスト」リンクは表示されず、表示されるメッセージは変わらないままになります。バックアップのリクエストについて詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md) での新しいデータバックアップのリクエストを参照してください。
>



## データのバックアップ

1. [!DNL Workfront Proof] インターフェイスの右上隅にある&#x200B;**[!UICONTROL アカウント設定]**&#x200B;をクリックします。（1）
1. 「**[!UICONTROL バックアップ]**」タブをクリックします。（2）
1. 「**[!UICONTROL 新しいバックアップをリクエスト]**」リンクをクリックします。（3）

バックアップの準備が整うと、次の処理が行われます。

* [!DNL Workfront Proof] から「[!DNL Workfront Proof] バックアップの準備ができました」というメールが届きます。このメールには、バックアップデータのダウンロードリンクが含まれています。
* [アカウント設定](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)の「バックアップ」タブには、バックアップデータのダウンロードリンクが表示されます。
* 「バックアップ」タブに「新しいバックアップをリクエスト」リンク（3）が再び表示されます

データを zip ファイルとしてダウンロードする準備が整います。バックアップ.zip ファイルは、次の節で説明されるように、通知メールまたは[!UICONTROL アカウント設定]を使用できます。

* [メール通知からのバックアップ.zip ファイルのダウンロード](#downloading-your-backup-zip-file-from-your-email-notification)
* [アカウント設定からのバックアップ.zip ファイルのダウンロード](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## メール通知からのバックアップ.zip ファイルのダウンロード {#downloading-your-backup-zip-file-from-your-email-notification}

バックアップ.zip ファイルをダウンロードする準備が整った場合、[!DNL Workfront Proof] から「[!DNL Workfront Proof] バックアップの準備が整いました」という件名のメールが届きます。

メールからバックアップ.zip ファイルをダウンロードするには、次の手順に従います。

1. メールのダウンロードリンクをクリックします。\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   現在 [!DNL Workfront Proof] にログインしていない場合は、新しいブラウザーウィンドウが開き、ログインページが表示されます。

## アカウント設定からのバックアップ.zip ファイルのダウンロード {#downloading-your-backup-zip-file-from-the-account-settings}

バックアップ.zip ファイルをダウンロードする準備が整ったら、「[!UICONTROL バックアップ]」タブにダウンロードリンクが表示されます。さらに、「[!UICONTROL 新しいバックアップを要求]」リンクが再び表示されます。

1. [!DNL Workfront Proof] インターフェイスの右上隅にある「**[!UICONTROL アカウント設定]**」をクリックします。（1）
1. 「**[!UICONTROL バックアップ]**」タブをクリックします。（2）\
   アカウント内のユーザがバックアップをリクエストしていない場合、「[!UICONTROL バックアップ]」タブにはバックアップがないことが示されます。ユーザーがバックアップをリクエストした場合、タブには最後のバックアップの作成日とダウンロードリンクが表示されます。

1. 「**[!UICONTROL バックアップをダウンロード]**」のリンクをクリックします。（3）\
   ![Download_Backup.png](assets/download-backup-350x167.png)「ファイルのダウンロード」画面が表示され、ダウンロードファイルを開くか、保存するかを尋ねられます。

1. 「**[!UICONTROL 保存]**」をクリックし、バックアップ.zip ファイルを保存するコンピューター上の場所を選択します。\
   最新のバックアップの日付を示すメッセージは、次回バックアップをリクエストするまで、[!UICONTROL バックアップ]ページの下部に表示されたままになります。「バックアップをダウンロード」のリンクは、最後のバックアップに適用されます。 「[!UICONTROL 新しいバックアップをリクエスト]」のリンクが表示されたら、それをクリックして別のバックアップをリクエストできます。

## バックアップ.zip ファイル内のファイルについて

バックアップ.zip ファイルには、データがバックアップされた時点までのアクティブなプルーフと、アーカイブされたプルーフの情報を含む 7 つの CSV（コンマ区切り値またはコンマ区切り）ファイルが含まれています。

* comments.csv - プルーフに関するコメントが含まれます
* comment_replies.csv - プルーフに対するコメントへの応答が含まれます。organization.csv - 数値識別子と組織の名前（アカウント）が含まれます
* contacts.csv - 各連絡先の数値識別子、名前、組織が含まれます
* files.csv - [!DNL Workfront Proof] にアップロードされたプルーフまたはファイルに関するプルーフの詳細ページ、またはファイルの詳細ページからの情報が含まれます
* recipients.csv - プルーフを [!DNL Workfront Proof] でレビューするためにアップロードする際に、レビュアー、承認者などとして指定された各ユーザーの数値識別子、役割、決定が含まれます
* users.csv - 数値識別子とアカウント内のすべてのユーザーの名前が含まれます

これらのファイルは、任意の zip ユーティリティを使用してバックアップ.zip ファイルから抽出し、コンピューター上の任意の場所に保存できます。 zip ファイルを保存し、個々の CSV ファイルを抽出した後、内部レコードの保持用に必要に応じて情報を操作できます。

リクエストで作成された各バックアップ .zip ファイルには、バックアップ作成日を含む固有の名前が付けられますが、各バックアップ .zip ファイルに含まれる CSV ファイルには、常に同じ名前が付けられます。 バックアップファイルが互いに区別されるようにするには、次のいずれかの方法を使用できます。

* 各バックアップ .zip ファイルと、そのファイルから抽出した CSV ファイルに対して新規フォルダーを作成します。
* zip ファイルから抽出する際に、個々の CSV ファイルの名前を変更し、バックアップの日付を含めます。

>[!NOTE]
>
>[!DNL Microsoft Excel] がコンピューターにインストールされている場合、抽出ユーティリティは、個々の CSV ファイルのファイルタイプを [!DNL Microsoft Office Excel] コンマ区切り値ファイルとしてリストする場合があります。 [!DNL Excel] を使用して抽出された CSV ファイルを開き、そのファイルを [!DNL Excel] ワークブック（&#42;.xlsx）またはその他のファイルタイプとして保存できます。
