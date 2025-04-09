---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: ' [!DNL Workfront Proof] でプルーフを生成する'
description: Workfront Proof を使用すると、ドキュメントまたは web サイトからプルーフを作成し、作成したプルーフを他のユーザーと共有できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 53%

---

# [!DNL Workfront Proof] でプルーフを生成

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

[!DNL Workfront Proof] を使用すると、ドキュメントまたは web サイトからプルーフを作成し、作成したプルーフを他のユーザーと共有できます。次の手順では、使用可能な様々な設定オプションについて説明します。

## ドキュメントからのプルーフの生成

1. 次のいずれかの操作を行って、**[!UICONTROL 新しいプルーフ]** ページを開きます。

   * 任意のページの左上隅にある **[!UICONTROL 新しいプルーフ]** ボタンをクリックします。
   * ドロップゾーン（エンタープライズ機能）経由で送信します。

1. 1 つ以上のドキュメントをプルーフするには、次のいずれかの方法で、プルーフするドキュメントを追加します（このプロセスを繰り返して複数のドキュメントを追加します）。

   * ファイルシステムから「**[!UICONTROL ファイルを追加]**」領域のドラッグ&amp;ドロップ領域にドキュメントをドラッグします。
   * **[!UICONTROL ファイルを追加]** 領域で **参照** リンクをクリックし、ワークステーションのファイルシステムからアップロードするドキュメントを検索して選択します。

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Web サイトのプルーフを行うには、「**[!UICONTROL ファイルの追加]**」領域に web サイトの URL を入力し、**[!UICONTROL Enter]** キーを押します。 この手順を繰り返して、プルーフに複数の web サイトを追加します。

   Web サイトのプルーフに関する詳細情報は、[URL のプルーフの生成](#generate-a-proof-for-a-url)を参照してください。

   ![ プルーフ web サイト ](assets/proof-website-350x65.png)

1. （オプション）アップロードしたファイルのファイル名を変更します。

   1. ドキュメントリストで、変更するドキュメント名にポインタを合わせ、「**[!UICONTROL 編集]**」アイコンをクリックします。

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. **[!UICONTROL プルーフ名]**&#x200B;フィールドで新しい名前を指定し、「**[!UICONTROL 完了]**」をクリックします。

   1. （オプション）アップロードするファイルを削除するには、ドキュメントリストで削除するドキュメントにポインタを合わせて **[!UICONTROL 削除]** アイコンをクリックします。

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. （任意）「**[!UICONTROL 互換性のあるすべてのファイルを 1 つのプルーフに結合する]**」オプションを有効にします。

      **このオプションが有効な場合：**&#x200B;すべての静的なファイルと web サイトは単一のプルーフで使用でき、一度に最大 50 個のファイルをアップロードすることができます。

      >[!NOTE]
      >
      >ビデオやインタラクティブ web サイトを含むインタラクティブファイルを結合して、単一のプルーフにすることはできません。

      **このオプションが無効な場合：**&#x200B;すべてのドキュメントおよび web サイトは個別のプルーフとして生成され、一度に 20 個までのファイルをアップロードできます。

      アップロードされたすべてのファイルと web サイトを単一のプルーフに組み合わせるには、以下のようにします。

      1. 「**[!UICONTROL 互換性のあるすべてのファイルを 1 つのプルーフに結合する]**」オプションを有効にします。
      1. **[!UICONTROL プルーフ名]** フィールドに、結合したプルーフの新しい名前を入力します。
      1. **[!UICONTROL ファイルを追加]**&#x200B;エリアで、ファイルを希望の順序にドラッグして、含まれるファイルの順序を変更します。ファイルの順序は、組み合わせたプルーフのページ順です。組み合わせプルーフの作成に関して詳しくは、[複数ページのプルーフを作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)を参照してください。

1. （オプション）複数のステージを含む自動ワークフローを使用する場合は、「**[!UICONTROL ワークフロー]**」セクションで次のオプションから選択します。

   * **基本：**&#x200B;プルーフの作成直後にそのプルーフへのアクセス権を持つユーザーを指定するには、このオプションを選択します。プルーフを複数のユーザーと共有することができます。

     プルーフの共有について詳しくは、[ 内でプルーフを共有する  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) を参照してください。

   * **自動：**&#x200B;複雑なレビュープロセスがある場合や、レビュー用のコンテンツを同じグループの同じ人々に定期的に送信する場合、このオプションを選択して、コンテンツのレビューと承認を管理します。自動ワークフローでは、プルーフはステージからステージへ、最終的な承認まで移動します。 関連するユーザーには、承認が必要なときにいつでも通知されます。

     自動ワークフローの作成に関して詳しくは、[自動ワークフローを使用してプルーフを設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2)を参照してください。

1. 前の手順で選択したユーザーに、メール通知とカスタムメッセージを送信するかどうかを選択します。

   * **このプルーフについて受信者に通知する：**&#x200B;ユーザーにメール通知を送信する場合は、このオプションを選択します。**[!UICONTROL 基本共有]**&#x200B;が&#x200B;**[!UICONTROL ワークフロー]**&#x200B;セクションで選択されている場合、プルーフの作成時にメール通知が送信されます。**[!UICONTROL 自動ワークフロー]**&#x200B;が&#x200B;**[!UICONTROL ワークフロー]**&#x200B;セクションで選択されている場合、ユーザーが関連付けられている自動ワークフローのステージにプルーフが入力されると、メール通知が送信されます。

   * **カスタムメッセージの追加：**&#x200B;通知にカスタムメッセージを含める場合は、このオプションを選択します。件名とメッセージ本文を指定できます。メッセージ本文には、太字、箇条書き記号、ハイパーリンクなどのリッチテキスト書式を含めることができます。

1. 以下のプルーフ設定のいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ログインが必要です。 このプルーフを他のユーザーと共有することはできません</td> 
      <td> <p>このオプションを選択した場合：</p> 
       <ul> 
        <li>ユーザーは、プルーフに追加されていない限り、プルーフにログインして表示できません。</li> 
        <li>購読を有効にできません。</li> 
       </ul> 
       <p>このオプションはデフォルトでは無効になっています。</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">校正判断に電子サインを必須にする</td> 
      <td><p>このオプションを選択した場合、ユーザーは、プルーフで決定を下す際に、ユーザー名とパスワードを指定する必要があります。</p>
      <p>このオプションはデフォルトでは無効になっています。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての必要な決定が行われた時点でプルーフをロックする</td> 
      <td> <p>この設定を有効にすると、すべての決定が行われた後、プルーフのステートがロックされます。最終承認者が決定を下すと、ステートは自動的にロック解除からロックに変更されます。</p> 
      <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">オリジナル ファイルのダウンロードを許可する</td> 
      <td> <p><strong></strong> このオプションを選択すると、レビューアは、プルーフの作成元のファイルをダウンロードできます。</p> <p>このオプションの選択を解除すると、ダウンロードアイコンは表示されなくなります。</p>
      <p>このオプションは、デフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコード経由によるプルーフの共有を許可する</td> 
      <td><p>このオプションを選択した場合、プルーフは公開 URL または埋め込みコード経由で共有できます。</p>
       <p>このオプションは、デフォルトで有効になっています。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコード経由によるプルーフの登録を許可します</td> 
      <td> <p>このオプションを選択すると、プルーフに追加されていない人物がプルーフを購読できます。 プルーフを購読しているユーザーには、次の設定で定義した役割とメールが付与されます。</p> 
       <ul> 
        <li><strong>サブスクライバーの役割</strong>：プルーフに登録するすべてのレビュー担当者に割り当てられる、デフォルトのプルーフの役割です。</li> 
        <li><strong>サブスクライバーのメールアラート設定</strong>：プルーフに登録するすべてのレビュー担当者に割り当てられる、デフォルトのメールアラートです。</li> 
        <li> <p><strong>メールのリンクからプルーフにアクセスする必要があります</strong>：プルーフへのリンクを含むメールをサブスクライバーが受信するかどうかを設定します。<strong> メールなし </strong> （プルーフにアクセスするためにメールリンクが必要ありません）、<strong> プルーフ通知メールのみ </strong> （サブスクライバーは検証なしのメールでプルーフへのリンクを受信します）、または <strong> 検証とプルーフ通知メール </strong> （サブスクライバーはプルーフへのリンクをメールで受信し、プルーフにアクセスするにはリンクをクリックする必要があります。 このオプションの目的は、ユーザーがアクセスできる正しいメールアドレスを入力していることを確認することです）。</p> <p>メモ：プルーフに自動ワークフローが添付されている場合、すべての購読は、プルーフの所有者に確認メールを生成するので、プルーフの所有者がユーザーを追加するステージを決定できます。</p> </li> 
       </ul> 
        <p>このオプションはデフォルトでは無効になっています。</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL プルーフを作成]** をクリックします。 Workfrontは、選択したドキュメントまたは web サイトのプルーフを生成します。

   ドキュメントのアップロードの遅れ時間は、ファイルのサイズとタイプによって異なります。 大きなファイルの生成には時間がかかります。 Workfrontが引き続きファイルを生成するので、ページから移動できます。 アップロードできるファイルの最大サイズは 4GB です。

