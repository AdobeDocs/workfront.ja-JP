---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Docs モジュール
description: Adobe Workfront Fusion [!DNL Google Docs] モジュールを使用すると、 [!DNL Google Docs] および [!DNL Google Docs] （[!DNL G Suite] ユーザー用）。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '4090'
ht-degree: 0%

---

# [!DNL Google Docs] モジュール

この [!DNL Adobe Workfront Fusion] [!DNL Google Docs] モジュールを使用すると、 [!DNL Google Docs] および [!DNL Google Docs] ( [!DNL G Suite] ユーザー )。

を使用するには [!DNL Google Docs] と [!DNL Adobe Workfront Fusion]の場合、 [!DNL Google] アカウント 次の条件を満たさない場合、 [!DNL Google] アカウントはまだ、 [!DNL Google] アカウントヘルプページ。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用する [!DNL Google Docs] モジュールを使用するには、Googleアカウントが必要です。

## [!DNL Google Docs] モジュールとそのフィールド

設定時に [!DNL Google Docs] モジュール [!UICONTROL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Docs] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### ドキュメント

* [[!UICONTROL 監視ドキュメント]](#watch-documents)
* [[!UICONTROL ドキュメントのリスト]](#list-documents)
* [[!UICONTROL ドキュメントのコンテンツを取得する]](#get-content-of-a-document)
* [[!UICONTROL ドキュメントの作成]](#create-a-document)
* [[!UICONTROL テンプレートからドキュメントを作成する]](#create-a-document-from-a-template)
* [[!UICONTROL 文書に段落を挿入する]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL ドキュメントに画像を挿入する]](#insert-an-image-to-a-document)
* [[!UICONTROL 画像を新しい画像に置き換える]](#replace-an-image-with-a-new-image)
* [[!UICONTROL ドキュメント内のテキストの置換]](#replace-text-in-a-document)
* [[!UICONTROL ドキュメントのダウンロード]](#download-a-document)
* [[!UICONTROL ドキュメントの削除]](#delete-a-document)

#### [!UICONTROL 監視ドキュメント]

このトリガーモジュールは、選択したフォルダーで新しいドキュメントが作成または変更された場合に、ドキュメントの詳細を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドキュメントを監視 ]</td> 
   <td> <p style="color: #000000;">作成日（[!UICONTROL 作成日別）ドキュメントと変更日（[!UICONTROL 変更日別）ドキュメントのどちらで視聴するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>監視するドライブの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>作成または変更したドキュメントを監視するフォルダを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>作成または変更したドキュメントを監視するフォルダを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>監視する共有ドライブを選択します。</p> <p>注意：この [!DNL Google Shared Drive] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>1 回の実行サイクルで返されるドキュメントの最大数をWorkfront Fusion で設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメントのリスト]

このアクションモジュールは、選択したフォルダーからドキュメントのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>ドキュメントの一覧表示元のドライブの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>ドキュメントを一覧表示するフォルダを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>ドキュメントを一覧表示するフォルダを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>ドキュメントの一覧を表示する共有ドライブを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>ドキュメントの最大数を設定 [!DNL Workfront Fusion] は 1 回の実行サイクルでを返します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメントのコンテンツを取得する]

このアクションモジュールは、指定されたドキュメントを取得します。

権限の拡張が必要になる場合があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドキュメントのコンテンツの取得 ]</td> 
   <td> <p>ドキュメントのドキュメント ID をマッピングするか、ドロップダウンメニューから手動でドキュメントを選択するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>取得するドキュメントが含まれているドライブの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>取得するドキュメントを含むフォルダーを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>取得するドキュメントを含むフォルダーを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>取得するドキュメントが含まれている共有ドライブを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フィルター ]</p> </td> 
   <td> <p>モジュールの出力で返すオブジェクトを選択します。</p> 
    <ul> 
     <li>[!UICONTROL 画像 ] （デフォルト）</li> 
     <li>[!UICONTROL 図面 ]</li> 
     <li>[!UICONTROL グラフ ]</li> 
    </ul> <p>メモ:  <p>これらのオブジェクトのさらなるマッピングについては、このモジュールの出力で（[!UICONTROL inlineObjects] ではなく） [!UICONTROL Inline Objects Array] 値を使用してください。</p> <p>[!UICONTROL Inline Objects Array] オブジェクトは、ドキュメント内での表示と同じ順序で並べ替えられます。 これにより、それ以上の処理が容易になります。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメントの作成]

このアクションモジュールを使用すると、選択したフォルダーに新しいドキュメントを作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>ドキュメントの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンテンツ ]</td> 
   <td> <p>ドキュメントのコンテンツを入力します。 HTMLがサポートされています。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>ドキュメントを作成するドライブの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>ドキュメントを作成するフォルダを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>ドキュメントを作成するフォルダを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>ドキュメントを作成する共有ドライブを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ヘッダーの挿入 ]</td> 
   <td> <p> ヘッダーをドキュメントに挿入し、ヘッダーのテキストを入力またはマッピングするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フッターを挿入 ] </td> 
   <td> <p>フッターをドキュメントに挿入し、ヘッダーのテキストを入力またはマッピングするには、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テンプレートからドキュメントを作成する]

このアクションモジュールは、既存のテンプレートドキュメントのコピーを作成し、任意のタグを置き換えます。 また、このモジュールでは、画像を URL で新しい画像に置き換えることもできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL テンプレートからドキュメントを作成 ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL マッピングによる ]</strong> <br>ドキュメントテンプレートをマッピングするには、このオプションを選択します。</li> 
     <li><strong>[!UICONTROL ドロップダウン別 ]</strong> <br>このオプションを選択して、ドロップダウンメニューからドキュメントテンプレートを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>テンプレートが配置されているドライブのタイプを選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>テンプレートが配置されているフォルダーを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>テンプレートが配置されているフォルダーを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>テンプレートが配置されている共有ドライブを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 値 ]</p> </td> 
   <td> <p>変数の代わりに新しいドキュメントに入力する値を入力します。</p> 
    <ul> 
     <li><strong>[!UICONTROL タグ ]</strong> <br>ドキュメントテンプレートに含まれるタグを入力します。 使用しない <code>&#123;&#123;&#125;&#125;</code>. 例：use <code>name</code> の代わりに <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL 置換された値 ]</strong><br>タグの値を入力します。</li> 
    </ul> <p>例えば、<code> &#123;&#123;name&#125;&#125;</code> 変数は、ここに名前フィールドとして表示されます。ここでは、次のような値を挿入できます。 <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 画像の置換 ]</p> </td> 
   <td> <p>現在の画像を置き換える [!UICONTROL 画像オブジェクト ID] および [!UICONTROL 画像 URL] へのリンクを入力します。</p> <p>注意：画像 ID を取得するには、[!UICONTROL Get a Document] モジュールを使用します。このモジュールでは、ID が配列 [!UICONTROL Inline Object Array] に含まれています。</p> <p>ALT テキストを [!DNL Google] 文書。 </p> <p>ALT テキストを [!DNL Google Docs] 画像：</p> 
    <ol> 
     <li value="1">画像を右クリックします。</li> 
     <li value="2">「 [!UICONTROL ALT text] 」オプションを選択します。</li> 
     <li value="3">「[!UICONTROL タイトル ]」フィールドに [!UICONTROL ALT テキスト ] を入力し、「[!UICONTROL OK]」をクリックします。</li> 
    </ol> <p>ALT テキストを画像に追加すると、ALT テキストが括弧内のフィールド名に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイトル ] </td> 
   <td> <p>新しいドキュメントの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>テンプレートが配置されているドライブのタイプを選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>ドキュメントを作成するフォルダーを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>ドキュメントを作成するフォルダーを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>ドキュメントを作成する共有ドライブを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文書に段落を挿入する]

