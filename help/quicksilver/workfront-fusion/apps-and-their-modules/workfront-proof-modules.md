---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Workfront Proof モジュール
description: 内、 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Workfront Proof]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 8764de907f49260908911ca393c1173b66dbb065
workflow-type: tm+mt
source-wordcount: '2934'
ht-degree: 0%

---

# [!DNL Workfront Proof] モジュール

内、 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Workfront Proof]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

これは、現在、内での検証がサポートされていないタスクを実行する必要がある場合に役立ちます。 [!DNL Workfront] または [!DNL Workfront Proof]：特定のイベントに基づいて配達確認を更新したり、配達確認の受信者を検索したりする場合などです。

The [!DNL Workfront Proof] コネクタは、組織で使用可能なアクティブなアプリの数に対してカウントされません。 すべてのシナリオ ( たとえ [!DNL Workfront Proof] アプリの場合、組織の合計シナリオ数に対してカウントします。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] モジュールとそのフィールド

設定時に [!DNL Workfront Proof] モジュール、 [!DNL Workfront Fusion] に、以下のフィールドを示します。 これらと共に、 [!DNL Workfront Proof] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [であるモジュールから別のモジュールに情報をマッピングします。 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

* [配達確認を見る](#watch-proofs)
* [PDF概要の監視](#watch-for-pdf-summary)
* [[!UICONTROL 配達確認アクティビティを監視]](#watch-proof-activity)

#### [!UICONTROL 配達確認を見る]

このスケジュール済みトリガーモジュールは、誰かが配達確認を作成または決定する際にシナリオを実行します。

このモジュールは、指定した期間に見つかったすべてのレコードのリストと、そのレコードのタイプを返します。 また、指定したフィールドの値も返されます。 モジュールで配達確認に関する決定が見つかった場合は、以前の値と現在の値の両方が個別のフィールドに含まれます。 この情報は、シナリオの後続のモジュールにマッピングできます。

この処理は、指定した定期的なスケジュール間隔で実行されます。

で配達確認または配達確認にアクセスするのに十分な権限が必要です。 [!DNL Workfront Proof] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">レコードタイプ</td> 
   <td>次のタイプを選択： [!DNL Workfront Proof] レコードを作成します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">出力</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">制限</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL PDF概要の監視]

このインスタントトリガーモジュールは、誰かが配達確認のPDF概要を作成したときにシナリオを実行します。

このモジュールには Webhook が必要です。

このモジュールは、配達確認に関連付けられたすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 また、PDFの概要に対する新しいイベントの購読を作成し、ペイロードで送信される「pdf_url」属性からコンテンツを出力します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>既存の Webhook を選択するか、新しい Webhook を作成できます。 詳しくは、 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">のインスタントトリガー（Web フック） [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 配達確認アクティビティを監視]

このトリガーモジュールは、配達確認で指定されたアクティビティが発生した場合にシナリオを実行します。

このモジュールは、配達確認に関連付けられたすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 また、イベントの概要に関する新しいPDFサブスクリプションを作成し、 `pdf_url` 属性がペイロードで送信されました。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アクティビティタイプ ]</td> 
   <td>新しい決定（[!UICONTROL 配達確認 ] のステータスの変更を含む）を監視するか、配達確認のステータスの全体的な変更のみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 配達確認を作成]](#create-proof)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL 配達確認をダウンロード]](#download-proof)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL リクエストPDFの概要]](#request-pdf-summary)
* [[!UICONTROL 配達確認を更新]](#update-proof)
* [[!UICONTROL ファイルをアップロード]](#upload-file)

#### [!UICONTROL 配達確認を作成]

このアクションモジュールは、で新しい配達確認または新しいバージョンの配達確認を作成します。 [!DNL Workfront Proof].

新しいバージョンを作成する場合は、新しい配達確認のパラメーターと、ソースの配達確認を指定します。

モジュールは、新しい配達確認または配達確認のバージョンの ID を返します。この情報は、シナリオの後続のモジュールでマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認の種類 ]</td> 
   <td> <p>作成する配達確認に基本ワークフローと [!UICONTROL 自動ワークフロー ] のどちらを使用するかを指定します。</p> <p>次に、選択した配達確認タイプに対して表示するフィールドに入力します。 例えば、「[!UICONTROL Automated Workflow]」を選択した場合は、 <strong>[!UICONTROL ワークフローステージ ]</strong> フィールドを使用してステージを設定します。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 元のファイルのダウンロードを許可 ]</td> 
   <td>配達確認の作成元となった元のファイルをダウンロードするかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic 配達確認ビューア ]</td> 
   <td>従来の配達確認ビューアを使用するかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL すべてのファイルを 1 つの配達確認に結合 ]</td> 
   <td>すべてのファイルを 1 つの複数ページの配達確認に組み合わせるには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新しい配達確認のバージョンを作成 ]</td> 
   <td>モジュールで既存の配達確認の新しいバージョンを作成する場合は、このオプションを選択します。 次に、 <strong>[!UICONTROL 既存の配達確認 ID]</strong> 配達確認の一意の ID を表示、マッピングまたは入力するフィールド。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタムリンクラベル ]</td> 
   <td>カスタム配達確認リンクのラベルを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタムリンク URL]</td> 
   <td>カスタムリンクの URL を入力またはマッピングします。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 購読者向けのデフォルトの電子メール通知 ]</td> 
   <td>次のいずれかの数値を入力して、配達確認に使用する次のデフォルトの E メール通知設定を指定します。
    <ul>
     <li><strong>1</strong>  — すべての新しいコメントと返信</li>
     <li><strong>2</strong>  — コメントへの返信</li>
     <li><strong>3</strong>  — 日別概要</li>
     <li><strong>4</strong>  — 時間別サマリ</li>
     <li><strong>5</strong>  — 決定のみ</li>
     <li><strong>9</strong>  — 無効</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Excel 概要を無効にする ]</td> 
   <td>配達確認のコメントを Excel ファイルにダウンロードする機能を無効にするかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROLPDF概要を無効にする ]</td> 
   <td>配達確認のコメントを配達確認ファイルにダウンロードする機能を無効にするPDFを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 配信登録メールを無効にする ]</td> 
   <td>この配達確認の配信登録メールを無効にするかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 埋め込みプレーヤーを有効にする ]</td> 
   <td>この配達確認に埋め込まれたプレーヤーを有効にするかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 購読を有効にする ]</td> 
   <td>参加者でない人に対し、配達確認の購読を許可するかどうかを選択します。<br>このオプションを選択すると、この表で説明するように、購読者の「デフォルトの役割」も選択できます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 購読検証を有効にする ]</td> 
   <td>サブスクリプションの電子メール検証を有効にするかどうかを選択します。 このオプションが有効な場合、購読者は配達確認にアクセスするには、E メール内のリンクをクリックする必要があります。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL チーム URL を有効にする ]</td> 
   <td>作成した配達確認でチーム URL の表示と非表示を切り替えるかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ファイルハッシュ ] <span style="font-weight: normal;">または</span> [!UICONTROL ファイルハッシュ ]</td> 
   <td>配達確認または配達確認の作成元となるファイルの ID を追加します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ファイル名 ]</td> 
   <td>作成した配達確認のファイル名または名前を追加します。これは必須フィールドです。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 必要なすべての決定がおこなわれたら配達確認をロックする ]</td> 
   <td>作成された配達確認を、必要なすべての決定がおこなわれた後にロックするかどうかを指定します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL この配達確認について受信者に通知します ]</td> 
   <td>配達確認の作成時に受信者に通知するかどうかを指定するオプションを選択します。&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認名 ]</td> 
   <td>作成した配達確認の名前を入力します。これは必須フィールドです。 複数の配達確認の名前を区切るには、パイプ記号 (|) を使用します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認の所有者 ID]</td> 
   <td>配達確認の所有者の ID を入力またはマッピングします。 このフィールドを空白のままにすると、配達確認の所有者は現在のユーザーに設定されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference ID]</td> 
   <td>配達確認の参照 ID を入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 電子署名が必要 ]</td> 
   <td>電子署名の送信を、配達確認に関する決定を行った人に対して要求するかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ログインが必要です ]</td> 
   <td> <p>作成された配達確認にログインを必要とするかどうかを指定します。 </p> <p>これは、 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL 配達確認の設定 ]( [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 解像度 ID]</td> 
   <td>配達確認に使用する解像度の ID を入力します。 解決 ID のリストについては、 [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">API ドキュメント</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROLSWF]</td> 
   <td>配達確認のタイプをSWFします。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 表示 ] [ 項目 ]</td> 
   <td>各項目について、配達確認に表示するかどうかを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>配達確認を作成するワークスペースの ID を入力します。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 受信者 ]</td> 
   <td>作成した配達確認に必要な受信者の E メールアドレスを追加します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>配達確認を作成する期限を指定します。 次の日付形式を使用します。</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Workfront Proof] API. これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Workfront Proof] モジュール。

