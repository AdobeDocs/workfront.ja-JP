---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Illustrator および InDesign 向け Workfront 拡張機能の使用
description: Workfront 拡張機能を使用すると、Adobe Illustrator および Adobe InDesign で保存および作成したデジタルコンテンツを Workfront に書き出すことができます。これにより、ドキュメントのレビューと承認プロセスが高速化されます。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '3076'
ht-degree: 81%

---

# Illustrator および InDesign 向け Workfront 拡張機能の使用

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Illustrator および InDesign 用の Workfront 拡張機能を、[アップデートされた Creative Cloud プラグイン](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md)に置き換えます。2022年後半以降、この拡張機能はサポートされなくなり、現状のままで利用できるようになります。

Workfront 拡張機能を使用すると、Adobe Illustrator および Adobe InDesign で保存および作成したデジタルコンテンツを Workfront に書き出すことができます。これにより、ドキュメントのレビューと承認プロセスが高速化されます。

Workfront 拡張機能は、Adobe Creative Cloud 2017 以降の以下のアプリケーションでサポートされています。

* InDesign
* Illustrator
* Photoshop

  >[!NOTE]
  >
  >新しい [Adobe Workfront for Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) プラグインの使用をお勧めします。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在： Pro 以上</p>
   または
   <p>新規：任意のプラン</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在：作業以上</p>
   または
   <p>新規：標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Workfront ライセンスに加えて、Adobe Creative Cloud ライセンスが必要です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>操作するオブジェクトへのアクセス権を編集します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Illustrator または InDesign から Workfront 拡張機能にログイン {#log-in-to-workfront-extension-from-illustrator-or-indesign}

サポートされているアドビアプリケーションの 1 つから Workfront にログインすると、サポートされているすべてのアドビアプリケーションにログインすることになります。

1. Workfront 拡張機能を使用するアドビアプリケーションに移動します。

   それぞれのサポートされているアプリケーションでサポートされている形式のリストについては、この記事にある[サポートされている書き出しファイルの形式](#supported-exported-file-formats)を参照してください。

1. **ウィンドウ**／**拡張機能**／Workfront をクリックします。

1. （オプション）Workfront パネルを、アドビアプリケーションで表示する位置にドラッグします。
1. プロンプトに従って Workfront にログインします。

   >[!NOTE]
   >
   >* Workfront は OAuth 2.0 を使用して Adobe Creative Cloud に接続します。OAuth 2.0 ほとんどの web ベースの統合で、ユーザーの認証と承認に使用される安全な標準です。
   >* 次の項目を入力するよう求められた場合、 [ドメインまたはホスト] Workfrontアカウントに次の形式で入力します。`yourCompany'sDomain.my.workfront.com`. 会社のドメインは通常、会社の名前です。

   プロジェクトが現在のステータスの場合は、割り当てられた作業アイテムのリストが表示されます。リストが表示されない場合は、Workfront にログインします。

   個人用タスクは「**プロジェクトなし**」の下に表示されます。

## Workfront プロジェクト、タスク、イシューにファイルをアップロード {#upload-a-file-to-a-workfront-project-task-or-issue}

コンピューターのファイルシステムからファイルをアップロードしたり、Adobe Creative Cloud アプリケーションで現在開いているファイルを Workfront プロジェクト、タスク、イシューに書き出したりすることができます。 

Adobe Creative Cloud からファイルをアップロードまたは書き出す際は、以下の点を考慮してください。

* アクセスレベルで、Workfront へのドキュメントのアップロードを許可する必要があります。詳しくは、[ドキュメントへのアクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)を参照してください。
* ドキュメントを目的の項目にアップロードするには権限が必要です。詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。
* ファイルは、選択した Workfront オブジェクトのドキュメントエリアにアップロードされます。
* Adobe Creative Cloud アプリケーションからメインメニュー ![](assets/main-menu-icon.png) のドキュメントエリアにドキュメントを書き出すことはできません。

以下の節では、以下について説明します。

* [ファイルをアップロード](#upload-a-file)
* [現在開いているファイルを Illustrator または InDesign で書き出す](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Illustrator または InDesign から新しいバージョンのファイルをアップロード](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### ファイルのアップロード {#upload-a-file}

Adobe Creative Cloud アプリケーションを離れることなく、プロジェクト、タスクまたはイシューにファイルをアップロードできます。

1. Adobe Creative Cloudアプリケーションを開いたときにWorkfront拡張機能が表示されない場合は、 **ウィンドウ** > **拡張機能** > **Workfront**.

   プロジェクトが現在のステータスの場合は、割り当てられた作業項目のリストが表示されます。 リストが表示されない場合は、Workfront にログインします。

   個人用タスクは、「**プロジェクトなし**」の下に表示されます。

1. ファイルのアップロード先のプロジェクト、タスクまたはイシューの名前をクリックします。

   これを検索するには、「**検索**」ボックスに名前を入力し、「**検索**」ボックスの右側にあるドロップダウンメニューから「**プロジェクト**」、「**タスク**」または「**イシュー**」を選択します。作業アイテムの名前が一覧に表示されない場合は、**Enter** キーを押して、表示アクセス権のあるすべての Workfront 項目を検索します。

1. クリック **選択** Workfront拡張機能の右下隅。
1. 「**クリックして形式を選択**」ドロップダウンメニューで、Workfront でファイルを保存する形式をクリックします。

   それぞれのサポートされているアプリケーションでサポートされている形式のリストについては、この記事にある[サポートされている書き出しファイルの形式](#supported-exported-file-formats)を参照してください。

1. （条件付き）ファイルをアップロードする作業項目にドキュメントフォルダが含まれている場合、 **クリックしてドキュメントフォルダを選択** 「 」フィールドで「 」をクリックし、 **選択**.

1. 「**ローカルファイルをアップロード**」をクリックします。
1. Adobe Analytics の **ファイルを開く** 」ボックスで、ファイルシステム内のファイルを探し、 **開く**.

1. （オプション）ファイルの新しい名前を入力します。

   ![](assets/rename-file-uploading.png)

1. 「**アップロード**」をクリックします。

   Workfrontで、選択したプロジェクト、タスクまたはイシューのドキュメント領域にドキュメントが表示されます。

1. （オプション）ドキュメントの名前をクリックすると、そのドキュメントの詳細ページが Workfront で開きます。

   Workfront が新しいブラウザータブで開きます。

### Illustrator または InDesign で現在開いているファイルを書き出し {#export-a-file-currently-open-in-illustrator-or-indesign}

1. サポートされている Adobe Creative Cloud アプリケーションで、Workfront に書き出すファイルを開きます。
1. Workfront拡張機能が表示されない場合は、「 **ウィンドウ** > **拡張機能** > **Workfront**.

   プロジェクトが現在のステータスの場合は、割り当てられた作業項目のリストが表示されます。 リストが表示されない場合は、Workfront にログインします。

   個人タスクは、**プロジェクトなし**&#x200B;の下に一覧表示されます。

1. ファイルを書き出すプロジェクト、タスクまたはイシューの名前をクリックします。

   これを検索するには、「**検索**」ボックスに名前を入力し、「**検索**」ボックスの右側にあるドロップダウンメニューから「**プロジェクト**」、「**タスク**」または「**イシュー**」を選択します。作業アイテムの名前が一覧に表示されない場合は、**Enter** キーを押して、表示アクセス権のあるすべての Workfront アイテムを検索します。

1. **クリックして形式を選択**&#x200B;ドロップダウンメニューで、Workfront にファイルを保存する形式をクリックします。

   それぞれのサポートされているアプリケーションでサポートされている形式のリストについては、この記事にある[サポートされている書き出しファイルの形式](#supported-exported-file-formats)を参照してください。

1. （条件付き）ファイルをアップロードする作業アイテムにドキュメントフォルダーが含まれている場合、「**クリックしてドキュメントフォルダーを選択**」フィールドでドキュメントフォルダーを選択し、「**選択**」をクリックします。
1. （オプション）ドキュメントの名前を変更するには、ドキュメント名をクリックし、新しい名前を入力します。

   ![](assets/rename-doc-exporting.png)

1. 「**書き出し**」をクリックします。

   ドキュメントが Workfront に正常に書き出されたことを確認するメッセージが表示されます。

   Workfront で、指定したオブジェクトのドキュメントエリアにドキュメントが一覧表示されます。

1. （オプション）ドキュメントの名前をクリックすると、Workfront でそのドキュメントにアクセスできます。

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront が新しいブラウザータブで開きます。

### Illustrator または InDesign から新しいバージョンのファイルをアップロード {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. サポートされているアドビアプリケーションで作業中のファイルを、新しいバージョンのファイルとして Workfront に書き出す場合は、そのファイルをそのアドビアプリケーションで開きます。
1. Workfront拡張機能が表示されない場合は、「 **ウィンドウ** > **拡張機能** > **Workfront**.

   プロジェクトが現在のステータスの場合は、割り当てられた作業項目のリストが表示されます。 リストが表示されない場合は、Workfront にログインします。

   個人用タスクは、「**プロジェクトなし**」の下に表示されます。

1. 既存のドキュメントが表示されているプロジェクト、タスク、またはイシューの名前をクリックします。

   これを検索するには、「**検索**」ボックスに名前を入力して、「**検索**」ボックスの右側にあるドロップダウンメニューから、**プロジェクト**、**タスク**、または&#x200B;**イシュー**&#x200B;を選択します。作業アイテムの名前がリストに表示されない場合は、**Enter** キーを押して、自身が表示アクセス権を持つすべての Workfront 項目を検索します。

   プロジェクト、タスク、またはイシューにアップロードされたすべてのドキュメントは、Adobe アプリケーションからアップロードされたかどうかに関係なく、リストに表示されます。

1. **クリックして形式を選択**&#x200B;ドロップダウンメニューで、Workfront で保存するファイルの形式をクリックします。

   これは、Adobe アプリケーションで開いているファイルを書き出す場合に必要です。サポートされている各アプリケーションでサポートされている形式のリストについて詳しくは、この記事にある[サポートされている書き出しファイル形式](#supported-exported-file-formats)を参照してください。

1. Adobe アプリケーションで開いているファイルを、選択した Workfront ドキュメントの新しいバージョンとして書き出す場合は、「**書き出し**」をクリックします。

   または

   選択した Workfront ドキュメントの新しいバージョンとして、コンピューターのファイルシステムからファイルをアップロードする場合は、**ローカルファイルをアップロード**&#x200B;をクリックして、表示されるボックス内でファイルを見つけ、**開く**&#x200B;をクリックして、次に&#x200B;**アップロード**&#x200B;をクリックします。

1. （オプション）ドキュメントの名前をクリックして、そのドキュメントの新しいバージョンを Workfront で表示します。

   >[!NOTE]
   >
   >Workfront のドキュメントの名前はデフォルトで入力され、編集できません。また、新しいバージョンとしてアップロード、または書き出すファイルの名前も変更されません。
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## IllustratorまたはInDesignからのWorkfrontドキュメントに対するコメント {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Adobe アプリケーション内の Workfront ドキュメントに直接コメントを追加できます。Workfront では、コメントは、ドキュメントの更新エリアと、ドキュメントが保存されている Workfront 項目の更新エリアに表示されます。

1. サポートされているアドビのアプリケーションのうちの 1 つを開きます。
1. Workfront拡張機能が表示されない場合は、「 **ウィンドウ** > **拡張機能** > **Workfront**.

   プロジェクトが現在のステータスの場合は、割り当てられた作業項目のリストが表示されます。 リストが表示されない場合は、Workfront にログインします。

   個人用タスクは、**プロジェクトなし**&#x200B;の下に表示されます。

1. 既存のドキュメントが表示されているプロジェクト、タスク、またはイシューをクリックします。

   これを検索するには、「**検索**」ボックスに名前を入力して、「**検索**」ボックスの右側にあるドロップダウンメニューから、**プロジェクト**、**タスク**、または&#x200B;**イシュー**&#x200B;を選択します。作業アイテムの名前が一覧に表示されない場合は、**Enter** キーを押して、表示アクセス権のあるすべての Workfront 項目を検索します。

1. 既存のドキュメントの名前をクリックし、 **選択** Workfront拡張機能の右下隅。
1. 次をクリック： **コメント** 」タブで、更新をボックスに入力します。

1. （オプション）他の Workfront ユーザーまたはチームをコメントに含めるには、「**担当者またはチームに通知**」ボックス内にユーザーまたはチームの名前の入力を開始し、ドロップダウンリストに表示される名前をクリックします。
1. （オプション）ドキュメントの承認をリクエストするには、 **承認リクエストを実行**.
1. 「**更新**」をクリックします。

   ドキュメントの「更新」タブにアップデートが投稿されます。コメントに含めたWorkfrontユーザーにはアプリ内通知が送信されます。また、Workfrontの設定によっては、が電子メール通知を受け取る場合もあります。

   Workfront内での通知について詳しくは、 [アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

   メール通知の受信について詳しくは、[Adobe Workfront 通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## Illustrator または InDesign からのドキュメントの承認のリクエスト

Workfront ドキュメントの承認をアドビアプリケーションから直接リクエストできます。

以下のエンティティからドキュメントの承認をリクエストできます。

* Workfront ユーザー
* Workfront アカウントを持たない外部ユーザー

以下の方法で、Adobe アプリケーションからドキュメントの承認をリクエストできます。

* 承認者をドキュメントに添付します。
* ドキュメントにコメントを付け、コメントを作成する際にその人に通知し、ドキュメントに承認者として添付することで、

  ドキュメントにコメントを作成する際の承認リクエストについて詳しくは、 [IllustratorまたはInDesignからのWorkfrontドキュメントに対するコメント](#comment-on-a-workfront-document-from-illustrator-or-indesign) 」を参照してください。

アドビアプリケーションからドキュメントの承認をリクエストするには、以下の操作を実行します。

1. サポートされているアドビのアプリケーションのうちの 1 つを開きます。
1. Workfront拡張機能が表示されない場合は、「 **ウィンドウ** > **拡張機能** > **Workfront**.

   プロジェクトが現在のステータスの場合は、割り当てられた作業項目のリストが表示されます。 リストが表示されない場合は、Workfront にログインします。

   個人用タスクは、「**プロジェクトなし**」の下に表示されます。

1. 既存のドキュメントが表示されているプロジェクト、タスク、またはイシューをクリックします。次に、既存のドキュメントの名前をクリックします。

   これを検索するには、「**検索**」ボックスに名前を入力し、「**検索**」ボックスの右側にあるドロップダウンメニューから、**プロジェクト**、**タスク**&#x200B;または&#x200B;**イシュー**&#x200B;を選択します。作業アイテムの名前がリストに表示されない場合は、**Enter** キーを押して、自身が表示アクセス権を持つすべての Workfront 項目を検索します。

1. 既存のドキュメントの名前、Workfront 拡張機能の右下隅にある「**選択**」の順にクリックします。
1. 「**承認**」タブをクリックします。
1. 承認者を追加するには、**名前の入力を開始ボックス**&#x200B;で、次のいずれかの操作を行います。

   * 承認者の名前を入力し、リストに表示されたら選択します。

     ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * 外部ユーザーのメールアドレスを入力します。

1. 「**承認をリクエスト**」をクリックします。

   コメントに含めるか承認者として追加したWorkfrontユーザーは、アプリ内通知を受け取り、Workfrontの設定に応じて、電子メール通知も受け取る場合があります。\
   外部ユーザーはメール通知を受け取り、そのメールから承認について決定を下すことができます。

   Workfront の通知について詳しくは、[アプリ内通知の表示および管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)を参照してください。メール通知の受信について詳しくは、[Adobe Workfront の通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## Illustrator や InDesign からプルーフを生成 {#generate-a-proof-from-illustrator-or-indesign}

組織が自動ワークフローテンプレートを使用している場合は、アドビのアプリケーションで作成したドキュメントのプルーフを、アプリケーションから移動せずに生成できます。プルーフの作成について詳しくは、[プルーフの作成](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md)を参照してください。自動ワークフローテンプレートについて詳しくは、[自動ワークフローの概要](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)の[自動ワークフローテンプレート](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate)を参照してください。

1. サポートされているアドビのアプリケーションのうちの 1 つを開きます。
1. Workfront 拡張機能が表示されない場合は、**ウィンドウ**／**拡張機能**／Workfront をクリックします。

   プロジェクトが現在のステータスの場合は、割り当てられた作業項目のリストが表示されます。 リストが表示されない場合は、Workfront にログインします。

   個人用タスクは、**プロジェクトなし**&#x200B;の下に表示されます。

1. ドキュメントがすでに Workfront にアップロードされている場合は、ドキュメントがリストされている Workfront 拡張機能でプロジェクト、タスクまたはイシューを選択し、ドキュメントの名前をクリックします。

   または

   この記事の [Workfront のプロジェクト、タスクまたはイシューにファイルをアップロード](#upload-a-file-to-a-workfront-project-task-or-issue)の節の説明に従って、アドビのドキュメントを Workfront のオブジェクトにアップロードし、続いてドキュメントの名前をクリックします。

1. **クリックして形式を選択**&#x200B;ドロップダウンメニューで、Workfront で保存したいファイルの形式をクリックします。

   この後の手順でプルーフ機能を有効にすると、一部の形式が使用できなくなります。詳しくは、この記事の[サポートされている書き出しファイル形式](#supported-exported-file-formats)を参照してください。

1. 「**新規プルーフとしてアップロード**」をクリックして有効にします。
1. ユーザーがドキュメントをレビューするときに使用する&#x200B;**ワークフローテンプレート**&#x200B;を選択します。

   Workfrontの管理者が、自動ワークフローテンプレートを設定します。詳しくは、 [自動ワークフローテンプレートの作成と管理](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). 質問がある場合は、管理者にお問い合わせください。

   1. ワークフローテンプレートの各ステージに、少なくとも 1 人の&#x200B;**新規受信者**&#x200B;を追加します。

      名前を入力し、表示されるドロップダウンリストに表示されたら、その名前を選択します。

   1. 追加する受信者ごとに、**プルーフの役割**&#x200B;と&#x200B;**メールアラート**&#x200B;の頻度を指定します。

   1. （オプション） **電子メール通知** 「 」セクションで、追加したすべての配達確認受信者に対して、配達確認に関するオプションのカスタムメッセージを含む e メール通知を送信するかどうかを選択します。

1. 「**プルーフを作成**」をクリックします。

   プルーフ作成プロセスの進捗状況を表示できます。生成が完了すると、アラートが表示されます。プルーフを作成したタスクを開くと、そこにタスクが表示されます。

## Illustrator や InDesign から移動せずに新しいバージョンのプルーフをアップロード

1. プルーフを含む既存のドキュメント、右下隅にある「**選択**」の順にクリックします。
1. 「**新しいプルーフバージョンとしてアップロード**」をクリックして有効にします。
1. （オプション）ユーザーが新しいバージョンをレビューするときに使用する&#x200B;**ワークフローテンプレート**&#x200B;を選択します。

   別のテンプレートを選択しない場合、以前のバージョン用に選択されたテンプレートは有効なままになります。また、以前のバージョンのテンプレートを変更した場合、その変更内容は新しいバージョンに対して有効になります。

   Workfrontの管理者が、自動ワークフローテンプレートを設定します。詳しくは、 [自動ワークフローテンプレートの作成と管理](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). 質問がある場合は、管理者にお問い合わせください。

   1. ワークフローテンプレートの各ステージに、少なくとも 1 人の&#x200B;**新規受信者**&#x200B;を追加します。

      名前を入力し、表示されるドロップダウンリストに表示されたら、その名前を選択します。

   1. 追加する受信者ごとに、**プルーフの役割**&#x200B;と&#x200B;**メールアラート**&#x200B;の頻度を指定します。
   1. （オプション） **電子メール通知** 「 」セクションで、追加したすべての配達確認受信者に対して、配達確認に関するオプションのカスタムメッセージを含む e メール通知を送信するかどうかを選択します。

1. 「**新しいプルーフバージョンを作成**」をクリックします。

   プルーフ作成プロセスの進捗状況を表示できます。生成が完了すると、アラートが表示されます。プルーフを作成したタスクを開くと、そこにタスクが表示されます。

## Workfront Extension からログアウトします。

1. Adobe・アプリケーションで、 **ウィンドウ** > **拡張機能** > **Workfront**.

1. 右側のパネルの右上隅にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックします。

1. （オプション）「 **フィードバック** 簡単な調査を開き、Workfront for Adobe Creative Cloudに関するフィードバックを送信します。
1. 「**ログアウト**」をクリックします。\
   ログイン画面が表示されます。ログインについて詳しくは、[Illustrator または InDesign から Workfront Extension にログイン](#log-in-to-workfront-extension-from-illustrator-or-indesign)を参照してください。

## サポートされている書き出し済みファイル形式 {#supported-exported-file-formats}

* [Adobe InDesign でサポートされている書き出し済みファイル形式](#supported-exported-file-formats-for-adobe-indesign)
* [Adobe Illustrator でサポートされている書き出し済みファイル形式](#supported-exported-file-formats-for-adobe-illustrator)

### Adobe InDesign でサポートされている書き出し済みファイル形式 {#supported-exported-file-formats-for-adobe-indesign}

Workfront では、ファイルを InDesign から Workfront に書き出すために、次のファイル形式をサポートしています。

* EPS - Encapsulated PostScript
* EPUB - 固定レイアウトの電子文書
* EPUB - リフロー可能な電子公開 &#42;
* HTML - HyperText マークアップ言語
* IDML - InDesign マークアップ言語 &#42;
* JPG、JPEG - Joint Photographic Experts Group
* PDF - Adobe Portable Document File
* PNG - Portable Network Graphics
* SWF - Flash Player &#42;
* XML - 拡張可能なマークアップ言語 &#42;

&#42; このファイル形式は、**新しいプルーフをアップロード**&#x200B;が有効になっている場合は使用できません（このオプションについて詳しくは、この記事の [Illustrator または InDesign からプルーフを生成](#generate-a-proof-from-illustrator-or-indesign)を参照）。**新しいプルーフをアップロード**&#x200B;を有効にする前にこのファイル形式が既に選択されている場合、システムはファイル形式を PDF に変更します。リストから別の形式を選択できます。

### Adobe Illustrator でサポートされている書き出し済みファイル形式 {#supported-exported-file-formats-for-adobe-illustrator}

Workfront では、ファイルを Illustrator から Workfront に書き出すために、次のファイル形式をサポートしています。

* DWG - AutoCAD Drawing、AutoCAD Interchange File &#42;
* JPG、JPEG - Joint Photographic Experts Group
* PNG - Portable Network Graphics
* PSD- Photoshop Document
* SWF - Flash Player &#42;
* TIFF - Tagged Image File Format

&#42; このファイル形式は、**新しいプルーフをアップロード**&#x200B;が有効になっている場合は使用できません（このオプションについて詳しくは、この記事の [Illustrator または InDesign からプルーフを生成](#generate-a-proof-from-illustrator-or-indesign)を参照）。**新しいプルーフをアップロード**&#x200B;を有効にする前にこのファイル形式が既に選択されている場合、システムはファイル形式を PNG に変更します。リストから別の形式を選択できます。
