---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Cvent モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Cvent を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 1%

---

# [!DNL Cvent] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Cvent]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Cvent] モジュールの場合、 [!DNL Cvent] アカウント

## 接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>この [!DNL Cvent] モジュールは [!UICONTROL SOAP] API 接続を作成するには [!DNL Cvent]を使用する場合、次の点を確認する必要があります。
>
>* お持ちの [!UICONTROL SOAP] へのアクセス [!DNL Cvent] API
>* この [!DNL Workfront Fusion] IP アドレスが組織の組織に追加されてい許可リストます。
>
>  のリスト [!DNL Workfront Fusion] IP アドレス ( [アクセス用の IP アドレス [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


次に、 [!DNL Cvent] 内部から直接アカウントを取得する [!DNL Cvent] モジュール。

1. 任意の [!DNL Cvent] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 接続する地域を選択します。

   * [!UICONTROL 北米]
   * [!UICONTROL ヨーロッパ]
   * [!UICONTROL サンドボックス]

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Cvent] モジュールとそのフィールド

設定時に [!DNL Cvent] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Cvent] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#create-meeting-request)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL 招待者を登録]](#register-invitee)
* [[!UICONTROL 招待者を追加]](#add-invitee)
* [[!UICONTROL 連絡先の削除]](#delete-contact)
* [[!UICONTROL 連絡先の更新]](#update-contact)
* [[!UICONTROL 会議出席依頼を作成する]](#create-meeting-request)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Cvent] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Cvent] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

このモジュールは、ステータスコードと共に、API 呼び出しのヘッダーと本文を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本文 (XML)</td> 
   <td> <p>API 呼び出しの本文を入力またはマッピングします。 XML のみを含める必要があります。 モジュールは、認証ヘッダーを自動的に含めます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、特定のレコードに関する情報を読み取ります。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL レコードタイプ ]</p> </td> 
   <td>読み取るレコードの項目タイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 連絡先 ] / [!UICONTROL イベント ] / [!UICONTROL 招待 ID]</td> 
   <td> <p>読み取る項目の ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。 フィールドは、選択した項目タイプに基づいて使用できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 招待者を登録]

このアクションモジュールは、イベントの招待者を登録します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>招待者 ID</p> </td> 
   <td> <p>イベントに登録する招待者の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">イベント ID</td> 
   <td> <p>招待者を登録するイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 招待者を追加]

このアクションモジュールは、連絡先をイベントに招待します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 連絡先 ID]</p> </td> 
   <td> <p>イベントに追加する連絡先の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント ID]</td> 
   <td> <p>連絡先を追加するイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先の削除]

このアクションモジュールは、Cvent 内の 1 つの連絡先を削除します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 連絡先 ID]</td> 
   <td> <p>削除する連絡先の ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先の更新]

このアクションモジュールは、ID を使用して既存の連絡先を更新します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 連絡先 ID]</p> </td> 
   <td> <p>更新する連絡先の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ]</td> 
   <td> <p>情報を入力するフィールドを選択し、それらのフィールドの必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カスタムフィールド ]</td> 
   <td> <p>情報を入力するフィールドを選択し、それらのフィールドの必要な値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 会議出席依頼を作成する]

このアクションモジュールは、お客様のアカウントに会議出席依頼を追加します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フォーム ID]</p> </td> 
   <td> <p>新しい会議出席依頼の作成に使用するフォームの ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 会議リクエストフィールド ]</td> 
   <td> <p>情報を入力する会議出席依頼のフィールドを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベントリクエストフィールド ]</td> 
   <td> <p>情報を入力するイベントリクエストフィールドを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP リクエストフィールド ]</td> 
   <td> <p>情報を入力する提案フィールドのリクエストを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL レコードのリスト]

この検索モジュールは、特定のタイプのすべてのレコードに関する情報を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Cvent] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Cvent] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL レコードタイプ ]</p> </td> 
   <td> <p>リストするレコードの種類を選択します。</p> 
    <ul> 
     <li> <p>お客様の [!DNL Cvent] アカウント</p> </li> 
     <li> <p>イベントのすべてのセッション</p> </li> 
     <li> <p>イベントのすべての招待者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント ID]</td> 
   <td> <p>招待者またはセッションをリストする場合は、招待者またはセッションが関連付けられているイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
