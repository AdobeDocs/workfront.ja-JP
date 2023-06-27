---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets モジュール
description: を使用 [!DNL Adobe Experience Manager Assets] コネクタ [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] アセットのアカウント、作成、アップロードおよび更新、およびフォルダーとアセットのコピーまたは移動をおこなう。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1544'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] モジュール

を使用 [!DNL Adobe Experience Manager Assets] コネクタ [!DNL Adobe Workfront Fusion]の場合、 [!DNL Adobe Experience Manager Assets] アセットのアカウント、作成、アップロードおよび更新、およびフォルダーとアセットのコピーまたは移動をおこなう。

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

* 次が必要です： [!DNL Adobe Experience Manager Assets] アカウントを使用してこれらのモジュールを使用します。
* を設定する必要があります [!UICONTROL サーバー間] 流れ [!DNL Adobe Developer console].

  の設定手順については、 [!UICONTROL サーバー間] 流れ [!DNL Adobe Developer console]を参照してください。 [サーバー側 API のアクセストークンの生成](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## 接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

の接続を作成するには、以下を実行します。 [!DNL Adobe Experience Manager Assets] モジュール：

1. クリック [!UICONTROL 追加] の横 [!UICONTROL 接続] ボックス

2. 作成する接続のタイプを選択します。

   * **[!DNL AEM Assets as a Cloud Service]**

     この設定には、 [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     この設定には、ユーザー名とパスワードが必要です。

3. 作成する接続のタイプのフィールドに入力します。

   の場合 [!DNL AEM Assets as a Cloud Service]を参照してください。 [接続の設定対象 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   の場合 [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]) を参照してください。 [接続の設定対象 [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. クリック **[!UICONTROL 続行]** 接続を保存し、モジュールに戻ります。


### 接続の設定対象 [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>これらのフィールドの情報は、設定の一環として生成されます [!UICONTROL サーバー間] 流れる [!DNL Adobe Developer Console]. これらの値は、設定の一環として生成されるサービス資格情報 JSON ファイルに含まれています。
>
>の設定手順については、 [!UICONTROL サーバー間] 流れる [!UICONTROL Adobe Developer Console]を参照してください。 [サーバー側 API のアクセストークンの生成](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL 接続名 ]</td>
                  <td>
                      <p>この接続の名前を入力</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL インスタンス URL （末尾にスラッシュを含まない）]</td>
                  <td>の URL を入力します。 [!DNL Adobe Experience Manager] インスタンス。 スラッシュを含めない <code>/</code> を返します。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL クライアント ID]</td>
                  <td>[!UICONTROL サーバー間 ] 設定で生成されたクライアント ID を入力します。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
                  <td>[!UICONTROL サーバー間 ] 設定で生成したクライアント秘密鍵を入力します。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL テクニカルアカウント ID]</td>
                  <td>テクニカルアカウントの ID を入力します。 これは、クライアント資格情報 JSON ファイルの「[!UICONTROL id]」フィールドです。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Org ID]</td>
                  <td class="">組織の ID を入力します。 これは、クライアント資格情報 JSON ファイルの「[!UICONTROL org]」フィールドです。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL メタスコープ ]</td>
                  <td>[!UICONTROL サーバー間 ] セットアップで生成されたメタスコープを入力します。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 秘密鍵 ]</td>
                  <td>[!UICONTROL サーバー間 ] セットアップで生成された秘密鍵を入力します。 秘密鍵を抽出するには、「[!UICONTROL 抽出 ]」をクリックし、抽出するファイルとファイルのパスワードを入力します。</td>
              </tr>
          </tbody>
      </table>


### 接続の設定対象 [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL 接続名 ]</td>
                <td>
                    <p>この接続の名前を入力</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL インスタンス URL （末尾にスラッシュを含まない）]</td>
                <td>の URL を入力します。 [!DNL Adobe Experience Manager] インスタンス。 スラッシュを含めない <code>/</code> を返します。</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL ユーザー名 ]</td>
                <td>のユーザー名を入力します。 [!DNL AEM Assets] この接続で使用されるアカウント。</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL パスワード ]</td>
                <td>のパスワードを入力 [!DNL AEM Assets] この接続で使用されるアカウント。</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] モジュールとそのフィールド

設定時に [!DNL Adobe Experience Manager Essentials] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Adobe Experience Manager Essentials] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL フォルダーまたはアセットのコピー]