このモジュールは、ステータスコード、ヘッダーおよび本文を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL メソッド ]</td> 
   <td>API 呼び出しのアクションを設定します。 使用可能なアクションについては、 <a href="https://api.proofhq.com/">配達確認 API ドキュメント</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 本文 (XML)]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>注意：  <p>条件ステートメント ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL 配達確認をダウンロード]

このアクションモジュールは、ID を使用して識別する特定の配達確認のソースファイルをダウンロードします。

配達確認の ID を指定します。

このモジュールは、配達確認の作成に使用するソースファイルの内容を返します。この情報は、シナリオの後続のモジュールでマッピングできます。

のレコードにアクセスするのに十分な権限が必要です [!DNL Workfront Proof] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認 ID]</td> 
   <td> <p>[!UICONTROL 配達確認の詳細 ] ページにある、配達確認の一意の ID を入力します。 詳しくは、 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">で配達確認の詳細を管理 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、 [!DNL Workfront Proof].

配達確認の ID と、配達確認に必要な情報を指定します。

このモジュールは、配達確認用に選択したフィールドの値とタイプを返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

のレコードにアクセスするのに十分な権限が必要です [!DNL Workfront Proof] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td>配達確認、配達確認のコメントまたは配達確認のレビュー担当者のどれを読み取るかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>一意の [!DNL Workfront Proof] モジュールが読み取るレコードの ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リクエストPDFの概要]

