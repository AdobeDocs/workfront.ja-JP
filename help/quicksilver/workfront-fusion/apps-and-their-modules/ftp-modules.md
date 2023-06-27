---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP モジュール
description: FTP モジュールを使用すると、選択したフォルダー内のファイルの変更を監視したり、新しいファイルを目的のフォルダーにアップロードしたり、既にフォルダー内にある既存のファイルを変更または削除したりできます。
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# FTP モジュール

FTP モジュールを使用すると、選択したフォルダー内のファイルの変更を監視したり、新しいファイルを目的のフォルダーにアップロードしたり、既にフォルダー内にある既存のファイルを変更または削除したりできます。

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

を使用するには [Fusion アプリ] と [!DNL Workfront Fusion]に設定するには、FTP アカウントが必要です。

## FTP モジュールでの接続の作成 {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続名 ]</td> 
   <td> <p> FTP 接続の名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ホスト ] </td> 
   <td> <p>FTP サーバーのホスト名を入力します。 E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ポート ] </td> 
   <td> <p>FTP サーバーのポート番号を入力します。 E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ユーザー名 ] </td> 
   <td> <p>FTP アカウントのユーザー名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL パスワード ] </td> 
   <td> <p>FTP アカウントのパスワードを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>セキュア接続 (TLS) を使用</p> </td> 
   <td> <p>セキュリティで保護された接続を使用するかどうかを選択します。</p> <p style="font-weight: bold;">[!UICONTROL いいえ ]</p> <p>接続が保護されていません。</p> <p style="font-weight: bold;">[!UICONTROL 明示的な暗号化または暗黙的な暗号化 ]</p> <p>接続は、SSL を使用して保護されます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 許可されていない証明書を拒否 ]</p> </td> 
   <td> <p>FTP サーバー証明書を検証するには、このオプションを有効にします。 検証に失敗した場合、接続は作成されません。 検証に合格するには、証明書が次のいずれかの条件を満たしている必要があります。</p> 
    <ul> 
     <li>根で署名される <a href="https://en.wikipedia.org/wiki/Certificate_authority">認証局</a></li> 
     <li>中間認証局によって署名される ( 例： <a href="https://knowledge.digicert.com/solution/SO16297.html">証明書チェーンの仕組み</a> を参照してください )。 この場合、すべての中間証明書を FTP サーバーにインストールする必要があります。</li> 
     <li>[!UICONTROL 自己署名証明書 ] フィールドに入力された自己署名証明書である（以下を参照）</li> </ul>

このオプションが無効になっている場合、FTP サーバー証明書は検証されません。 このオプションを無効にしないことを強くお勧めします。無効にすると、接続が安全でなくなり、セキュリティ上のリスクが大きくなるからです。</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL 自己署名証明書 ]</p> </td> 
   <td> <p>次をクリック： <b>[!UICONTROL 抽出 ]</b> ボタンをクリックして、アップロードダイアログを開きます。</p> <p>自己署名済み証明書で TLS を使用するには、証明書をアップロードします。 [!DNL Workfront Fusion] は、ファイルやパスワードなど、指定したデータを保持または保存しません。 ファイルとパスワードは、証明書を抽出する場合にのみ使用します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP モジュールとそのフィールド

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

#### [!UICONTROL 監視ファイル]

[!UICONTROL 監視ファイル] は、FTP 用の唯一のトリガーモジュールです。 選択したフォルダーのファイルコンテンツを監視します。 このトリガーは、新しいファイルが指定のフォルダーに挿入されると実行されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>FTP アカウントへの接続を確立する手順については、 <a href="#create-a-connection" class="MCXref xref">FTP モジュールでの [!UICONTROL 接続の作成 ]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL フォルダー ]</p> </td> 
   <td> <p>監視するフォルダーを選択します。</p> <p><b>注意：</b> 1 つのシナリオにつき 1 つのフォルダーのみを使用できます。 サブフォルダーは無視されます。</p> <p><b>ヒント：</b> 複数のフォルダーを追跡するには、それぞれに個別のシナリオを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返されるファイルの最大数 ] </td> 
   <td> <p>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 値が大きすぎると、指定されたサードパーティサービス側（タイムアウト）で接続が中断される場合があります。 [!DNL Workfront Fusion] これに対する影響はありません。 サイクルの最大数に対しては、値を小さく設定して大きい値を定義するか、シナリオをより頻繁に実行することをお勧めします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 権限の変更]](#change-permissions)
* [[!UICONTROL フォルダーの作成]](#create-a-folder)
* [[!UICONTROL ファイルの削除]](#delete-a-file)
* [[!UICONTROL フォルダーの削除]](#delete-a-folder)
* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL フォルダー内のファイルのリスト]](#list-of-files-in-a-folder)
* [[!UICONTROL ファイルまたはフォルダの移動]](#move-a-file-or-folder)
* [[!UICONTROL アップロード] ファイル](#upload-a-file)

#### [!UICONTROL 権限の変更]

このアクションモジュールは、ファイルまたはフォルダの権限設定を変更します。

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL 接続 ]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP アカウントへの接続を確立する手順については、 <a href="#Create" class="MCXref xref" >FTP モジュールでの [!UICONTROL 接続の作成 ]</a> 」を参照してください。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL] の権限設定の変更</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>ファイルまたはフォルダの設定を変更するかどうかを選択します。</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL ファイルパス ]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">フォルダーまたはファイルへのファイルパスを入力またはマッピングします。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 権限 ]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>必要なファイルまたはフォルダーの権限を設定します。 chmod パラメータを使用します。 例： <code>777 </code>または <code>-rwxrwxrwx</code>.</p>
               <p>権限はのパターンに一致する必要があります <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL フォルダーの作成]

このアクションモジュールは、新しいフォルダーを作成します。

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL 接続 ]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP アカウントへの接続を確立する手順については、 <a href="#Create" class="MCXref xref" >FTP モジュールでの [!UICONTROL 接続の作成 ]</a> 」を参照してください。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL フォルダーパス ]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">新しいフォルダにファイルパスを入力またはマップします。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL 新しいフォルダー名 ]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>新しいフォルダの名前を入力またはマップします。</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL ファイルの削除]

