---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: で配達確認を生成 [!DNL Workfront Proof]
description: Workfrontの配達確認を使用すると、ドキュメントや Web サイトから配達確認を作成し、他のユーザーと共有できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '2254'
ht-degree: 0%

---

# で配達確認を生成 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] を使用すると、ドキュメントまたは Web サイトから配達確認を作成し、他のユーザーと配達確認を共有できます。 次の手順では、使用可能な様々な設定オプションについて説明します。

## ドキュメントの配達確認を生成

1. 次のいずれかの操作を行って、新しい配達確認の作成を開始し、 [!UICONTROL 新しい配達確認] ページ：

   * 緑をクリック **[!UICONTROL 新しい配達確認]** 」ボタンをクリックします。
   * Adobe Analytics の **[!UICONTROL ダッシュボード]** 領域、内 **[!UICONTROL 概要]** タブで、 **[!UICONTROL 新しい配達確認]** リンク。

   * ドロップゾーン（エンタープライズ機能）を使用して送信します。
   * The **[!UICONTROL 新しい配達確認]** ページが表示されます。

1. 1 つ以上のドキュメントを配達確認するには、次のいずれかの方法で配達確認するドキュメントを追加します（配達確認する複数のドキュメントを追加するには、この手順を繰り返します）。

   * ファイルシステムからドキュメントを **[!UICONTROL ファイルを追加]** 領域。
   * ドラッグ&amp;ドロップ領域で、 **[!UICONTROL ファイルを追加]** 領域を参照し、アップロードするドキュメントをワークステーション上のファイルシステムから探して選択します。

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. 1 つ以上の Web サイトを配達確認するには、配達確認する Web サイトの URL を **[!UICONTROL ファイルを追加]** 「 」エリアで「 」をクリックし、 **[!UICONTROL 入力]**.