このアクションモジュールは、の特定のPDFの配達確認の概要を要求します。 [!DNL Workfront Proof].

配達確認の ID を指定します。

モジュールは、PDFの概要情報を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

のレコードにアクセスするのに十分な権限が必要です [!DNL Workfront Proof] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認 ID]</td> 
   <td> <p>一意の [!DNL Workfront Proof] 配達確認の概要をリクエストするPDFの ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL コールバック URL]</td> 
   <td>PDFの概要を送信する URL を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

##### 考えられるエラー

* **エラー**: &quot;[!UICONTROL この要求を実行する権限がありません。 ステージには、少なくとも 1 人の受信者が含まれている必要があります。]&quot;
* **解決策**：自分が、ワークフローのステージに割り当てられた唯一のものではないことを確認します。 ワークフローのステージに別のユーザーを割り当てる必要があります。

#### [!UICONTROL 配達確認を更新]

このアクションモジュールは、 [!DNL Workfront Proof].

配達確認の ID とレコードのタイプ、および出力に含めるフィールドを指定します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

のレコードにアクセスするのに十分な権限が必要です [!DNL Workfront Proof] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認 ID]</td> 
   <td> <p>[!UICONTROL 配達確認の詳細 ] ページにある、配達確認の一意の ID を入力します。 詳しくは、 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">で配達確認の詳細を管理 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>配達確認を作成する期限を指定します。 次の日付形式を使用します。</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 購読者向けのデフォルトの電子メール通知 ]</td> 
   <td>配達確認で使用する、次のデフォルトの電子メール通知設定の中から、どれを選択します。
    <ul>
     <li> [!UICONTROL 新しいコメントと返信 ]</li>
     <li>[!UICONTROL コメントに返信 ]</li>
     <li>[!UICONTROL 日別概要 ]</li>
     <li> [!UICONTROL 時間別概要 ]</li>
     <li> [!UICONTROL 決定のみ ]</li>
     <li> [!UICONTROL 無効 ]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL デフォルトの役割 ]</td> 
   <td>配達確認のデフォルトの役割を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配信登録メールを無効にする ]</td> 
   <td>この配達確認の配信登録メールを無効にするかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 購読を有効にする ]</td> 
   <td>参加者でない人に対し、配達確認の購読を許可するかどうかを選択します。<br>このオプションを選択すると、この表で説明するように、購読者に対して [!UICONTROL デフォルトの役割 ] を選択することもできます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 購読検証を有効にする ]</td> 
   <td>サブスクリプションの電子メール検証を有効にするかどうかを選択します。 このオプションが有効な場合、購読者は配達確認にアクセスするには、E メール内のリンクをクリックする必要があります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チーム URL を有効にする ]</td> 
   <td>作成した配達確認でチーム URL の表示と非表示を切り替えるかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 必要なすべての決定がおこなわれたら配達確認をロックする ]</td> 
   <td>作成された配達確認を、必要なすべての決定がおこなわれた後にロックするかどうかを指定します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Message]</td> 
   <td>配達確認に付随するメッセージを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認 ID] </td> 
   <td>更新する配達確認の ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認名 ]</td> 
   <td>更新する配達確認の名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ログインが必要です ]</td> 
   <td> <p>作成された配達確認にログインを必要とするかどうかを指定します。 </p> <p>これは、 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL 配達確認の設定 ]( [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 次のようなバージョンを表示 ]</td> 
   <td>この配達確認の他のバージョンへのリンクを表示するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 件名 ]</td> 
   <td>配達確認の件名を入力またはマッピング</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをアップロード]

