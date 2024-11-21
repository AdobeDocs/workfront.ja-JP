---
title: HubSpot CRM モジュール
description: ' [!DNL Adobe Workfront Fusion] HubSpot CRM モジュールを使用すると、イベント、レコード、連絡先、エンゲージメント、ファイルやフォームの送信を監視したり、 [!DNL HubSpot CRM] アカウント内のレコード、連絡先、エンゲージメント、イベント、ファイルを作成、取得、アップデート、削除したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '6411'
ht-degree: 41%

---

# [!DNL HubSpot CRM] モジュール

[!DNL Adobe Workfront Fusion][!DNL HubSpot CRM]モジュールを使用すると、イベント、レコード、連絡先、エンゲージメント、ファイルやフォームの送信を監視したり、[!DNL HubSpot CRM]アカウント内のレコード、連絡先、エンゲージメント、イベント、ファイルを作成、取得、アップデート、削除したりすることができます。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL HubSpot CRM] モジュールを使用するには、[!DNL HubSpot CRM] アカウントが必要です。

## HubSpot CRM API 情報

HubSpot CRM コネクタは以下を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ベース URL</td> 
   <td>https://api.hubapi.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API タグ</td> 
   <td>v2.0.14</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Adobe Workfront Fusion] を [!DNL HubSpot CRM] に接続