## URL を使用した静的プルーフの生成 {#generate-a-proof-for-a-url}

Web サイトの URL を使用して静的プルーフを生成できます。

>[!NOTE]
>
>[!DNL Workfront] 環境が [!DNL Workfront Proof] プレミアムアカウントと統合されている場合にのみ、URL のインタラクティブなプルーフを生成できます。この節で説明しているようにプルーフを使用できない場合は、Workfront管理者にお問い合わせください。

1. 次のいずれかの操作を行って、**[!UICONTROL 新しいプルーフ]** ページを開きます。

   * 任意のページの左上隅にある **[!UICONTROL 新しいプルーフ]** ボタンをクリックします。
   * ドロップゾーン（エンタープライズ機能）経由で送信します。

1. **新しいプルーフ** ページの「**[!UICONTROL ファイルを追加]**」領域で、プルーフを作成する Web サイトの URL を入力し、キーボードの **[!UICONTROL Enter]** または **[!UICONTROL Return]** キーを押します。

1. （オプション）このプロセスを繰り返して、プルーフに複数の web サイトを追加します。

   ![proof_website.png](assets/proof-website-350x65.png)

1. **[!UICONTROL ファイルを追加]** 領域で、URL の右側にある **編集** アイコンをクリックして、web サイトのプルーフの詳細を開きます。

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. **[!UICONTROL プルーフ名]** を入力します。 デフォルトでは、プルーフ名はサイトの URL と同じです。