1. （オプション）複数の Web サイトを配達確認用に追加する場合は、このプロセスを繰り返します。

   Web サイトの校正について詳しくは、 [URL の配達確認を生成](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. （オプション）アップロードしたファイルのファイル名を変更します。

   1. 変更するドキュメント名の上にマウスを移動します（ドキュメントリスト内のドキュメント名）。 **[!UICONTROL ファイルを追加]** 「 」領域で、 **[!UICONTROL 編集]** アイコン。

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. Adobe Analytics の **[!UICONTROL 配達確認名]** フィールドに新しい名前を入力し、「 **[!UICONTROL 完了]**.

   1. （オプション）ファイルをアップロードから削除するには、削除するドキュメントの上にマウスを移動して、 **[!UICONTROL ファイルを追加]** 「 」領域で、 **[!UICONTROL 削除]** アイコン。

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. （オプション）オプションを有効にします。 **[!UICONTROL 互換性のあるすべてのファイルを 1 つの配達確認に結合する]**.

      **このオプションが有効な場合：** すべての静的ファイルおよび Web サイトは、1 つの配達確認で使用でき、一度に 50 個までのファイルをアップロードできます。

      >[!NOTE]
      >
      >ビデオやインタラクティブ Web サイトを含むインタラクティブファイルを結合して、1 つの配達確認にすることはできません。

      **このオプションが無効な場合：** すべてのドキュメントおよび Web サイトは個々の配達確認として生成され、一度に 20 個までのファイルをアップロードできます。

      アップロードされたすべてのファイルと Web サイトを 1 つの配達確認に組み合わせるには：

      1. オプションを有効にします。 **[!UICONTROL 互換性のあるすべてのファイルを 1 つの配達確認に結合する]**.
      1. Adobe Analytics の **[!UICONTROL 配達確認名]** 「 」フィールドで、組み合わせ配達確認の新しい名前を指定します。
      1. Adobe Analytics の **[!UICONTROL ファイルを追加]** 「 」領域で、ファイルを目的の順序にドラッグして、含まれるファイルの順序を変更します。 ファイルの順序は、組み合わせ配達確認のページ順です。 組み合わせ配達確認の作成について詳しくは、 [複数ページの配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. （オプション）複数のステージを含む自動ワークフローを使用する場合は、 **[!UICONTROL ワークフロー]** 「 」セクションで、次のオプションから選択します。

   * **基本：** 配達確認の作成直後にその配達確認へのアクセス権を持つユーザーを指定するには、このオプションを選択します。 配達確認を複数のユーザーと共有できます。

     配達確認の共有について詳しくは、 [内で配達確認を共有 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **自動：** 複雑なレビュープロセスがある場合や、レビュー用のコンテンツを同じグループの同じ人々に定期的に送信する場合は、コンテンツのレビューと承認を管理する場合に、このオプションを選択します。 自動ワークフローを使用すると、配達確認はステージからステージへと移動し、最終承認がおこなわれます。 承認が必要になった場合は、該当するユーザーに通知が送信されます。

     自動ワークフローの作成について詳しくは、 [で自動ワークフローを使用した配達確認の設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. 前の手順で選択したユーザーに電子メール通知とカスタムメッセージを送信するかどうかを選択します。

   * **この配達確認について受信者に通知する：** ユーザーに電子メール通知を送信する場合は、このオプションを選択します。 条件 **[!UICONTROL 基本共有]** が **[!UICONTROL ワークフロー]** 「 」セクションに入力すると、配達確認の作成時に e メール通知が送信されます。 条件 **[!UICONTROL 自動ワークフロー]** が **[!UICONTROL ワークフロー]** 「 」セクションに入力すると、配達確認が、ユーザーが関連付けられている自動ワークフローのステージに入ると、電子メール通知が送信されます。

   * **カスタムメッセージの追加：** 通知にカスタムメッセージを含める場合は、このオプションを選択します。 件名とメッセージ本文を指定できます。 メッセージ本文には、太字、箇条書き記号、ハイパーリンクなどのリッチテキスト書式を含めることができます。

1. 次のいずれかの配達確認設定を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ログインが必要 — 配達確認は他のユーザーとのみ共有できます</td> 
      <td> <p><strong>ログインが必要 — 配達確認は他のユーザーとのみ共有できます：</strong> このオプションを選択した場合は、 [!DNL Workfront Proof] ユーザーは、配達確認を表示できます。</p> <p>このオプションはデフォルトで無効になっています。URL を持つユーザーは誰でも配達確認を表示できます。</p> <p>このオプションを選択した場合：</p> 
       <ul> 
        <li>ユーザーは、配達確認に追加されていない限り、配達確認にサインインできません。</li> 
        <li>購読を有効にできません。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">この配達確認に必要な決定は 1 つだけです</td> 
      <td> <p>このオプションを選択すると、レビューは、ある意思決定者が決定した後に完了します。</p> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">電子署名するには決定が必要です</td> 
      <td>配達確認を決定する際には、ユーザー名とパスワードを指定する必要があります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての必要な決定がおこなわれたら配達確認をロックする</td> 
      <td> <p><strong></strong> この設定を有効にすると、すべての決定がおこなわれた後、配達確認の状態がロックされます。 最終承認者が決定を下すと、状態は自動的にロック解除からロックに変更されます。</p> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">元のファイルをダウンロード</td> 
      <td> <p><strong></strong> このオプションを選択すると、レビュー担当者は、配達確認の作成元のファイルをダウンロードできます。</p> <p>このオプションの選択を解除すると、ダウンロードアイコンは表示されなくなります。<br>このオプションは、デフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコードを使用して配達確認を共有</td> 
      <td>このオプションを選択した場合、配達確認はパブリック URL または埋め込みコード経由で共有できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコードで配達確認に登録</td> 
      <td> <p>このオプションを選択すると、配達確認に明示的に追加されていないユーザーも配達確認を購読できます。 配達確認を購読しているユーザーには、次の設定で定義した役割と E メールが付与されます。</p> 
       <ul> 
        <li><strong>購読者の役割</strong>：配達確認を購読するすべてのレビュー担当者に割り当てられる、デフォルトの配達確認の役割。</li> 
        <li><strong>購読者向けの電子メールアラート設定</strong>：配達確認を購読するすべてのレビュー担当者に割り当てられるデフォルトの E メールアラート。</li> 
        <li> <p><strong>次に必要な電子メールリンクを介した配達確認へのアクセス：</strong>：配達確認へのリンクを含む E メールを購読者が受信するかどうかを設定します。 次の項目を選択できます。 <strong>メールなし</strong> （配達確認にアクセスするには、E メールリンクは必要ありません）。 <strong>配達確認通知 E メールのみ</strong> （購読者が、確認なしで E メールで配達確認へのリンクを受け取る場合）、または <strong>検証および配達確認の通知 E メール</strong> （購読者は、E メールで配達確認へのリンクを受け取り、リンクをクリックして配達確認にアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しい E メールアドレスを入力したことを確認することです）。</p> <p>注意：配達確認に自動ワークフローがすべて添付されている場合、すべての購読が配達確認の所有者に確認 E メールを生成するので、配達確認の担当者を追加するステージを決定できます。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 配達確認を作成]**.

   Workfrontは、選択したドキュメントまたは Web サイトの配達確認の生成を開始します。 ドキュメントのアップロードに関する遅延時間は、ファイルサイズとタイプに応じて異なります。 大きなファイルの生成に時間がかかるので、しばらくお待ちください。 ページから移動すると、Workfrontは引き続きファイルを生成します。 最大ファイルアップロードサイズは 4GB です。

   配達確認が生成されたら、「 **[!UICONTROL 配達確認に移動]** をクリックして、校正ツールを起動します。

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   文書が校正ツールに表示されます。

   自分のアカウントで校正が有効になっていないユーザーは、引き続きドキュメントを表示し、配達確認にコメントを付けることができます。

## URL の配達確認を生成 {#generate-a-proof-for-a-url}

URL の配達確認を初めて生成できます。 または、以前に配達確認が生成された URL 配達確認の新しいバージョンを生成できます。

>[!NOTE]
>
>URL に対してインタラクティブな配達確認を生成できるのは、 [!DNL Workfront] 環境が [!DNL Workfront Proof] プレミアムアカウント。 この節で説明したように、校正を使用できない場合は、システム管理者に問い合わせてください。

URL の配達確認を生成するには：

1. 次のいずれかの操作を行って、新しい配達確認の作成を開始し、 [!UICONTROL 新しい配達確認] ページ：

   * 緑をクリック **[!UICONTROL 新しい配達確認]** 」ボタンをクリックします。
   * Adobe Analytics の **[!UICONTROL ダッシュボード]** 領域、内 **[!UICONTROL 概要]** タブで、 **[!UICONTROL 新しい配達確認]** リンク。

   * ドロップゾーン（エンタープライズ機能）を使用して送信します。

1. （条件付き） **[!UICONTROL 新しい配達確認]** 既存の配達確認の新しいバージョンを作成するために表示されるページ：

   1. 新しいバージョンを追加する URL 配達確認を選択します。
   1. 次をクリック： **[!UICONTROL 新しいバージョン]** 」ボタンをクリックします。

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. 表示される新しい配達確認のバージョンページで、配達確認を行う Web サイトの URL を **[!UICONTROL ファイルを追加]** 「 」エリアで「 」をクリックし、 **[!UICONTROL 入力]**.

1. （オプション）複数の Web サイトを配達確認用に追加する場合は、このプロセスを繰り返します。

   ![proof_website.png](assets/proof-website-350x65.png)

1. ドキュメントリスト内の Web サイトをクリックします。 **[!UICONTROL ファイルを追加]** 領域。

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. を指定します。 **[!UICONTROL 配達確認名]** 配達確認のために。

   デフォルトでは、配達確認の名前はサイトの URL と同じです。

1. 選択 **[!UICONTROL サイトコンテンツの処理]** options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">スクリーンショットをキャプチャ</td> 
      <td>URL の最前面ページの静的画像の配達確認を作成します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">対話型</td> 
      <td> <p>レビュー担当者がサイト内を移動したり、HTML5 個の画像、Flash要素などを表示したりできる配達確認を作成します。</p> <p>インタラクティブな配達確認を作成するには、Web サイトを安全なプロトコル (https) でホストする必要があります。 また、iframe に埋め込むことができない Web サイトを、インタラクティブな配達確認として生成することはできません（iframe の埋め込み制限は、埋め込もうとしている Web サイトによって制御されます）。</p> <p>最初の配達確認を作成した後のバージョンを作成する場合は、この設定を変更できません。</p> <p>インタラクティブ校正の詳細については、 <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">インタラクティブコンテンツの配達確認を生成</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">スクリーンショットの解像度</td> 
      <td> <p>（このオプションは、インタラクティブな配達確認には使用できません）。 コンテンツを表示する解像度を調整したり、複数の解像度を選択したりできます。</p> <p>これにより、配達確認を確認するユーザーは、携帯電話、タブレット、モニターの様々なサイズなど、様々なデバイスでのコンテンツの表示を確認できます。</p> <p>複数の解像度を選択した場合は、選択した解像度ごとに個別の配達確認が作成されます。</p> <p>ユーザーが配達確認にコメントする際、現在の画面の解像度がコメントに自動的に表示され、他のユーザーがコメントに関連付けられている解像度を認識できるようになります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブページを検索</td> 
      <td>（このオプションは、インタラクティブな配達確認には使用できません）。 Web サイトのページ間を移動するには、このオプションを選択します。 Web サイトは、メインページから最大 2 レベルまで拡張できます。 ページの URL を表示するには、ページにマウスを移動します。 配達確認するページのみを選択します。 選択した各ページは、デフォルトでは個々の配達確認として作成されます。または、 <strong>1 つの配達確認に結合</strong> 」オプションを使用します。</td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）配達確認の共有、自動ワークフローの追加、アクセス設定や購読設定など、高度な校正オプションを設定します。 これらのオプションの詳細については、次の記事を参照してください。

   * [内で配達確認を共有 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [で自動ワークフローを使用した配達確認の設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [配達確認のアクセスおよび購読設定を構成する](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. クリック **[!UICONTROL 完了]**.

   既存の URL 配達確認に新しいバージョンを追加する場合、元の配達確認または以前のバージョンに設定されたオプションは、このバージョンで維持されます。既存の URL 配達確認に新しいバージョンを追加する場合、元の配達確認または以前のバージョンで設定されたオプションは維持されます。

1. クリック **[!UICONTROL 配達確認を作成]**.

## インタラクティブコンテンツの配達確認を生成 {#generate-a-proof-for-interactive-content}

この機能を使用するには、Pro Workfront Plan 以降が必要です。 利用可能な様々なプランについて詳しくは、 [Workfront Plans](https://www.workfront.com/plans).

インタラクティブコンテンツについて詳しくは、 [インタラクティブコンテンツの配達確認の概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [インタラクティブコンテンツを URL として追加](#add-interactive-content-as-a-url)
* [インタラクティブコンテンツを ZIP ファイルとして追加](#add-interactive-content-as-a-zip-file)

### インタラクティブコンテンツを URL として追加 {#add-interactive-content-as-a-url}

インタラクティブな URL 配達確認を追加する方法について詳しくは、  [URL の配達確認を生成](#generate-a-proof-for-a-url).

### インタラクティブコンテンツを ZIP ファイルとして追加 {#add-interactive-content-as-a-zip-file}

1. .zip バンドルファイルを作成して、コンテンツを準備します。

   .zip バンドルファイルの仕様について詳しくは、 [ZIP ファイル内のインタラクティブコンテンツを校正用に準備する方法について](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) 記事内 [インタラクティブコンテンツの配達確認の概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 次のいずれかの操作を行って、新しい配達確認の作成を開始し、 [!UICONTROL 新しい配達確認] ページ：

   * 緑をクリック **[!UICONTROL 新しい配達確認]** 」ボタンをクリックします。
   * Adobe Analytics の **[!UICONTROL ダッシュボード]** 領域、内 **[!UICONTROL 概要]** タブで、 **[!UICONTROL 新しい配達確認]** リンク。

   * ドロップゾーン（エンタープライズ機能）を使用して送信します。

1. Adobe Analytics の **[!UICONTROL 新しい配達確認]** 表示されるページで、インタラクティブ.zip バンドルを **[!UICONTROL ファイルを追加]** 領域。

1. （オプション）配達確認の共有、自動ワークフローの追加、アクセスおよび購読の設定など、高度な校正オプションを設定します。 これらのオプションの詳細については、次の記事を参照してください。

   * [内で配達確認を共有 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * 記事内
   * [配達確認のアクセスおよび購読設定を構成する](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. クリック **[!UICONTROL 配達確認を作成]**.

   Workfrontは.zip バンドルの配達確認の生成を開始します。 バンドルサイズに応じて、ドキュメントのアップロードに関する遅延時間は異なります。 サイズの大きいファイルは、生成に時間がかかります。 ページから移動すると、Workfrontは引き続きファイルを生成します。 最大ファイルアップロードサイズは 4GB です。

   配達確認が生成されたら、 **[!UICONTROL 配達確認に移動]** ボタンをクリックして配達確認を開きます。