[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、[ [!DNL Adobe Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

>[!NOTE]
>
>接続を設定する際に、**HubSpot CRM** 接続タイプを選択します。 HubSpot CRM （非推奨）タイプは既存の接続をサポートしていますが、新しい接続を作成するためにこのタイプを使用することはお勧めしません。

## [!DNL HubSpot CRM] モジュールとそのフィールド

[!DNL Hubspot CRM] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Hubspot CRM] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [CRM オブジェクト](#crm-objects)
* [レコード（契約、連絡先、会社）](#records-deals-contacts-and-companies)
* [連絡先](#contacts)
* [契約](#deals)
* [会社](#companies)
* [エンゲージメント](#engagements)
* [イベントと通知](#events-and-notifications)
* [ファイル](#files)
* [タスク](#tasks)
* [ユーザー](#users)
* [チケット](#tickets)
* [フォーム](#forms)
* [ソーシャルメディア（放送）](#social-media-broadcast)
* [ ブログ投稿 ](#blog-posts)
  <!--* [Workflows]-->
* [ 購読 ](#subscriptions)
  <!--* [Associations](#associations)-->
* [その他](#other)

+++**CRM オブジェクト**

### CRM オブジェクト

* [CRM オブジェクトの検索](#search-for-crm-objects)
* [CRM オブジェクトの監視](#watch-crm-objects)

#### [!UICONTROL CRM オブジェクトを検索]

この検索モジュールは、カスタムプロパティまたはクエリで CRM オブジェクトを検索します。製品や明細項目を検索するには、必要なカスタムスコープで特別な接続を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>モジュールが 1 回の実行サイクルで返す最大項目数を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type to Search]</td> 
   <td>検索する Hubspot CRM オブジェクトのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。使用可能なフィールドは、選択したオブジェクトによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by] </td> 
   <td> <p>検索のフィルター方法を選択</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>クエリを入力またはマッピング</p> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>検索のグループまたはフィルターを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>結果を並べ替える場合は、クリックします。結果の並べ替えを選択すると、以下のフィールドが表示されます。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Property name]</strong> </p> <p>結果の並べ替えに使用するプロパティを選択します</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>結果を昇順または降順のどちらで並べ替えるかを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">開始オフセット</td> 
    <td>詳細を取得する最初の項目の ID を入力またはマッピングします。 このモジュールは、一度に最大 5000 件の結果のみを返します。 開始オフセットを設定すると、最初の 5000 以外の項目を取得できます。 開始オフセットが 5000 の場合、モジュールは項目 5000-9999 を返します。</td> 
   </tr>
 </tbody> 
</table>

#### CRM オブジェクトの監視

このトリガーモジュールは、CRM オブジェクトが作成または更新されると、シナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>モジュールが 1 回の実行サイクルで返す最大項目数を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！検索する UICONTROL オブジェクトの種類 ]</td> 
   <td> <p>検索するオブジェクトのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>このモジュールの出力に含めるプロパティを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL が作成/更新されました ]</td> 
   <td>作成された（新規）オブジェクトと更新された（変更済み）オブジェクトのどちらをウォッチするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by]</td> 
   <td>フィルターを追加すると、特定の条件を満たした場合にのみシナリオが開始されるようになります。<ul><li><b>クエリ</b><p>フィルターに使用するクエリを入力します。</li><li><b>プロパティ</b><p>結果のフィルタに使用する各プロパティに対して、[<b> アイテムの追加 </b>] をクリックし、プロパティ名、演算子、およびプロパティ値を入力します。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**レコード （取引、連絡先、会社）**

### レコード（契約、連絡先、会社）

* [レコードを作成](#create-a-record)
* [[!UICONTROL レコードを作成（レガシー）]](#create-a-record-legacy)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL レコードの取得]](#get-a-record)
* [[!UICONTROL レコードプロパティを取得]](#get-a-record-property)
* [レコードのリスト](#list-records)
* [[!UICONTROL レコードの更新]](#update-a-record)
* [[!UICONTROL レコードを監視]](#watch-records)

#### レコードを作成

このアクションモジュールは、連絡先、会社または取引を作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロパティ グループ ]</td> 
   <td>レコードの作成時に追加するプロパティごとに、プロパティがあるグループを選択します。 プロパティグループが開き、プロパティの値を入力できます。 使用できるプロパティグループとプロパティは、作成するレコードのタイプによって異なります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成（レガシー）]

このアクションモジュールは、連絡先、会社または契約を作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>レコードに設定するプロパティを入力します。使用できるフィールドは、作成するレコードのタイプによって異なります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、連絡先、会社または契約を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>削除するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除する連絡先、会社または契約の ID を入力します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを取得]

このアクションモジュールは、連絡先、会社または契約の詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>レコードタイプを選択します。</p> 
    <ul> 
     <li>[!UICONTROL Contact]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td>連絡先を取得する場合は、ID で識別するか、メールアドレスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>取得する連絡先、会社または契約の ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>詳細を取得する連絡先のメールアドレスを入力します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードプロパティを取得]

このアクションモジュールは、（内部）名で特定のレコードプロパティのメタデータを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>メタデータを取得するプロパティを持つレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property Name]</td> 
   <td>メタデータを取得するプロパティを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> 一部のプロパティには、ユーザーがプロパティ値として選択できる一連の使用可能なオプションがあります。取得するプロパティ値を表すオプションの ID を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードのリスト

この検索モジュールは、連絡先、会社、または取引のリストを返します。 出力は、5,000 の連絡先、12,500 の会社、または 12,500 の取引に制限されています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>返すレコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>このモジュールの出力に含めるプロパティを選択します。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr>

</tbody> 
</table>

#### [!UICONTROL レコードを更新]

このアクションモジュールは、連絡先、会社または契約を更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>更新するレコードの種類を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>連絡先を取得する場合は、レコードを識別する方法を選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>更新する連絡先、会社または契約の ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>詳細を更新する連絡先のメールアドレスを入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>レコードに設定するプロパティを入力します。使用できるフィールドは、作成するレコードのタイプによって異なります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを監視]

このトリガーモジュールは、過去 30 日以内に連絡先、会社または契約が変更または作成された場合にシナリオを開始します。出力できるレコード数は 10,000 個に制限されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>監視するプロパティを持つレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>最近変更したレコードと最近作成したレコードのどちらを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>モジュールの出力に含めるプロパティを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**連絡先**

### 連絡先

* [[!UICONTROL リストに連絡先を追加]](#add-contacts-to-a-list)
* [連絡先の作成/更新](#createupdate-a-contact)
* [[!UICONTROL 連絡先を作成／更新（レガシー）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 連絡先グループを作成／更新]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 連絡先のリスト]](#list-contacts)
* [[!UICONTROL 会社の連絡先のリスト]](#list-contacts-of-a-company)
* [[!UICONTROL 連絡先を結合]](#merge-contacts)
* [[!UICONTROL リストから連絡先を削除]](#remove-a-contact-from-a-list)
* [[!UICONTROL 連絡先を検索]](#search-for-contacts)
* [リストに追加された連絡先を見る](#watch-contacts-added-to-a-list)

#### [!UICONTROL リストに連絡先を追加]

このモジュールは、システムで既に作成されている連絡先レコードを、連絡先リストに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>連絡先を追加するリストの ID を選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/Emails] </td> 
   <td> <p>リストに追加する連絡先を識別する方法を選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>リストに追加する連絡先の ID を追加します。</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>リストに追加する連絡先のメールアドレスを追加します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### 連絡先の作成/更新

このアクションモジュールは、ポータルに連絡先が存在しない場合、連絡先を作成します。 連絡先がポータルに存在する場合、このモジュールは指定された値で連絡先を更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロパティ グループ ]</td> 
   <td>連絡先を作成するときに追加するプロパティごとに、プロパティがあるグループを選択します。 プロパティグループが開き、プロパティの値を入力できます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先を作成／更新（レガシー）]

ポータルに存在しない場合は連絡先を作成します。または存在する場合は最新のプロパティ値で更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>連絡先の設定または更新を行うプロパティを入力します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先グループを作成／更新]

連絡先のグループを作成するか、既に存在する場合は更新します。バッチサイズが 100 件の連絡先以下に制限されている場合は、最適なパフォーマンスが実現します。このエンドポイントを通じて行われた変更は非同期で処理されるので、連絡先レコードに変更が適用されるまで数分かかる場合があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch of Contacts to Create/Update] </td> 
   <td> <p>連絡先のバッチを追加します。</p> <p><strong>[!UICONTROL Add item]</strong> をクリックして、新しい連絡先を追加します。表示されるウィンドウで、次の情報を入力またはマッピングします。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>連絡先を識別する方法を選択してください。</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>作成または更新する連絡先の ID を入力します。 </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>作成または更新する連絡先のメールアドレスを入力します。 </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>連絡先の設定または更新を行うプロパティを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先のリスト]

ポータルで作成されたすべての連絡先を返します。出力できる連絡先は 5000 に制限されます。前の連絡先または次の連絡先を一覧表示するには、[!UICONTROL 詳細]パラメーターを使用して、リストをオフセットします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>[!DNL Workfront Fusion] が 1 回のシナリオ実行サイクルで返す連絡先の最大数。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。 </td> 
  </tr> 
   <tr> 
    <td role="rowheader">連絡先 ID [ 開始オフセット ] </td> 
    <td>リストを開始するユーザーの ID を入力またはマッピングします。 例えば、連絡先 ID を 101 番目の連絡先の ID として設定すると、モジュールは 1-5000 ではなく、101-5100 の連絡先をリストできます。 </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL 会社の連絡先リスト]

会社内の連絡先リストを取得します。出力できる連絡先は 5000 に制限されます。前の連絡先または次の連絡先を一覧表示するには、[!UICONTROL 詳細]パラメーターを使用して、リストをオフセットします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>連絡先をリストしたい会社の ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>[!DNL Workfront Fusion] が 1 回のシナリオ実行サイクルで返す連絡先の最大数。 </td> 
  </tr> 
   <tr> 
    <td role="rowheader">連絡先 ID [ 開始オフセット ] </td> 
    <td>リストを開始するユーザーの ID を入力またはマッピングします。 例えば、連絡先 ID を 101 番目の連絡先の ID として設定すると、モジュールは 1-5000 ではなく、101-5100 の連絡先をリストできます。 </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL 連絡先を結合]

このアクション モジュールは連絡先を結合します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>結合するいずれかの連絡先の ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>結合する他の連絡先の ID を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストから連絡先を削除]

連絡先リストから連絡先を削除。

>[!NOTE]
>
>動的リストから連絡先を手動で削除することはできません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>連絡先を削除するリストの ID を選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID] </td> 
   <td>リストから削除する連絡先の ID を入力します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連絡先を検索]

検索クエリを使用して連絡先のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>検索クエリを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>[!DNL Workfront Fusion] が 1 回のシナリオ実行サイクルで返す連絡先の最大数を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストに追加された連絡先を監視]

このトリガーモジュールは、新しい連絡先がリストに追加されると、シナリオを開始します。これは、有料マーケティングアカウントを持つユーザーのみが利用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>監視する連絡先が含まれるリストの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>モジュールの出力に含めるプロパティを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**取引**

### 契約

* [[!UICONTROL 契約の CRM パイプラインを取得]](#get-a-deals-crm-pipeline)
* [[!UICONTROL 契約／チケットパイプラインのリスト]](#list-dealticket-pipelines)

#### [!UICONTROL 契約の CRM パイプラインを取得]

特定の契約パイプラインを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pipeline ID] </td> 
   <td>詳細を取得するパイプラインの ID を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>詳細を取得するステージの ID を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 契約パイプラインまたはチケットパイプラインのリスト]

指定されたポータルのすべての契約とチケットのパイプラインを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>契約またはチケットのどちらをリストするか選択します。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**会社**

### 会社

#### [!UICONTROL ドメインで会社を検索]

ドメインプロパティとの完全一致に基づいて、会社のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td><code>[!DNL hubspot].com</code> など、検索する会社のドメインを入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>1 回のシナリオ実行サイクルで [!DNL Workfront Fusion] が返す必要のある最大企業数。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。 </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**業務**

### エンゲージメント

* [エンゲージメントと CRM オブジェクトの関連付け](#associate-an-engagement-with-a-crm-object)
* [エンゲージメントの作成](#create-an-engagement)
* [エンゲージメントの削除](#delete-an-engagement)
* [エンゲージメントの監視](#watch-engagements)

#### エンゲージメントと CRM オブジェクトの関連付け

このアクションモジュールは、エンゲージメントを連絡先、会社または取引に関連付けます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>契約を関連付ける CRM レコードのタイプを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンゲージメント ID]</td> 
  <td>オブジェクトに関連付ける契約の ID を入力またはマッピングします。</td> 
   </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record ID]</td> 
  <td>エンゲージメントを関連付けるレコードの ID を入力またはマッピングします。</td> 
   </tr> 
 </tbody> 
</table>

#### エンゲージメントの作成

このアクションモジュールは、HubSpot の CRM オブジェクトとのエンゲージメント（メモ、タスク、アクティビティなど）を作成します。 エンゲージメントとは、CRM に記録する必要がある連絡先とのインタラクションです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL はアクティブですか？]</td> 
   <td>新しいエンゲージメントが作成時にアクティブになる場合は、このオプションを有効にします。 タイムラインに表示するには、エンゲージメントがアクティブである必要があります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
  <td>作成する契約のタイプを選択します。
  <ul>
  <li><b>メール</b><p></p><a href="#email-metadata" class="MCXref xref" > メールメタデータ </a> に進みます。</p></li>
  <li><b>通話</b><p><a href="#call-metadata" class="MCXref xref" > メタデータの呼び出し </a> を続行します。</p></li>
  <li><b>ミーティング</b><p><a href="#meeting-fields" class="MCXref xref" > 会議フィールド </a> に進みます。</p></li>
  <li><b>タスク</b><p><a href="#task-fields" class="MCXref xref" > タスクフィールド </a> に進みます。</p></li>
  <li><b>メモ</b><p>「本文」フィールドに、メモのテキストを入力します。</p></li>
  </ul>
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">タイムスタンプ</td> 
   <td>エンゲージメントのタイムスタンプを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">所有者 ID</td> 
   <td>エンゲージメントが割り当てられる人物の所有者 ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">UID</td> 
   <td>エンゲージメントの ID を入力またはマッピングします。この ID は、オブジェクトタイプをまたいで使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ポータル ID</td> 
   <td>ポータルの ID を入力またはマッピングします。 組織に複数のポータルがある場合に役立ちます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">関連連絡先</td> 
   <td>この契約を関連付ける連絡先ごとに、[<b> 項目の追加 </b>] をクリックして連絡先 ID を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">関係会社</td> 
   <td>この契約を関連付ける会社ごとに、「<b> 項目を追加 </b>」をクリックして会社 ID を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">関連取引</td> 
   <td>このエンゲージメントを関連付ける取引ごとに、「<b> 項目を追加 </b>」をクリックして、取引 ID を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">関連チケット</td> 
   <td>このエンゲージメントを関連付けるチケットごとに、「<b> 項目を追加 </b>」をクリックしてチケット ID を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">添付ファイル</td> 
   <td>この契約を関連付ける添付ファイルごとに、[<b> アイテムの追加 </b>] をクリックし、添付するファイルのファイル ID を入力します。</td> 
  </tr> 
 </tbody> 
</table>

##### メールメタデータ

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL From &gt; Email]</p> </td> 
   <td> <p>メールの送信元のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First Name]</td> 
   <td>メールの送信元のユーザーの名を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Last Name]</td> 
  <td>メールの送信元の人物の姓を入力またはマッピングします。
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">終了</td> 
   <td>メールの送信先のメールアドレスごとに、「<b> 項目を追加 </b>」をクリックして、メールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cc</td> 
   <td>メールの CC の送信先とするメールアドレスごとに、「<b> 項目を追加 </b>」をクリックして、メールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bcc</td> 
   <td>メールの BCC 送信先のメールアドレスごとに、「<b> 項目を追加 </b>」をクリックして、メールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">件名</td> 
   <td>メールの件名のテキストを入力またはマッピング</td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML</td> 
   <td>HTML形式のメールを送信するには、メールの本文をHTMLタグを含めて入力するかマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">テキスト</td> 
   <td>テキストのみのメールを送信するには、メールの本文のテキストを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

##### メタデータの呼び出し

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL から Number へ ]</p> </td> 
   <td> <p>通話の宛先の電話番号を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL From Number]</td> 
   <td>通話の発信元の電話番号を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
  <td>通話のステータスを選択します。
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">本文</td> 
   <td>通話の詳細またはメモを入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">外部 ID</td> 
   <td>このフィールドは、HubSpot で行われた呼び出しの内部 ID を表します。 アクションは必要ありません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">期間</td> 
   <td>呼び出しの長さをミリ秒単位で入力またはマッピングします</td> 
  </tr> 
  <tr> 
   <td role="rowheader">外部アカウント ID</td> 
   <td>このフィールドは、HubSpot で行われた呼び出しの内部アカウント ID を表します。 アクションは必要ありません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">録画 URL</td> 
   <td>記録ファイルの URL を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

##### 会議フィールド

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Title]</p> </td> 
   <td> <p>会議のタイトルまたは件名を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>ミーティングの説明または詳細のテキストを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始時刻 ]</td> 
  <td>会議の開始時刻を UNIX タイムスタンプとして入力またはマップします。
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">終了時間</td> 
   <td>会議の終了時刻を UNIX タイムスタンプとして入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

##### タスクフィールド

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Subject]</p> </td> 
   <td> <p>タスクのタイトルまたは件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>タスクの説明または詳細のテキストを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ステータス</td> 
   <td>タスクのステータスを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL （オブジェクト型） ]</td> 
  <td><code>CONTACT</code> または <code>COMPANY</code> を入力します。
  </td> 
   </tr> 
 </tbody> 
</table>

#### エンゲージメントの削除

このアクションモジュールは、ID によってエンゲージメントを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>削除する契約の ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### エンゲージメントの監視

このトリガーモジュールは、ポータルで新しいエンゲージメントが作成されたときにシナリオを開始します。 このモジュールは、過去 30 日間に作成されたレコード、または最近作成された 10,000 件のレコードのみを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>1 回のシナリオ実行サイクルで [!DNL Workfront Fusion] が返す必要のある最大企業数。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>イベントを監視する最も早い日付を入力またはマップします。 <code>MM/DD/YYYY h:mm</code> の形式を使用します。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**イベントと通知**

### イベントと通知

* [タイムラインイベントの作成/更新](#create--update-a-timeline-event)
* [タイムラインイベントタイプのリスト](#list-timeline-event-types)
* [カレンダーイベントを見る](#watch-calendar-events)
* [通知を見る](#watch-notifications)

#### タイムラインイベントの作成/更新

このアクションモジュールは、タイムラインイベントを作成または更新します。 このモジュールは、ユーザー識別子、HubSpot API キー、クライアント ID およびクライアント秘密鍵を含む開発者接続でのみ使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アプリケーション ID]</td> 
   <td>このイベントが属するアプリケーションの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td>このイベントの ID を入力またはマッピングします。 イベント ID はシステムによって生成されません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント タイプ ID]</td> 
   <td>このイベントのイベントタイプの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>イベントを作成する連絡先のメールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL オブジェクト ID]</td> 
   <td>イベントを作成する連絡先の ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp]</td> 
   <td>このイベントのタイムスタンプを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カスタム データ ]</td> 
   <td>このイベントに追加するカスタム データの項目ごとに、[<b> 項目の追加 </b>] をクリックし、項目の名前と値を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### タイムラインイベントタイプのリスト

この検索モジュールは、特定のアプリケーションのすべてのタイムラインイベントのリストを返します。 このモジュールは、ユーザー識別子、HubSpot API キー、クライアント ID およびクライアント秘密鍵を含む開発者接続でのみ使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アプリケーション ID]</td> 
   <td>このイベントが属するアプリケーションの ID を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### カレンダーイベントを見る

