---
title: HubSpot CRM モジュール
description: ' [!DNL Adobe Workfront Fusion] HubSpot CRM モジュールを使用すると、イベント、レコード、連絡先、エンゲージメント、ファイルやフォームの送信を監視したり、 [!DNL HubSpot CRM] アカウント内のレコード、連絡先、エンゲージメント、イベント、ファイルを作成、取得、アップデート、削除したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 5bb394c2fffb4426d66a8b144802db8f7c97afe1
workflow-type: tm+mt
source-wordcount: '2586'
ht-degree: 98%

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

## [!DNL Adobe Workfront Fusion] を [!DNL HubSpot CRM] に接続

[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、[ [!DNL Adobe Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

## [!DNL HubSpot CRM] モジュールとそのフィールド

[!DNL Hubspot CRM] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Hubspot CRM] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [CRM オブジェクト](#crm-objects)
* [レコード（契約、連絡先、会社）](#records-deals-contacts-and-companies)
* [連絡先](#contacts)
* [契約](#deals)
* [会社](#companies)
* [ファイル](#files)
* [チケット](#tickets)
* [API 呼び出しを実行](#make-an-api-call)

### CRM オブジェクト

#### [!UICONTROL CRM オブジェクトを検索]

この検索モジュールは、カスタムプロパティまたはクエリで CRM オブジェクトを検索します。製品や明細項目を検索するには、必要なカスタムスコープで特別な接続を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### レコード（契約、連絡先、会社）

* [[!UICONTROL レコードを作成（レガシー）]](#create-a-record-legacy)
* [[!UICONTROL レコードを取得]](#get-a-record)
* [[!UICONTROL レコードを更新]](#update-a-record)
* [[!UICONTROL レコードを削除]](#delete-a-record)
* [[!UICONTROL レコードプロパティを取得]](#get-a-record-property)
* [[!UICONTROL レコードを監視]](#watch-records)

#### [!UICONTROL レコードを作成（レガシー）]

このアクションモジュールは、連絡先、会社または契約を作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>レコードに設定するプロパティを入力します。使用できるフィールドは、作成するレコードのタイプによって異なります。</td> 
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
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL レコードを更新]

このアクションモジュールは、連絡先、会社または契約を更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL レコードを削除]

このアクションモジュールは、連絡先、会社または契約を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL レコードプロパティを取得]

このアクションモジュールは、（内部）名で特定のレコードプロパティのメタデータを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL レコードを監視]

このトリガーモジュールは、過去 30 日以内に連絡先、会社または契約が変更または作成された場合にシナリオを開始します。出力できるレコード数は 10,000 個に制限されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

### 連絡先

* [[!UICONTROL 連絡先を作成／更新（レガシー）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 連絡先グループを作成／更新]](#createupdate-a-group-of-contacts)
* [[!UICONTROL リストに連絡先を追加]](#add-contacts-to-a-list)
* [[!UICONTROL リストから連絡先を削除]](#remove-a-contact-from-a-list)
* [[!UICONTROL 連絡先を結合]](#merge-contacts)
* [[!UICONTROL 連絡先を検索]](#search-for-contacts)
* [[!UICONTROL 連絡先のリスト]](#list-contacts)
* [[!UICONTROL 会社の連絡先のリスト]](#list-contacts-of-a-company)

#### [!UICONTROL 連絡先を作成／更新（レガシー）]

ポータルに存在しない場合は連絡先を作成します。または存在する場合は最新のプロパティ値で更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL リストに連絡先を追加]

このモジュールは、システムで既に作成されている連絡先レコードを、連絡先リストに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください</p> </td> 
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
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください</p> </td> 
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

#### [!UICONTROL 連絡先を結合]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL 連絡先を検索]

検索クエリを使用して連絡先のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL 連絡先のリスト]

ポータルで作成されたすべての連絡先を返します。出力できる連絡先は 5000 に制限されます。前の連絡先または次の連絡先を一覧表示するには、[!UICONTROL 詳細]パラメーターを使用して、リストをオフセットします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>[!DNL Workfront Fusion] が 1 回のシナリオ実行サイクルで返す連絡先の最大数。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
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
   <td> <p>[!DNL HubSpot CRM]アカウントを[!DNL Workfront Fusion]に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>連絡先をリストしたい会社の ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>[!DNL Workfront Fusion] が 1 回のシナリオ実行サイクルで返す連絡先の最大数。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
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
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください</p> </td> 
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

### 契約

* [[!UICONTROL 契約／チケットパイプラインのリスト]](#list-dealticket-pipelines)
* [[!UICONTROL 契約の CRM パイプラインを取得]](#get-a-deals-crm-pipeline)

#### [!UICONTROL 契約パイプラインまたはチケットパイプラインのリスト]

指定されたポータルのすべての契約とチケットのパイプラインを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>契約またはチケットのどちらをリストするか選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 契約の CRM パイプラインの取得]

特定の契約パイプラインを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

### 会社

#### [!UICONTROL ドメインで会社を検索]

ドメインプロパティとの完全一致に基づいて、会社のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

### ファイル

* [[!UICONTROL フォルダーを作成]](#create-a-folder)
* [[!UICONTROL フォルダーを削除]](#delete-a-folder)
* [[!UICONTROL ファイルを移動]](#move-a-file)

#### [!UICONTROL フォルダーを作成]

このモジュールは、フォルダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

#### [!UICONTROL フォルダーを削除]

フォルダーを削除済みとしてマークします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM]アカウントを[!DNL Workfront Fusion]に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するフォルダーの ID を入力します。</td> 
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
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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

### チケット

#### [!UICONTROL チケットの削除]

ID を指定して既存のチケットを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL HubSpot CRM]アカウントを[!DNL Workfront Fusion]に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するチケットの ID を入力します。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 呼び出しの実行]

カスタム API 呼び出しを実行できます。

>[!NOTE]
>
>次のエンドポイントは、2023 年 8 月 31 日に HubSpot API で廃止されたので、Fusion モジュールでは使用できなくなりました。
>
>* コンテンツイベントのリスト
>* ソーシャルイベントのリスト
>* カレンダータスクイベントのリスト
>* すべてのカレンダーイベントのリスト
>* カレンダータスクを作成
>* ID 別のカレンダータスクの取得
>* カレンダータスクを更新
>* カレンダータスクの削除

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL HubSpot CRM] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
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