このアクションモジュールは、既存のドキュメントに新しい段落を追加または挿入します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドキュメントを選択 ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL マッピングによる ]</strong> <br>ドキュメントをマッピングするには、このオプションを選択します。</li> 
     <li><strong>[!UICONTROL ドロップダウン別 ]</strong> <br> このオプションを選択して、ドロップダウンメニューからドキュメントを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>段落を追加するドライブの種類を選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>段落を追加するドキュメントの場所を選択し、そのドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>段落を追加するドキュメントの場所を選択し、そのドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>段落を追加するドキュメントがある共有ドライブを選択し、そのドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 段落を挿入 ]</p> </td> 
   <td> <p>新しいテキストをドキュメントに挿入する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 場所の指定による ]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL インデックス別 ]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL インデックス ]</strong> </p> <p>テキストを挿入するインデックス番号を入力します。 [!UICONTROL Get a Document] モジュールを使用して、インデックス番号を取得できます。</p> <p>ドキュメント内のすべての文字（非表示も含む）を表示するには、[!UICONTROL 表示 ] アドオンを使用します。 アドオンは、[!UICONTROL Add-ons] / [!UICONTROL Get add-ons] にあります。 [!UICONTROL Show] を検索し、[!UICONTROL Show] アドオンをインストールします。</p> </li> 
         <li> <p><strong>[!UICONTROL 挿入されたテキスト ]</strong> </p> <p>ドキュメントに挿入するテキストを入力します。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL セグメント ID 別 ]</strong> </p> <p>テキストコンテンツを挿入するヘッダーとフッターを選択し、挿入するテキストを対応するフィールドに入力します。</p> <p>ヘッダーまたはフッターに既にテキストが含まれている場合は、新しいテキストが既存のテキストの前に追加されます。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL ドキュメントの本文にを追加する方法 ]</strong> </p> <p>文書の本文コンテンツの末尾に入力したテキストを追加します。</p> <p>新しい段落のスタイルは、現在の挿入インデックスの段落から、リストや箇条書き記号を含むコピーされます。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL セグメントの末尾にを追加する（ヘッダーおよびフッター）]</strong> </p> <p>テキストコンテンツを挿入するヘッダーとフッターを選択し、挿入するテキストを対応するフィールドに入力します。</p> <p>ヘッダーまたはフッターに既にテキストが含まれている場合は、新しいテキストが既存のテキストの後に追加されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 追加テキスト ]</td> 
   <td>ドキュメントに追加するテキストを入力またはマッピングします</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメントに画像を挿入する]