このトリガーモジュールは、新しいイベントがカレンダーに追加されたときにシナリオを開始します。 開始日と終了日の間の間隔には、最大 500 個のタスクが含まれます。 このモジュールは、ユーザー識別子、HubSpot API キー、クライアント ID およびクライアント秘密鍵を含む開発者接続でのみ使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベントの種類 ]</td> 
   <td>ソーシャルイベント、コンテンツイベントまたはすべてのイベントのどちらを視聴するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオ実行サイクルでモジュールが返す最大ファイル数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>開始日を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>終了日を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### 通知を見る

このトリガーモジュールは、変更に関する新しい通知が送信されると、シナリオを開始します。  開始日と終了日の間の間隔には、最大 500 個のタスクが含まれます。 このモジュールは、ユーザー識別子、HubSpot API キー、クライアント ID およびクライアント秘密鍵を含む開発者接続でのみ使用できます。 HubSpot では、開発者アプリケーションごとに 1 つの Webhook URL のみを持つことができます。

このモジュールの Webhook を作成するには、Webhook フィールドの横にある **追加** をクリックし、次のフィールドに入力します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アプリケーション ID]</td> 
   <td>この Webhook に使用するアプリケーション ID を入力します。 ID は、HubSpot 開発者ポータルで確認できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 購読 ]</td> 
   <td> <p>監視する通知のタイプごとに、「<b> 項目を追加 </b>」をクリックし、購読のタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 古いサブスクリプションを強制的に削除 ]</td> 
   <td>このオプションを有効にすると、この Webhook に添付されている古いサブスクリプションがデタッチまたは削除されます。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**ファイル**

