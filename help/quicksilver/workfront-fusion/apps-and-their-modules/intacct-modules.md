---
title: インタラクトモジュール
description: インタラクトモジュール
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# インタラクトモジュール

内 [!DNL Adobe Workfront Fusion] シナリオの場合、Intacct を使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。

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

Intacct モジュールを使用するには、Intacct アカウントが必要です。

## Intacct をWorkfront Fusion に接続

### 認証中 [!DNL Workfront Fusion] Intacct で変更を行うには

前 [!DNL Workfront Fusion] 接続可能 [!DNL Intacct]に設定する場合は、認証する必要があります。

Intacct アカウントで、 **[!UICONTROL 会社]** タブをクリックします。

1. クリック **会社情報**.
1. 次に移動： **セキュリティ** タブをクリックします。
1. クリック [!UICONTROL 編集] 右上隅に
1. 「 Web サービス認証」を選択します。
1. プラスアイコンをクリックします。
1. sender_id に AzuquaMPP と入力します。
1. （オプション）接続の説明を入力します

### での接続の設定 [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

次に、 [!DNL Intacct] 内部から直接アカウント [!DNL Intacct] モジュール。

1. 任意の Intacct モジュールで、 **[!UICONTROL 追加]** 「接続」フィールドの横に表示されます。
1. Intacct 資格情報を入力してください

   * 会社 ID
   * ユーザー ID
   * パスワード

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## モジュールとそのフィールドをインタラクトします

設定時に [!DNL Intacct] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、アプリやサービスでのアクセスレベルなどの要因に応じて、追加のインタラクトフィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL カスタム API 呼び出しをおこなう]](#make-a-custom-api-call)
* [[!UICONTROL レコードを検索]](#search-records)

### [!UICONTROL カスタム API 呼び出しをおこなう] {#make-a-custom-api-call}

このアクションモジュールを使用すると、 [!DNL Intacct] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Intacct] モジュール。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>接続</p> </td> 
   <td> <p>Intacct アカウントをに接続する手順については、 [!DNL Workfront Fusion] 2.0。 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Workfront Fusion での接続の設定</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本文 XML</td> 
   <td> <p>本文内に XML のみを含めます。 リクエストには、認証ヘッダーが自動的に含まれます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを検索]

この検索モジュールは、特定の検索条件に一致するレコードのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>接続</p> </td> 
   <td> <p>Intacct アカウントをに接続する手順については、 [!DNL Workfront Fusion] 2.0。 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Workfront Fusion での接続の設定</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>検索するレコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>検索条件</p> </td> 
   <td> 
    <ul> 
     <li> <p>検索するフィールドを選択します</p> </li> 
     <li> <p>検索に使用する演算子を選択します</p> </li> 
     <li> <p>検索する値を入力します</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">結果セット</td> 
   <td>一致するすべてのレコードを返すか、最初に一致したレコードのみを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">制限</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">並べ替え基準</td> 
   <td>結果の並べ替えに使用するフィールドを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">順序</td> 
   <td>昇順と降順のどちらで並べ替えるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">出力</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">大文字と小文字の区別</td> 
   <td>クエリで大文字と小文字を区別するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">プライベートエンティティにクエリ</td> 
   <td>モジュールでプライベートエンティティの検索を許可するには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>