このアクションモジュールは、URL からドキュメントに画像を挿入します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドキュメントを選択 ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL マッピングによる ]</strong> <br>ドキュメントテンプレートをマッピングするには、このオプションを選択します。</li> 
     <li><strong>[!UICONTROL ドロップダウン別 ]</strong> <br> このオプションを選択して、ドロップダウンメニューからドキュメントを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>イメージを追加するドライブの種類を選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>画像を追加するドキュメントの場所のフォルダを選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>画像を追加するドキュメントの場所のフォルダを選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>画像を追加するドキュメントが存在する共有ドライブを選択し、ドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 画像の挿入 ]</p> </td> 
   <td> <p>新しい画像をドキュメントに挿入する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 場所の指定による ]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL インデックス別 ]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL インデックス ]</strong> </p> <p>画像を挿入するインデックス番号を入力します。 [!UICONTROL Get a Document] モジュールを使用して、[!UICONTROL Index number] を取得できます。</p> <p>ドキュメント内のすべての文字（非表示も含む）を表示するには、[!UICONTROL 表示 ] アドオンを使用します。 アドオンは、[!UICONTROL Add-ons] / [!UICONTROL Get add-ons] にあります。 [!UICONTROL Show] を検索し、[!UICONTROL Show] アドオンをインストールします。</p> </li> 
         <li> <p><strong>[!UICONTROL 画像 URL]</strong> </p> <p>ドキュメントに挿入する画像の URL を入力します。</p> <p>最大画像サイズは 50 MB です。 25 メガピクセルを超えないようにする必要があります。 PNG、JPEG、またはGIF形式のみがサポートされます。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL セグメント ID 別 ]</strong> </p> <p>画像を挿入するヘッダーとフッターを選択し、対応するフィールドに画像 URL を入力します。</p> <p>最大画像サイズは 50 MB です。 画像は 25 メガピクセル以下にする必要があります。 PNG、JPEG、またはGIF形式のみがサポートされます。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL ドキュメントの本文にを追加する方法 ]</strong> </p> <p>ドキュメントの本文コンテンツの最後に特定の画像を追加します。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL セグメントの末尾にを追加する（ヘッダーおよびフッター）]</strong> </p> <p>画像を挿入するヘッダーとフッターを選択し、挿入する画像 URL を対応するフィールドに入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 高さの大きさ（ポイント単位）/幅の大きさ（ポイント単位）]</p> </td> 
   <td> <p>挿入する画像のサイズを定義します。 縦横比は維持されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 画像を新しい画像に置き換える]

このアクションモジュールは、既存の画像を置き換えます。 元の画像の縦横比は維持されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドキュメントを選択 ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL マッピングによる ]</strong> <br>ドキュメントテンプレートをマッピングするには、このオプションを選択します。</li> 
     <li><strong>[!UICONTROL ドロップダウン別 ]</strong> <br> このオプションを選択して、ドロップダウンメニューからドキュメントを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>イメージを置き換えるドキュメントの種類を選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>画像を置き換えるドキュメントが存在するフォルダを選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>画像を置き換えるドキュメントが存在するフォルダを選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>画像を置き換えるドキュメントが存在する共有ドライブを選択し、ドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 画像 URL]</p> </td> 
   <td> <p>既存の画像を置き換える新しい画像の URL を入力またはマッピングします。</p> <p>画像は、ドキュメント内での表示順に表示されます。 例： <code>Body: Image No. 1</code> はドキュメント内の最初の画像です。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメント内のテキストの置換]

