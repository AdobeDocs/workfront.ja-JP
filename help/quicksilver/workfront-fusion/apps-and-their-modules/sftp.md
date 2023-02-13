---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP モジュール
description: この [!DNL Adobe Workfront Fusion SFTP] モジュールを使用すると、選択したフォルダーやサブフォルダーのファイルの変更を監視したり、新しいファイルを目的のフォルダーにアップロードしたり、既にフォルダー内にある既存のファイルを変更、削除したり、ファイル権限を変更したりできます。
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# SFTP モジュール

この [!DNL Adobe Workfront Fusion] SFTP モジュールを使用すると、選択したフォルダーまたはサブフォルダー内のファイルの変更を監視したり、新しいファイルを目的のフォルダーにアップロードしたり、既にフォルダー内にある既存のファイルを変更、削除したり、ファイル権限を変更したりできます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

で SFTP を使用するには [!DNL Workfront Fusion]の場合、SFTP アカウント ( [!DNL GoDaddy] web ホスティング )。

## SFTP の接続先 [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

SFTP アカウントをに接続するには、以下を実行します。 [!DNL Workfront Fusion] ターゲットホストと、モジュールの [!UICONTROL 接続の作成] ダイアログ。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続名 ]</td> 
   <td> <p> SFTP 接続の名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ホスト ]</p> </td> 
   <td> <p>接続する SFTP サーバーのホスト名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ポート ] </td> 
   <td> <p>SFTP サーバーポートを入力します。 例：22</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 認証タイプ ]</p> </td> 
   <td> <p>SFTP サーバーへの接続に使用する認証方法を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL ユーザー名とパスワード ]</strong>:資格情報を入力します。</li> 
     <li> <p><strong>[!UICONTROL ユーザー名とキー ]</strong>:ユーザー名と秘密鍵/証明書を入力します</p> <p>自己署名済み証明書を使用して TLS を使用する場合は、クライアント側の認証を使用するために秘密鍵をアップロードするか、証明書（P12 または PFX ファイル）をアップロードします。 クライアント側の証明書認証を使用している場合は、ここに CA 証明書を入力できます。</p> <p>[!DNL Workfront Fusion] は、ここで指定したデータ（ファイル、パスワード）を保持または保存しません。 ファイルとパスワードは、秘密鍵/証明書を抽出する場合にのみ使用します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

接続情報を入力したら、 **[!UICONTROL 続行]** 接続を確立するために使用します。

## [!UICONTROL SFTP] モジュールとそのフィールド

設定時に [!UICONTROL SFTP] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!UICONTROL SFTP] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### トリガー

#### [!UICONTROL フォルダ内のファイルを監視する]

指定されたフォルダ内でファイルが作成または変更された場合に、詳細を含むファイルを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>監視するフォルダーを入力またはマッピングします。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>バッファサイズ [B]</td> 
   <td> <p> バッファサイズをバイト単位で入力します。 値は、サーバーから転送されるチャンクのサイズを定義します。 値が大きすぎると、一部のサーバーで問題が発生したり、ファイルが破損したりする場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返されるファイルの最大数 ]</td> 
   <td> <p> 最大ファイル数を設定 [!DNL Workfront Fusion] は、1 サイクルでと連携します</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダ内のサブフォルダを監視する]

指定されたフォルダー内でフォルダーが作成または変更された場合に、詳細を含むフォルダーを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>監視するフォルダーを入力またはマッピングします。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返されるファイルの最大数 ]</td> 
   <td> <p> フォルダーの最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間に戻ります。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

#### [!UICONTROL フォルダーのコンテンツのリスト]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 表示 ] </td> 
   <td> <p>ファイル、フォルダ、またはその両方を取得するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>リストに表示するファイルまたはフォルダを含むフォルダを入力またはマップします。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索 ] </td> 
   <td> <p>検索語句を入力またはマッピングします。 例えば、ファイル拡張子が.txt のファイルを検索する場合は、「 <code>.txt</code>検索するファイルの名前を入力またはマッピングすることもできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 並べ替え基準 ]</td> 
   <td> <p> ファイル名、サイズ、最終アクセス日、最終変更日のどれで結果を並べ替えるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 並べ替え順 ] </td> 
   <td> <p>結果を昇順または降順で返すかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL モジュールが結果を返さない場合でも、ルートの実行を続行します ]</p> </td> 
   <td>結果が返されない場合にこのモジュールがシナリオを停止しないようにするには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返される結果の最大数 ]</td> 
   <td> <p> 結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間に戻ります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ダウンロード]