このアクションモジュールは、フォルダーまたはアセットをAdobe Experience Manager Assets アカウント内の別の場所にコピーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>フォルダーとアセットのどちらをコピーするかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ] / [!UICONTROL アセット選択 ]</td> 
   <td>コピーするフォルダーまたはアセットを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 宛先パス ]</td> 
   <td>新しいフォルダーまたはアセットの場所を選択またはパスにマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コピーしたフォルダーの名前 ] / [!UICONTROL アセット ]</td> 
   <td>新しいフォルダーまたはアセットの名前を入力します。 に表示されるフォルダー名 [!DNL Adobe Experience Manager Assets] は元の名前と同じです。 ここで入力した名前は、新しいフォルダーまたはアセットの URL に表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 子をコピー ]</td> 
   <td>フォルダー内のサブフォルダーまたはアセットをコピーするには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 上書き ]</td> 
   <td>コピー先のフォルダーまたはアセットと同じ名前を持つ保存先のフォルダーまたはアセットを上書きするには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの作成]

このアクションモジュールは、フォルダーまたはアセットコメントを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL オブジェクトタイプ ]</td> 
   <td> <p>アセットに対してフォルダーとコメントのどちらを作成するかを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL フォルダー ]</p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p>[!UICONTROL 名前 ]</p> <p>フォルダーの名前を入力します。 この名前はファイルパスに含まれるので、スペースや他の文字を含めることはできません。 </p> </li> 
       <li> <p>[!UICONTROL タイトル ]</p> <p>名前の代わりに表示できるフォルダーのタイトルを入力します。</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL アセットコメント ]</p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p>[!UICONTROL アセットの選択 ]</p> <p>コメントを追加するアセットの ID を選択またはマッピングします。</p> </li> 
       <li> <p>[!UICONTROL コメント ]</p> <p>コメントのテキストを入力します。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの削除]

このアクションモジュールは、フォルダー、アセットまたはレンディションを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>フォルダー、アセット、レンディションのどれを削除するかを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL フォルダー ]</p> <p>パス内のフォルダーを選択して、削除するフォルダーを選択します。</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>パス内のフォルダーを選択してアセットを選択した後、削除するアセットを選択します。</p> </li> 
     <li> <p>[!UICONTROL レンディション ]</p> <p>パス内のフォルダーを選択して、レンディションを選択します。</p> <p>レンディションの名前を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL フォルダーの一覧を取得する]

このアクションモジュールは、既存のフォルダーとその子エンティティ（フォルダーまたはアセット）の表現を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>取得するフォルダーを選択またはマッピングします。 サブフォルダーをパスに追加するには、プラスアイコンをクリックし、サブフォルダーを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL カスタム API 呼び出しをおこなう]

このアクションモジュールは、 [!DNL Adobe Experience Manager Assets] API

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>次に関連するパスを入力： [!DNL Adobe Experience Manager] ベース URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ] </td> 
   <td> <p>リクエストクエリ文字列を入力します。 キーと値のペアごとに、 <b>[!UICONTROL 項目を追加 ]</b> [!UICONTROL キー ] と [!UICONTROL 値 ] を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL フォルダーまたはアセットの移動]

このアクションモジュールは、指定されたパスのアセットまたはフォルダーを新しい場所に移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>フォルダーを移動するかアセットを移動するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ] / [!UICONTROL アセット ]</td> 
   <td>移動するフォルダーまたはアセットを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 宛先パス ]</td> 
   <td>フォルダーまたはアセットの移動先を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 移動されたフォルダーの名前 ] / [!UICONTROL アセット ]</td> 
   <td>移動したフォルダーまたはアセットの新しい名前を入力します。 に表示されるフォルダー名 [!DNL Adobe Experience Manager Assets] は元の名前と同じです。 ここで入力した名前は、移動したフォルダーまたはアセットの URL に表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 上書き ]</td> 
   <td>コピー先のフォルダーまたはアセットと同じ名前を持つ保存先のフォルダーまたはアセットを上書きするには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの更新]

このアクションモジュールは、既存のレコードを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>アセットのメタデータとアセットのレンディションのどちらを削除するかを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL アセットメタデータ ]</p> 
      <ul> 
       <li> <p>メタデータを更新するアセットを選択します。</p> </li> 
       <li> <p>アセットの新しいタイトルを入力します。</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL アセットレンディション ]</p> 
      <ul> 
       <li> <p>レンディションを更新するアセットを選択します。</p> </li> 
       <li> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL アセットのアップロード]

このアクションモジュールは、 [!DNL Adobe Experience Manager Assets] アカウント

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Experience Manager Assets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">接続 [!DNL Adobe Experience Manager Assets] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 宛先 ]</td> 
   <td> <p>アセットをアップロードするフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td>ソースファイルの名前とデータを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
