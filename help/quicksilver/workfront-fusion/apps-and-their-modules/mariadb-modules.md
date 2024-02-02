---
title: MariaDB モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL MariaDB] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '593'
ht-degree: 100%

---

# [!DNL MariaDB] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL MariaDB] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL MariaDB] モジュールを使用するには、[!DNL MariaDB] アカウントが必要です。

## [!DNL MariaDB] を [!DNL Workfront Fusion] に接続

[!DNL MariaDB] アカウントへの接続を、[!DNL MariaDB] モジュール内から直接作成できます。

1. 任意の [!DNL MariaDB] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 次のフィールドを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>新しい接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>データベースインスタンスの IP アドレスまたはホスト名を入力します。このホストは、ネットワークの外部からアクセスできる必要があります。</p> <p>例： <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>デフォルトのポートは 3306 です。非標準のポートを使用している場合は、この番号をポートに設定します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Database Name]</td> 
      <td>操作するデータベースの名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>ユーザー名を入力してください.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>パスワードを入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL MariaDB] モジュールとそのフィールド

[!DNL MariaDB] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらと共に、アプリやサービスのアクセスレベルなどの要因に応じて、追加の [!DNL MariaDB] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

### クエリの実行（上級）

このアクションモジュールは、指定したクエリに基づいて、データベースから情報を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL MariaDB] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の「<a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">[!DNL MariaDB] を [!DNL Workfront Fusion]</a> へ接続」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>モジュールがデータの取得に使用する SQL クエリを入力します。</p> <p>重要：クエリで使用される変数は不要部分が削除されていません。SQL 挿入を防ぐために、変数の不要部分を適切に削除してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL テーブルから行を選択（上級）]

このモジュールは、データベースからレコードを読み取ります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL MariaDB] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">[!DNL MariaDB] を [!DNL Workfront Fusion]</a> に接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table]</td> 
   <td> <p>読み取るレコードがあるテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>行の選択に使用するフィルターを設定します。</p> 
    <ul> 
     <li> <p>検索の基準となるフィールドを選択</p> </li> 
     <li> <p>検索に使用する演算子を選択</p> </li> 
     <li> <p>検索する値を入力またはマッピング</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort] </td> 
   <td> <p>結果を並べ替える各レベルで「<strong>[!UICONTROL Add item]</strong>」をクリックし、次に、結果の並べ替えの基準となるフィールドを選択し、昇順または降順のどちらで並べ替えるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