このモジュールは、指定されたフォルダのファイルを一覧表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL バッファーサイズ [B]]</td> 
   <td> <p> バッファサイズをバイト単位で入力します。 値は、サーバーから転送されるチャンクのサイズを定義します。 値が大きすぎると、一部のサーバーで問題が発生したり、ファイルが破損したりする場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>リストに表示するファイルまたはフォルダを含むフォルダを入力またはマップします。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索 ] </td> 
   <td> <p>検索語句を入力またはマッピングします。 例えば、ファイル拡張子が.txt のファイルを検索する場合は、「 <code>.txt</code>検索するファイルの名前を入力またはマッピングすることもできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 並べ替え基準 ]</td> 
   <td> <p> ファイル名、サイズ、最終アクセス日、最終変更日のどれで結果を並べ替えるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 並べ替え順 ]</td> 
   <td> <p> 結果を昇順または降順で返すかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL モジュールが結果を返さない場合でも、ルートの実行を続行します ]</p> </td> 
   <td>結果が返されない場合にこのモジュールがシナリオを停止しないようにするには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返される結果の最大数 ]</td> 
   <td> <p> 最大ファイル数を設定 [!DNL Workfront Fusion] は、1 サイクルの間に戻ります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの取得]

このモジュールは、ファイルのデータを含むファイルの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL バッファーサイズ [B]]</td> 
   <td> <p> バッファサイズをバイト単位で入力します。 値は、サーバーから転送されるチャンクのサイズを定義します。 値が大きすぎると、一部のサーバーで問題が発生したり、ファイルが破損したりする場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルパス ] </td> 
   <td> <p>ファイルのパスを入力します。 絶対パスを指定できます。例えば、 <code>/home/user/file.txt</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのアップロード]

このモジュールを使用すると、SFTP サーバーにファイルをアップロードできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>既存のフォルダをファイルの保存場所として指定します。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td> <p> [!UICONTROLDropbox] / [!UICONTROL ファイルの取得 ] など、以前のモジュールからソースファイルをマッピングします。 また、ファイル名とファイルデータを入力またはマッピングすることもできます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 権限 ]</p> </td> 
   <td> <p>ファイルまたはフォルダーに対する必要な権限を設定します。 chmod パラメータを使用します。 例： <code>777 </code>または <code>-rwxrwxrwx</code>.</p> <p>chmod の詳細については、 <a href="https://ss64.com/bash/chmod.html">chmod ドキュメント</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル名の変更]

ファイルの名前を変更します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルパス ]</td> 
   <td> <p> 名前を変更するファイルのパスを入力します。 絶対パスを指定できます。例えば、 <code>/home/user/file.txt</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新しいファイル名 ]</td> 
   <td> <p> ファイル拡張子を含む、ファイルの新しい名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの移動]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルパス ]</td> 
   <td> <p> 移動するファイルのパスを入力します。 絶対パスを指定できます。例えば、 <code>/home/user/file.txt</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新規フォルダー ]</td> 
   <td> <p> ファイルの新しい場所へのパスを入力します。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの削除]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルパス ]</td> 
   <td> <p> 削除するファイルのパスを入力します。 絶対パスを指定できます。例えば、 <code>/home/user/file.txt</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの権限を更新]

ファイルの権限を変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルパス ]</td> 
   <td> <p> 移動するファイルのパスを入力します。 絶対パスを指定できます。例えば、 <code>/home/user/file.txt</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 権限 ]</p> </td> 
   <td> <p>必要なファイル権限を設定します。 chmod パラメータを使用します。 例： <code>777 </code>または <code>-rwxrwxrwx</code>.</p> <p>パターンに一致する必要があります <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>chmod の詳細については、 <a href="https://ss64.com/bash/chmod.html">chmod ドキュメント</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーを作成]

指定された場所に新しいフォルダを作成します。

>[!NOTE]
>
>フォルダーが既に存在する場合、モジュールはエラーをスローします。 フローを中断せずに続行するには、エラーを検出するためにエラーハンドラルートをモジュールに接続し、 [!UICONTROL 再開] フローを続行するための命令。 エラーハンドラールートのアタッチについては、 [でのエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). エラーハンドラーのルートについて詳しくは、 [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>新しいフォルダの保存場所として既存のフォルダを指定します。 絶対パスを指定できます。例えば、 <code>/home/user/file.txt</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー名 ]</td> 
   <td> <p> フォルダー名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 権限 ]</p> </td> 
   <td> <p>目的のフォルダー権限を設定します。 chmod パラメータを使用します。 例： <code>777 </code>または <code>-rwxrwxrwx</code>.</p> <p>パターンに一致する必要があります <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>chmod の詳細については、 <a href="https://ss64.com/bash/chmod.html">chmod のマニュアルページ</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの削除]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td>
   <td> <p>SFTP アカウントの接続先 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP の接続先 [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> 削除するフォルダーのパスを指定します。 絶対パスを指定できます。例えば、 <code>/home/user/</code>. また、ログインしたユーザーの特定のフォルダーを指す相対パス ( 例： <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