### ファイル

* [[!UICONTROL フォルダーを作成]](#create-a-folder)
* [ファイルの削除](#delete-a-file)
* [[!UICONTROL フォルダーを削除]](#delete-a-folder)
* [ファイルのリスト](#list-files)
* [[!UICONTROL ファイルを移動]](#move-a-file)
* [ファイルのアップロード](#upload-a-file)
* [ファイルを見る](#watch-files)

#### [!UICONTROL フォルダーを作成]

このモジュールは、フォルダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder Name] </td> 
   <td>新しいフォルダーの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>作成するフォルダーの親フォルダーの ID を選択します。 </td> 
  </tr> 
 </tbody> 
</table>

#### ファイルの削除

このアクション モジュールは、ファイル マネージャからファイルとすべての関連データとサムネイルを完全に削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>削除するファイルの ID を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーを削除]

フォルダーを削除済みとしてマークします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するフォルダーの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### ファイルのリスト

この検索モジュールは、ファイルマネージャに格納されているファイルのリストを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオ実行サイクルでモジュールが返す最大ファイル数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>一覧表示するファイルを含むフォルダの ID を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>ファイル名に特定の文字を含むファイルのみを含めるには、ファイル名に含める文字を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの移動]

ファイルを別のフォルダーに移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>移動するファイルの ID を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>ファイルを移動するフォルダーの ID を選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>移動するファイルの名前を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### ファイルのアップロード

このアクションモジュールは、ファイルマネージャーにファイルをアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アクセスの種類 ] </td> 
   <td>ファイルをプライベート、パブリックだがインデックス不可、またはパブリックでインデックス可能にするかどうかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>ファイルをアップロードするフォルダーの ID を選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>ファイルがフォルダー内に既に存在する場合、このオプションを有効にしてファイルを上書きします。</td> 
  </tr> 
 </tbody> 
</table>

### 監視ファイル

このトリガーモジュールは、新しいファイルがファイルマネージャーに保存されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオ実行サイクルでモジュールが返す最大ファイル数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>監視するファイルを含むフォルダーの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>ファイル名に特定の文字を含むファイルのみを含めるには、ファイル名に含める文字を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**タスク**

### タスク

* [カレンダータスクの作成](#create-a-calendar-task)
* [カレンダータスクの削除](#create-a-calendar-task)
* [タスクイベントを見る](#watch-task-events)

#### カレンダータスクを作成する

このアクションモジュールは、カレンダーに新しいタスクを作成します。 このモジュールで使用される接続では、有料のマーケティングアカウントを持つユーザーの資格情報を使用する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>新しいカレンダータスクの名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>新しいカレンダータスクの説明を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 所有者 ID]</td> 
   <td>このタスクに割り当てるユーザーの所有者 ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベントの日付 ]</td> 
   <td>このタスクの日付を入力またはマップします。<p>サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">型強制：[!DNL Adobe Workfront Fusion]</a> を参照してください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>イベントのタイプを選択します。<ul><li><b>ブログ投稿</b><p>コンテンツグループ ID を入力します。 これはブログページの ID です。</p></li><li><b>メール</b><p>使用するメールテンプレートへのパスを入力またはマッピングします。</li><li><b>ランディングページ</b><p>使用するランディングページテンプレートへのパスを入力またはマッピングします。</li><li><b>カスタム</b></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>イベントの状態が「やること」か「完了」かを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL キャンペーン GUID]</td> 
   <td>このイベントが含まれているキャンペーンの内部ハブスポット ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### カレンダータスクの削除

このアクションモジュールは、カレンダータスクを削除します。 このモジュールで使用される接続では、有料のマーケティングアカウントを持つユーザーの資格情報を使用する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するタスクの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### タスクイベントを見る

このトリガーモジュールは、カレンダーに新しいタスクイベントが発生するとシナリオを開始します。 このモジュールで使用される接続では、有料のマーケティングアカウントを持つユーザーの資格情報を使用する必要があります。 このモジュールは最大 500 個のイベントを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオ実行サイクルでモジュールが返す最大ファイル数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>イベントを監視する最も早い日付を入力またはマップします。 <code>MM/DD/YYYY h:mm</code> の形式を使用します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>イベントを監視する最終日を入力またはマップします。 <code>MM/DD/YYYY h:mm</code> の形式を使用します。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**ユーザー**

### ユーザー

* [所有者の取得](#get-an-owner)
* [リスト所有者](#list-owners)

#### 所有者の取得

このアクションモジュールは、所有者の詳細を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 所有者 ID]</td> 
   <td> <p>詳細を返す所有者の ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### リスト所有者

この検索モジュールは、HubSpot アカウントのすべての所有者のリストを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**チケット**

### チケット

<!--* [Create a Ticket]-->
* [チケットの削除](#delete-a-ticket)
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->

<!-- Create a Ticket Need to find a working connection-->

#### [!UICONTROL チケットの削除]

ID を指定して既存のチケットを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するチケットの ID を入力します。 </td> 
  </tr> 
 </tbody> 
</table>

<!-- Get a Ticket  Need to find a working connection-->

<!-- List Tickets  Need to find a working connection-->

&lt;! – 有効な接続を見つけるために必要なチケットの更新 – >

<!-- Watch Tickets Need to find a working connection-->

+++

+++**Forms**

### フォーム

* [フォーム経由でアップロードされたファイルの取得](#get-a-file-uploaded-via-form)
* [ リストForms](#list-forms)
  <!--* [Submit Data to a Form]-->
  <!--* [Watch Submissions for a Form]-->

#### フォーム経由でアップロードされたファイルの取得

このアクションモジュールは、フォームを通じてアップロードされたファイルを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td>取得するファイルの URL を入力またはマッピングします。 これは、フォームメタデータ内にあります。</td> 
  </tr> 
 </tbody> 
</table>

#### リストのForms

このアクションモジュールは、このモジュールに使用される接続に関連付けられたアカウントで作成されたすべてのフォームを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>1 回の実行サイクルでモジュールが返すフォームの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Submit Data to a Form Need to find a working connection-->



&lt;!—#### フォームの送信を監視する – 有効な接続を見つける必要がある >—>

+++

+++**ソーシャルメディア（放送）**

### ソーシャルメディア（放送）

* [ブロードキャストメッセージのキャンセル](#cancel-a-broadcast-message)
* [ブロードキャストメッセージの作成](#create-a-broadcast-message)
* [放送メッセージを見る](#watch-broadcast-messages)

#### ブロードキャストメッセージのキャンセル

このアクションモジュールは、ツイートやFacebook投稿など、スケジュールされたブロードキャストをキャンセルします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ブロードキャスト ID]</td> 
   <td>キャンセルするブロードキャストの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### ブロードキャストメッセージの作成

このアクションモジュールは、指定されたソーシャルメディアチャネルでメッセージを作成して直ちに公開します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel ID]</td> 
   <td>このブロードキャストに使用するチャネルの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>この放送のタイトルを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>放送のテキストを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 写真 URL]</td> 
   <td>ブロードキャストに含める写真の URL を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サムネール URL]</td> 
   <td>このブロードキャストに使用するサムネールの URL を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL トリガー]</td> 
   <td>ブロードキャストを送信する日時を入力またはマッピングします。 空白のままにすると、ブロードキャストは直ちに送信されます。<p>サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">型強制：[!DNL Adobe Workfront Fusion]</a> を参照してください。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 放送メッセージを見る

このトリガーモジュールは、HubSpot から指定されたソーシャルメディアチャンネルにメッセージが投稿されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>モジュールが 1 回の実行サイクルで返す最大項目数を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！ステータスによる UICONTROL フィルター ]</td> 
   <td>メッセージが特定のステータスの場合にのみシナリオを開始するには、ステータスを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！チャネルによる UICONTROL フィルター ]</td> 
   <td>メッセージが特定のチャネル上にあるときにのみシナリオを開始するには、チャネルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ブロードキャスト ID]</td> 
   <td>メッセージが特定の日付以降の場合にのみシナリオを開始するには、日付を <code>MM/DD/YYYY</code> の形式で入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**ブログ投稿**

### ブログ投稿

<!--* [Create a Blog Post]-->
* [ ブログ投稿の削除 ](#delete-a-blog-post)
  <!--* [List Blog Posts]-->
* [ ブログ投稿のPublish/非公開 ](#publish--unpublish-a-blog-post)
  <!--* [Watch Blog Posts]-->

<!--
#### Create a Blog Post May need connection
-->


#### ブログ投稿の削除

このアクションモジュールは、1 つのブログ投稿を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するブログ投稿の ID を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

<!--#### List Blog Posts May need connection

This search module retrieves posts from a HubSpot blog.-->

#### Publish/ブログ投稿の非公開

このアクション モジュールは、ブログ投稿の公開をスケジュールまたはキャンセルします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>スケジュールまたはキャンセルするブログ投稿の ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td>ブログ投稿をスケジュールするか、以前にスケジュールしたブログ投稿をキャンセルするかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Watch Blog PostsMay need connection-->

+++

<!--+++**Workflows**>

<!--### Workflows May need connection

#### Add a Contact to a Workflow


#### Remove a Contact from a Workflow

-->

<!--+++-->

+++**購読**

### 購読

* [E メール購読の更新](#update-email-subscription)
* [ポータルの購読タイムラインを見る](#watch-subscriptions-timeline-for-a-portal)

#### E メール購読の更新

このアクションモジュールは、HubSpot のメールサブスクリプションを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>更新するサブスクリプションのメールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Statuses]</td> 
   <td>購読を更新するステータスごとに、「<b> 項目を追加 </b>」をクリックし、ステータスの ID と、メールアドレスがそのステータスを購読するかどうかを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ポータル登録の法的状態 ]</td> 
   <td>このサブスクリプションの GDPR に対する法的根拠を記録するには、このサブスクリプションの法的状態を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ポータル登録法的根拠の説明 ]</td> 
   <td>この GDPR 向けサブスクリプションの法的根拠に関するメモを追加するには、メモのテキストを入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### ポータルの購読タイムラインを見る

このトリガーモジュールは、新しいメールタイムラインサブスクリプションがポータルに追加されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>モジュールが 1 回の実行サイクルで返す最大項目数を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始タイムスタンプ ]</td> 
   <td>特定の日付以降の結果を返すには、形式に日付を入力します <code>MM/DD/YYYY.</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 終了タイムスタンプ ]</td> 
   <td>特定の日付以前の結果を返すには、形式で日付を入力します <code>MM/DD/YYYY.</code></td> 
  </tr> 
 </tbody> 
</table>

+++

<!--+++**Associations**-->

<!--### Associations-->

<!--#### Associate CRM Objects  May need connection

This action module associates two CRM objects.-->

<!--#### Associate Multiple CRM Objects  May need connection-->



<!--#### Delete an Association May need connection-->



<!--#### Delete Multiple Associations between CRM Objects May need connection-->



<!--#### List Associations for a CRM Object May need connection-->

<!--+++-->

+++**その他**

### その他

#### [!UICONTROL API 呼び出しの実行]

カスタム API 呼び出しを実行できます。

>[!NOTE]
>
>次のエンドポイントは、2023年8月31日に HubSpot API で廃止されたので、Fusion モジュールでは使用できなくなりました。
>
>* コンテンツイベントのリスト
>* ソーシャルイベントのリスト
>* カレンダータスクイベントのリスト
>* すべてのカレンダーイベントのリスト
>* カレンダータスクの作成
>* ID 別のカレンダータスクの取得
>* カレンダータスクの更新
>* 単一タスクの削除

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>https://api.hubapi.com/ からの相対パスを入力します。例：/contacts/v1/lists/all/contacts/all</p> <p>使用可能なエンドポイントの一覧については、<a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API ドキュメント</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>使用する HTTP メソッドを選択します。</p> <p>[!UICONTROL GET]</p> <p>エントリの情報を取得します。</p> <p>[!UICONTROL POST]</p> <p>新しいエントリを作成します。</p> <p>[!UICONTROL PUT]</p> <p>既存のエントリを更新または置き換えます。</p> <p>[!UICONTROL PATCH]</p> <p>エントリを部分的に更新します。</p> <p>[!UICONTROL DELETE]</p> <p>エントリを削除します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> 希望するリクエストヘッダーを入力します。認証ヘッダーを追加する必要はありません。既に追加されています。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> リクエストクエリ文字列を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で API 呼び出しの本文コンテンツを追加します。JSON で、<code>if</code> などの条件文を使用する場合は、条件文を引用符で囲みます。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**&#x200B;次の API 呼び出しは、[!DNL HubSpot] アカウントのすべての連絡先を返します。
>
>**URL**：`/contacts/v1/lists/all/contacts/all`
>
>**メソッド**：`GET`
>
>![](assets/hubspot-api-config.png)
>
>一致した検索結果は、[!UICONTROL バンドル]／[!UICONTROL 本文]／[!UICONTROL 連絡先]下のモジュールの出力に表示されます。
>
>この例では、3 件の連絡先が返されました。
>
>![](assets/hubspot-api-output.png)

+++

## 新規アプリケーションの作成

1. [!DNL HubSpot] 開発者アカウントにログインします。
1. 「**[!UICONTROL アプリを作成]**」オプションを選択します。
1. アプリ名を入力し、ダイアログを[!UICONTROL 保存]します。
1. Web フックに必要なスコープを選択します。

   例えば、新規連絡先が作成または削除された場合にモジュールをトリガーするための連絡先スコープを追加します。

   連絡先、契約および会社イベントの web フックを受け取るために必要な情報は、[!UICONTROL 連絡先スコープ]だけです。

   >[!IMPORTANT]
   >
   >「[!UICONTROL リダイレクト URL]」フィールドには入力しないでください。