1. 次のいずれかの **[!UICONTROL サイトコンテンツを処理]** オプションを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">スクリーンショットのキャプチャ</td> 
      <td>URL のトップページの静的画像のプルーフを作成します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">対話型</td> 
      <td> <p>レビュー担当者がサイト内を移動したり、HTML 5 画像、Flash 要素などを表示したりできるプルーフを作成します。</p> <p>インタラクティブなプルーフを作成するには、web サイトが安全なプロトコル（https）でホストされている必要があります。 また、iframe に埋め込めない web サイトは、インタラクティブプルーフとして生成することはできません（iframe の埋め込み制限は、埋め込もうとしている web サイトによって制御されます）。</p> <p>最初のプルーフを作成した後、それに続くバージョンを作成する場合は、この設定を変更できません。</p> <p>インタラクティブなプルーフについて詳しくは、<a href="#generate-a-proof-for-interactive-content" class="MCXref xref">インタラクティブなコンテンツのプルーフを生成</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">スクリーンショットの解像度</td> 
      <td> <p>（このオプションは、インタラクティブなプルーフには使用できません）。 コンテンツが表示される解像度を調整したり、複数の解像度を選択したりできます。</p> <p>これにより、プルーフを確認するユーザーは、携帯電話、タブレット、モニターなどの様々なサイズのデバイスで、コンテンツがどのように表示されるかを確認できます。</p> <p>複数の解像度を選択した場合は、選択した解像度ごとに別々のプルーフが作成されます。</p> <p>ユーザーがプルーフにコメントする際、現在の画面の解像度がコメントに自動的に表示され、コメントが関連付けられている解像度を他のユーザーが認識できるようになります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブページの検索</td> 
      <td>（このオプションは、インタラクティブなプルーフには使用できません）。 Web サイトのページ間を移動するには、このオプションを選択します。 Web サイトは、メインページから最大 2 レベルまで展開できます。ページの上にマウスポインターを置くと、ページの URL が表示され、プルーフするページのみを選択します。 選択する各ページは、デフォルトで個々のプルーフとして作成されます。 または、「互換性のあるすべてのファイルを 1 つのプルーフに結合する <strong> オプションを有効にするこ </strong> もできます。</td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）プルーフの共有、自動ワークフローの追加、アクセス設定やサブスクリプション設定など、その他のプルーフオプションを設定します。これらのオプションについて詳しくは、次の記事を参照してください。

   * [ [!DNL Adobe Workfront] でプルーフを共有する](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [ [!DNL Workfront Proof] で自動ワークフローを使用したプルーフを設定する](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [プルーフのアクセスおよびサブスクリプション設定を行う](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 「**[!UICONTROL 完了]**」をクリックします。

1. 「**[!UICONTROL プルーフを作成]**」をクリックします。

## インタラクティブコンテンツのプルーフの生成 {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

インタラクティブコンテンツについて詳しくは、[インタラクティブコンテンツのプルーフの概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)を参照してください。

* [インタラクティブコンテンツを URL として追加](#add-interactive-content-as-a-url)
* [インタラクティブコンテンツを ZIP ファイルとして追加](#add-interactive-content-as-a-zip-file)

### インタラクティブコンテンツを URL として追加 {#add-interactive-content-as-a-url}

インタラクティブ URL プルーフの追加方法について詳しくは、[URL のプルーフの生成 ](#generate-a-proof-for-a-url) を参照してください。

### インタラクティブコンテンツを ZIP ファイルとして追加 {#add-interactive-content-as-a-zip-file}

1. .zip バンドルファイルを作成して、コンテンツを準備します。

   .zip バンドルファイルの仕様について詳しくは、[ インタラクティブコンテンツ配達確認の概要 ](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md) を参照してください。

1. 次のいずれかの操作を行って、**[!UICONTROL 新しいプルーフ]** ページを開きます。

   * 任意のページの左上隅にある **[!UICONTROL 新しいプルーフ]** ボタンをクリックします。
   * ドロップゾーン（エンタープライズ機能）経由で送信します。

1. **[!UICONTROL 新規プルーフ]** ページで、インタラクティブな.zip バンドルを **[!UICONTROL ファイルを追加]** 領域にドラッグ&amp;ドロップします。

1. （オプション）プルーフの共有、自動ワークフローの追加、アクセス設定やサブスクリプション設定など、その他のプルーフオプションを設定します。これらのオプションについて詳しくは、次の記事を参照してください。

   * [ [!DNL Adobe Workfront] 内でプルーフを共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [プルーフのアクセスおよびサブスクリプション設定を行う](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. **[!UICONTROL プルーフを作成]** をクリックします。 Workfrontが zip ファイルのプルーフを生成します。

   ドキュメントのアップロードの遅れ時間は、zip ファイルのサイズによって異なります。 Workfrontが引き続きファイルを生成するので、ページから移動できます。 アップロードできるファイルの最大サイズは 4GB です。
