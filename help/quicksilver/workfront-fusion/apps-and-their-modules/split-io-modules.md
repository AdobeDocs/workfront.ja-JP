---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Split.io モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Split.io]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# [!DNL Split.io] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Split.io]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Split.io] モジュールの場合、 [!DNL Split.io] アカウント

## 接続 [!DNL Split.io] から [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

次に、 [!DNL Split.io] 内部から直接アカウントを取得する [!DNL Split.io] モジュール。

1. 任意の [!DNL Split.io] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 接続の名前を入力します。
1. を入力します。 [!DNL Split.io] API キー。

   詳しくは、 [!DNL Split.io] API キー（を参照） [API キー](https://help.split.io/hc/en-us/articles/360019916211-API-keys) 内 [!DNL Split.io] ドキュメント。

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Split.io] モジュールとそのフィールド

設定時に [!DNL split.io] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL split.io] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL 分割を取得]](#get-split)
* [[!UICONTROL 環境での分割定義の取得]](#get-split-definition-in-environment)
* [[!UICONTROL 分割を作成]](#create-split)
* [[!UICONTROL 分割を削除]](#delete-split)
* [[!UICONTROL 環境での分割定義の作成]](#create-split-definition-in-environment)
* [[!UICONTROL 環境から分割定義を削除]](#remove-split-definition-from-environment)
* [[!UICONTROL 環境での部分更新分割定義]](#partial-update-split-definition-in-environment)
* [[!UICONTROL タグを関連付け]](#associate-tags)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL split.io] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL split.io] モジュール。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は、認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割を取得]

このアクションモジュールは、分割を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>取得する分割を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>取得する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境での分割定義の取得]

このアクションモジュールは、指定された環境から特定の分割定義を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>取得する分割定義を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 環境名または ID]</td> 
   <td>取得する分割定義を含む環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>分割定義を取得する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割を作成]

このアクションモジュールは、トラフィックタイプを指定して、組織内に新しい分割を作成します。

>[!NOTE]
>
>API はどの環境でも分割を設定しません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割を作成するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL トラフィックタイプ ID または名前 ]</td> 
   <td>分割の作成に使用するトラフィックタイプを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>作成する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割の説明 ]</td> 
   <td>作成する分割の [!UICONTROL split] の説明を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割を削除]

このアクションモジュールは、組織から分割を削除します。 これにより、すべての環境から分割定義の設定が自動的に解除されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割を削除するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>削除する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境での分割定義の作成]

このアクションモジュールは、特定の環境の分割定義を構成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割定義を作成するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 環境名または ID]</td> 
   <td>分割定義を作成する環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>定義を作成する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コメント ]</td> 
   <td>分割定義に追加するコメントを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ルール ]</td> 
   <td> <p>定義に追加するターゲティングルールごとに、 <b>[!UICONTROL 項目を追加 ]</b>」、「 」、「 」、「 」、「 」、「 」、「 」、「 」、「 」、「 」、「 」、「 」のいずれかを入力またはマッピングします。</p> <p>ターゲットルールについて詳しくは、 <a href="https://docs.split.io/reference#create-split-definition-in-environment">環境での分割定義の作成</a> 内 [!DNL Split.io] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL デフォルトルール ]</td> 
   <td> <p>他のルールの仕様を満たさないトラフィックに対して分割で使用するルールを入力またはマッピングします。</p> <p>ターゲットルールについて詳しくは、 <a href="https://docs.split.io/reference#create-split-definition-in-environment">環境での分割定義の作成</a> 内 [!DNL Split.io] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL デフォルトの処理 ]</td> 
   <td> <p>分割が強制終了した場合、または顧客がトラフィック配分に含まれていない場合に、分割で使用する処理を入力またはマッピングします。</p> <p>トリートメントについて詳しくは、 <a href="https://docs.split.io/reference#create-split-definition-in-environment">環境での分割定義の作成</a> 内 [!DNL Split.io] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>定義に追加する各処理に対して、 <b>[!UICONTROL 項目を追加 ]</b>処理を入力するか、マッピングします。</p> <p>トリートメントについて詳しくは、 <a href="https://docs.split.io/reference#create-split-definition-in-environment">環境での分割定義の作成</a> 内 [!DNL Split.io] ドキュメント。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境から分割定義を削除]

このアクションモジュールは、特定の環境の分割定義の構成を解除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割定義を削除するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 環境名または ID]</td> 
   <td>分割定義を削除する環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>定義を削除する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コメント ]</td> 
   <td>分割定義に追加するコメントを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境での部分更新分割定義]

このアクションモジュールは、特定の環境の分割定義を更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割定義を更新するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 環境名または ID]</td> 
   <td>分割定義を更新する環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割名 ]</td> 
   <td> <p>定義を更新する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンテンツを更新 ]</td> 
   <td> <p>更新する分割の各属性で、 <b>[!UICONTROL 項目を追加 ]</b> 必要な変更を入力またはマッピングします。</p> <p>詳しくは、 <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">環境での部分更新分割定義</a> 内 [!DNL Split.io] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コメント ]</td> 
   <td>分割定義に追加するコメントを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL タグを関連付け]

このアクションモジュールは、指定したオブジェクトにタグを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>タグを追加するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>タグを追加するオブジェクトの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL オブジェクトタイプ ]</td> 
   <td> <p>タグを追加するオブジェクトのタイプを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タグ ]</td> 
   <td> <p>追加するタグごとに、 <b>[!UICONTROL 項目を追加 ]</b> タグを入力するか、タグをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL ワークスペースを取得]](#get-workspaces)
* [[!UICONTROL 環境の取得]](#get-environments)
* [[!UICONTROL 分割を取得]](#get-splits)
* [[!UICONTROL 環境内の分割定義のリスト]](#list-split-definitions-in-an-environment)
* [[!UICONTROL トラフィックタイプの取得]](#get-traffic-types)

#### [!UICONTROL ワークスペースを取得]

この検索モジュールは、組織のワークスペースを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールで取得するワークスペースの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境の取得]

この検索モジュールは、環境のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストする環境を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割を取得]

この検索モジュールは、分割のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストに表示する分割を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールで取得する分割の最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境内の分割定義のリスト]

この検索モジュールは、特定の環境の分割定義のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストする分割定義を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 環境名または ID]</td> 
   <td>リストする分割定義を含む環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中にモジュールで取得する分割定義の最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL トラフィックタイプの取得]

この検索モジュールは、トラフィックタイプのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Split.io] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">接続 [!DNL Split.io] から [!UICONTROL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストに表示するトラフィックタイプを含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
