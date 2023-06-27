---
title: MariaDB モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL MariaDB]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 1%

---

# [!DNL MariaDB] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL MariaDB]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL MariaDB] モジュールの場合、 [!DNL MariaDB] アカウント

## 接続 [!DNL MariaDB] から [!DNL Workfront Fusion]

次に、 [!DNL MariaDB] 内部から直接アカウントを取得する [!DNL MariaDB] モジュール。

1. 任意の [!DNL MariaDB] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 次のフィールドを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 接続名 ]</p> </td> 
      <td> <p>新しい接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ホスト ]</td> 
      <td> <p>データベースインスタンスの IP アドレスまたはホスト名を入力します。 このホストは、ネットワークの外部からアクセスできる必要があります。</p> <p>例: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ポート ]</td> 
      <td>デフォルトのポートは 3306 です。 非標準ポートを使用している場合は、この番号をポートに設定します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL データベース名 ]</td> 
      <td>やり取りするデータベースの名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ユーザー名 ]</td> 
      <td>ユーザー名を入力してください.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL パスワード ]</td> 
      <td>パスワードを入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL MariaDB] モジュールとそのフィールド

設定時に [!DNL MariaDB] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL MariaDB] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### クエリの実行（詳細）

このアクションモジュールは、指定したクエリに基づいて、データベースから情報を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL MariaDB] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">接続 [!DNL MariaDB] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ ]</td> 
   <td> <p>モジュールがデータの取得に使用する SQL クエリを入力します。</p> <p>重要：クエリで使用される変数は不要部分が削除されません。 SQL 挿入を防ぐために、変数の不要部分を適切に削除してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL テーブルから行を選択（詳細）]

このモジュールは、データベースからレコードを読み取ります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL MariaDB] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">接続 [!DNL MariaDB] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表 ]</td> 
   <td> <p>読み取るレコードを含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>行を選択するフィルターを設定します</p> 
    <ul> 
     <li> <p>検索するフィールドを選択します</p> </li> 
     <li> <p>検索に使用する演算子を選択します</p> </li> 
     <li> <p>検索する値を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え ] </td> 
   <td> <p>結果を並べ替える各レベルで、 <strong>[!UICONTROL 項目を追加 ]</strong>次に、結果の並べ替えに使用するフィールドを選択し、昇順または降順のどちらで並べ替えるかを選択します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