このアクションモジュールは、 [!UICONTROL 配達確認を作成] モジュール内 [!DNL Workfront Proof].

このモジュールは、アップロードされたファイルのハッシュ ID を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL 検索]](#search)
* [[!UICONTROL ワークフローテンプレートのリスト]](#list-workflow-templates)

#### [!UICONTROL 検索]

この検索モジュールは、 [!DNL Workfront Proof] 指定した検索クエリに一致する

このモジュールは、配達確認を検索する場合に、配達確認の ID を返します。 また、受信者を検索する場合は、受信者のユーザー ID、E メール、名前、位置および E メールエイリアスを返します。この情報は、シナリオの後続のモジュールでマッピングできます。

のレコードにアクセスするのに十分な権限が必要です [!DNL Workfront Proof] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>検索対象</td> 
   <td> <p>[!UICONTROL ] モジュールで検索するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 配達確認 ]</strong> </p> <p>検索する配達確認の「配達確認名」を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL 受信者 ]</strong> </p> <p>検索する受信者の電子メールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 結果セット ]</td> 
   <td>モジュールが <strong>[!UICONTROL 一致するすべてのレコード ]</strong> または <strong>[!UICONTROL 最初に一致したレコード ]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 並べ替え基準 ]</td> 
   <td>結果の並べ替えに使用するフィールドを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 並べ替え方向 ]</td> 
   <td> <p>結果を昇順または降順に並べ替えるかどうかを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークフローテンプレートのリスト]

この検索モジュールは、使用可能なすべてのワークフローテンプレートを一覧表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>接続方法については、 [!DNL Workfront Proof] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すテンプレートの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