このアクションモジュールは、ドキュメント内のテキストを置き換えます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドキュメントを選択 ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL マッピングによる ]</strong> <br>ドキュメントテンプレートをマッピングするには、このオプションを選択します。</li> 
     <li><strong>[!UICONTROL ドロップダウン別 ]</strong> <br> このオプションを選択して、ドロップダウンメニューからドキュメントを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>テキストを追加するドライブの種類を選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>テキストを追加するドキュメントの場所を選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>テキストを追加するドキュメントの場所を選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>テキストを追加するドキュメントの場所の共有ドライブを選択し、ドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL テキストの置換 ]</p> </td> 
   <td> <p>置き換える各テキストを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 置き換える古いテキスト ]</strong> </p> <p>置き換えるテキストを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL 挿入する新しいテキスト ]</strong> </p> <p>新しいテキストを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメントのダウンロード]

このアクションモジュールは、選択したドキュメントを変換およびダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>ダウンロードするドキュメントが存在するドライブの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>ダウンロードするドキュメントが存在するフォルダを選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>ダウンロードするドキュメントが存在するフォルダを選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>ダウンロードするドキュメントが存在する共有ドライブを選択し、ドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL の種類 ] </p> </td> 
   <td> <p>ダウンロードするドキュメントのターゲットファイル形式を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドキュメントの削除]

このアクションモジュールは、ドキュメントを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>削除するドキュメントが存在するドライブの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>削除するドキュメントが存在するフォルダを選択し、そのドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>削除するドキュメントが存在するフォルダを選択し、そのドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>削除するドキュメントが存在する共有ドライブを選択し、ドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 共有ドライブ ]</td> 
   <td> <p>ダウンロードするドキュメントが含まれているドライブを選択し、ドキュメントを選択します。 このオプションは、 [!DNL Google Docs] 「 [!UICONTROL ドライブを選択 ] 」フィールドで、以下の操作を実行します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドキュメント ID]</td> 
   <td> <p> 1 つ以上の画像を置き換えるドキュメントを選択またはマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)
* [[!UICONTROL ドキュメント内のすべてのリンクをクリック可能にする]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>相対パスを入力 <code>https://docs.googleapis.com/</code>. 例: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> リクエストクエリ文字列を入力します。</p> </td> 
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

**例：** 次の API 呼び出しは、Googleドキュメント内の指定されたドキュメントの詳細を取得します。

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**メソッド:**

[!UICONTROL GET]

![](assets/api-call-example.png)

取得したドキュメントの詳細は、モジュールの「出力」の下にあります。 [!UICONTROL バンドル] > [!UICONTROL 本文].

![](assets/api-output.png)

#### [!UICONTROL ドキュメント内のすべてのリンクをクリック可能にする]

このアクションモジュールは、ドキュメント内のすべてのリンクを検索し、クリック可能にします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドキュメント内のすべてのリンクを作成 ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL マッピングによる ]</strong> <br>ドキュメントテンプレートをマッピングするには、このオプションを選択します。</li> 
     <li><strong>[!UICONTROL ドロップダウン別 ]</strong> <br> このオプションを選択して、ドロップダウンメニューからドキュメントを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>リンクをクリック可能にするドライブの種類を選択します。 このオプションは、前のフィールドで [!UICONTROL ドロップダウン別 ] を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL マイドライブ ]</strong> </p> <p>リンクをクリック可能にするドキュメントの場所を選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 自分と共有</strong> </p> <p>リンクをクリック可能にするドキュメントの場所を選択し、ドキュメントを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共有ドライブ ]</strong> ( [!DNL G Suite] ユーザーのみ )</p> <p>[!UICONTROL ドメイン管理者アクセスを使用 ] するかどうかを選択します。 [!UICONTROL はい ] を選択すると、ドメイン管理者として要求が発行され、要求者が管理者である共有ドライブがすべて返されます。</p> <p>リンクをクリック可能にするドキュメントが存在する共有ドライブを選択し、ドキュメントを選択します。</p> <p>注意：この [!DNL Google Docs] オプションを選択し、 [!DNL G Suite] ユーザー、エラー <code>[400] Invalid Value</code> が返されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 共有ドライブ ]</td> 
   <td> <p>リンクを更新するドキュメントが含まれているドライブを選択し、ドキュメントを選択します。 このオプションは、 [!DNL Google Docs] 「 [!UICONTROL ドライブを選択 ] 」フィールドで、以下の操作を実行します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドキュメント ID]</td> 
   <td> <p> リンクを更新するドキュメントを選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
