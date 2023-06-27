---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Azure Active Directory モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Azure] Active Directory を使用し、複数のサードパーティのアプリケーションやサービスに接続します。
author: Becky
feature: Workfront Fusion
exl-id: ac966231-251e-44de-be61-00afa5ece3fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 1%

---

# [!DNL Azure Active Directory] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Azure Active Directory]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用する [!DNL Azure Active Directory] モジュールの場合、 [!DNL Azure Active Directory] アカウント

## [!DNL Azure Active Directory] モジュールとそのフィールド

設定時に [!DNL Azure Active Directory] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Azure Active Directory] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL レコードを監視] （スケジュール済み）

このポーリング（スケジュール設定）トリガーモジュールは、選択したオブジェクトのレコードが、前回のスケジュールされた実行以降に作成された場合に、シナリオを実行します。 [!DNL Azure Active Directory]. また、レコードまたはレコードに関連付けられたすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値も返します。この情報は、シナリオの後続モジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure Active Directory] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ]</td> 
   <td>ユーザーレコードとグループレコードのどちらを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最大レコード数 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL レコードの読み取り]](#read-record)
* [[!UICONTROL レコードを作成]](#create-record)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、 [!DNL Azure Active Directory].

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

のレコードにアクセスするのに十分な権限が必要です [!DNL Azure Active Directory] この情報を取得するために。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure Active Directory] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>[!UICONTROL User] レコードと [!UICONTROL Group] レコードのどちらを読み取るかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>一意の [!DNL Azure Active Directory] モジュールが読み取るレコードの ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成]

このアクションモジュールは、新しいユーザーまたはグループレコードを作成します。

レコードのタイプを指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure Active Directory] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>[!UICONTROL User] レコードと [!UICONTROL Group] レコードのどちらを読み取るかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL その他のフィールド ]</td> 
   <td>新しいレコードの値を設定するには、次のフィールドに入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Azure Active Directory] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Azure Active Directory] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure Active Directory] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>パスを入力またはマッピングします <code>https://graph.microsoft.com/{version}/{resource}?{query-parameters}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> </td> 
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
 </tbody> 
</table>

### 検索

* [ユーザーの検索](#search-users)
* [ユーザー/グループデルタの検索](#search-usersgroups-delta)

#### [!UICONTROL ユーザーの検索]

この検索モジュールは、 [!DNL Azure Active Directory] 指定した検索クエリに一致する この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure Active Directory] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 検索条件 ]</td> 
   <td> <p>検索に使用する条件を入力します。</p> <p>「[!UICONTROL $filter]」など、使用するパラメーターについて詳しくは、 <a href="https://docs.microsoft.com/en-us/graph/query-parameters">クエリパラメータを使用して応答をカスタマイズする</a> 内 [!DNL Microsoft] API ドキュメント。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL レコードの最大数 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ユーザー/グループデルタの検索]

この検索モジュールは、 [!DNL Azure AD] 作成、更新または削除された この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure Active Directory] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