指定したフォルダからファイルを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP アカウントへの接続を確立する手順については、 <a href="#Create" class="MCXref xref" >FTP モジュールでの [!UICONTROL 接続の作成 ]</a> 」を参照してください。</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>ファイルを削除する FTP フォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル名 ]</td> 
   <td> <p> ファイル名拡張子を含むファイル名を入力します。 例: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの削除]

このアクションモジュールは、指定されたフォルダを完全に削除します。

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL 接続 ]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">FTP アカウントへの接続を確立する手順については、 <a href="#Create" class="MCXref xref" >FTP モジュールでの [!UICONTROL 接続の作成 ]</a> 」を参照してください。</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL フォルダー ]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>ファイルを削除する FTP フォルダを選択します。</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL ファイルの取得]

FTP サーバーからファイルを取得し、それらのファイルをさらに処理できます ( 例えば、 [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>FTP アカウントへの接続を確立する手順については、 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 接続の作成</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルパス ]</td> 
   <td> <p> 取得するファイルのパスを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダー内のファイルのリスト]

ファイルやフォルダーの情報を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>FTP アカウントへの接続を確立する手順については、 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 接続の作成</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>検索する FTP フォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 表示 ] </td> 
   <td> <p>ファイルまたはフォルダに関する情報を取得するか、またはその両方を取得するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索 ] </td> 
   <td> <p>検索語句を入力します。 検索語句を入力しない場合、指定したフォルダーのすべてのファイルとフォルダーが取得されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返されるファイルの最大数 ]</td> 
   <td> <p> このモジュールで取得されるファイルの最大数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルまたはフォルダの移動]

このアクションモジュールは、ファイルまたはフォルダを別の場所に移動します。

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL 接続 ]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">FTP アカウントへの接続を確立する手順については、 <a href="#Create" class="MCXref xref" >FTP モジュールでの [!UICONTROL 接続の作成 ]</a> 」を参照してください。</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL 古いファイルパス ]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>ファイルの移動元のパスを入力します。 例: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL 新しいファイルパス ]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>ファイルの移動先のパスを入力します。 例: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL ファイルのアップロード]

FTP サーバーにファイルをアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td>FTP アカウントへの接続を確立する手順については、 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 接続の作成</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>ファイルのアップロード先の FTP フォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ] </td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 既存のファイルに追加 ]</td> 
   <td> <p>このオプションを有効にし、FTP サーバーに既にファイルが存在する場合は、ファイルの内容が既存のファイルに追加されます。 このオプションを有効にしないと、ファイルの内容が上書きされます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 存在しない場合のフォルダーの作成 ] </td> 
   <td> <p>このオプションを有効にし、「フォルダー」フィールドに入力したフォルダーが FTP サーバー上に存在しない場合、モジュールはフォルダーを作成します</p> </td> 
  </tr> 
 </tbody> 
</table>

## トラブルシューティング {#troubleshooting}

接続の作成中またはモジュールの操作中に FTP アプリで問題が発生した場合は、一般的な FTP クライアントの 1 つを使用して、同じ操作を試みて（例えば、接続やフォルダー内のファイルのリストを作成）ください。 を FTP クライアントに置き換えます。 FTP クライアントでも同じ問題が発生している場合は、FTP サーバーの設定が誤っている可能性があります。
