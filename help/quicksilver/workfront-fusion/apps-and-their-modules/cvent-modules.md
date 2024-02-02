---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Cvent モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオでは、Cvent を使用するワークフローを自動化したり、複数のサードパーティアプリケーションおよびサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1044'
ht-degree: 100%

---

# [!DNL Cvent] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Cvent] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Cvent] モジュールを使用するには、[!DNL Cvent] アカウントが必要です。

## [!DNL Adobe Workfront Fusion] に [!DNL Cvent] を接続 {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>[!DNL Cvent] モジュールは、[!UICONTROL SOAP] API 経由で動作します。[!DNL Cvent] への接続を作成するには、次の点を確認する必要があります。
>
>* [!DNL Cvent] API への [!UICONTROL SOAP] アクセス権を持っている
>* [!DNL Workfront Fusion] IP アドレスが組織の許可リストに追加されている。
>
>  [!DNL Workfront Fusion] IP アドレスのリストについては、[アクセス用の IP アドレス [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)を参照してください。


[!DNL Cvent] アカウントへの接続を、[!DNL Cvent] モジュール内から直接作成できます。

1. 任意の [!DNL Cvent] モジュールで、[!UICONTROL 接続]フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続する地域を選択します。

   * [!UICONTROL 北米]
   * [!UICONTROL ヨーロッパ]
   * [!UICONTROL サンドボックス]

1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL Cvent] モジュールとそのフィールド

[!DNL Cvent] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらとともに、アプリやサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Cvent] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) におけるモジュール間での情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#create-meeting-request)
* [[!UICONTROL レコードの読み取り]](#read-a-record)
* [[!UICONTROL 招待者の登録]](#register-invitee)
* [[!UICONTROL 招待者の追加]](#add-invitee)
* [[!UICONTROL 連絡先の削除]](#delete-contact)
* [[!UICONTROL 連絡先の更新]](#update-contact)
* [[!UICONTROL 会議出席リクエストの作成]](#create-meeting-request)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL Cvent] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Cvent] モジュールでは不可能なデータフロー自動処理を実現できます。

このモジュールを設定する際には、次のフィールドが表示されます。

このモジュールは、ステータスコードと共に API 呼び出しのヘッダーと本文を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Cvent] への [!DNL Adobe Workfront Fusion]</a> の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本文（XML）</td> 
   <td> <p>API 呼び出しの本文を入力またはマッピングします。XML のみを含める必要があります。モジュールには、認証ヘッダーが自動的に含まれます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、特定のレコードに関する情報を読み取ります。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Cvent] の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td>読み取るレコードの項目タイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact]／[!UICONTROL Event]／[!UICONTROL Invitee ID]</td> 
   <td> <p>読み取る項目の ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。フィールドは、選択した項目タイプに基づいて使用できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 招待者の登録]

このアクションモジュールでは、イベントの招待者を登録できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Cvent] の接続を参照してください。</p> </td> 
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

#### [!UICONTROL 招待者の追加]

このアクションモジュールでは、連絡先をイベントに招待できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Cvent] への [!DNL Adobe Workfront Fusion]</a> の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>イベントに追加する連絡先の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>連絡先を追加するイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先の削除]

このアクションモジュールでは、Cvent 内の 1 つの連絡先を削除できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Cvent] への [!DNL Adobe Workfront Fusion]</a> の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID]</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Cvent] への [!DNL Adobe Workfront Fusion]</a> の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>更新する連絡先の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>情報を入力するフィールドを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> <p>情報を入力するフィールドを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 会議出席リクエストの作成]

このアクションモジュールは、お客様のアカウントに会議出席リクエストを追加します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Cvent] を [!DNL Adobe Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Form ID]</p> </td> 
   <td> <p>新しい会議出席リクエストの作成に使用するフォームの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Meeting Request Fields]</td> 
   <td> <p>情報を入力する会議出席リクエストフィールドを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Request Fields]</td> 
   <td> <p>情報を入力するイベントリクエストフィールドを選択し、それらのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Cvent] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Cvent] を [!DNL Adobe Workfront Fusion]</a> へ接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td> <p>リストに表示するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!DNL Cvent] アカウントからのすべてのイベント</p> </li> 
     <li> <p>イベントのすべてのセッション</p> </li> 
     <li> <p>イベントのすべての招待者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>招待者またはセッションをリストする場合は、招待者またはセッションが関連付けられているイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
