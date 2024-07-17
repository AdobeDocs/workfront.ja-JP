---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Workfront基板モジュール
description: Adobe Workfront Boards コネクタを使用すると、Workfront Boards 内のプロセスを自動化し、サードパーティのアプリやサービスに接続できます。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 0b4a25f7-a8f1-47f4-8929-7eff82f1dfdc
source-git-commit: 7003ea4b6daba68957ef0ec501ecfd4a8d750d4c
workflow-type: tm+mt
source-wordcount: '2591'
ht-degree: 20%

---

# [!DNL Adobe Workfront] Boards モジュール

>[!NOTE]
>
>このコネクタは現在Betaにあります。

Adobe Workfront ボードは、列やカードを含む共有ボードへのアクセスを提供することで、チームの共同作業を可能にする柔軟なツールです。

Adobe Workfront ボード モジュールを使用すると、レコードの読み取りや更新、Workfront ボード API への API 呼び出しを行ったり、ボードでアクションが発生した場合のシナリオのトリガーを設定したりできます。

Workfront ボードの一般的な情報については、[ ボードの概要 ](/help/quicksilver/agile/boards-overview.md) を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>任意</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td>
   <td> <p>新規：標準</p><p>または</p><p>現在：[!UICONTROL 計画 ]、[!UICONTROL 作業 ]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。


## 前提条件

ボードに接続するには、Adobe Workfrontでボードを設定しておく必要があります。

## Workfront Boards への接続の作成

>[!NOTE]
>
>Workfront接続を使用してWorkfront Boards に接続するか、別のWorkfront Boards 接続を作成できます。

Workfront ボード接続を作成するには：

1. 任意の [!DNL Adobe Workfront Boards] モジュールで、「接続」ボックスの横にある「**[!UICONTROL 追加]**」をクリックします。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>この接続の名前を入力します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>実稼動環境と非実稼動環境のどちらに接続するかを選択します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>サービスアカウントに接続するか、個人アカウントに接続するかを選択します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]<p>（オプション）</p></td>
          <td>[!DNL Adobe] [!UICONTROL Client ID] を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]<p>（オプション）</p></td>
          <td>[!DNL Adobe] [!UICONTROL Client Secret] を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Authentication URL]<p>（オプション）</p></td>
          <td>Workfrontのインスタンスで、この接続の認証に使用する URL を入力します。 <p>デフォルト値は <code>https://oauth.my.workfront.com/integrations/oauth2</code> です。</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Host prefix]</td>
          <td>ホストのプレフィックスを入力します。<p>デフォルト値は <code>origin-</code> です。</p>
        </tr>
      </tbody>
    </table>
1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。

## Adobe Workfront Boards モジュールとそのフィールド

Workfront ボードモジュールを設定すると、以下に示 [!DNL Workfront Fusion] フィールドが表示されます。 これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加のWorkfront ボードフィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [カード](#cards)
* [ボード](#boards)
* [列](#columns)
* [タグ](#tags)
* [コメント](#comments)
* [その他](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### カード

* [チェックリスト項目を追加](#add-checklist-item)
* [サブタスクを追加](#add-subtask)
* [カードの作成](#create-a-card)
* [カードの移動](#move-a-card)
* [カードを読み取る](#read-a-card)
* [カードの更新](#update-a-card)

#### チェックリスト項目を追加

このアクションモジュールは、指定されたカードにチェックリスト項目を追加します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>チェックリスト項目を追加するカードの ID を入力またはマッピングします<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チェックリスト項目 ]</td> 
   <td>追加するチェックリスト項目ごとに、「項目を追加」をクリックし、チェックリスト項目の名前を入力して、項目が完了したかどうかを選択します。</p></td> 
  </tr> 
 </tbody> 
</table>

#### サブタスクを追加

このアクションモジュールは、ボードのカードにサブタスクを追加します。 カードは接続されている必要があります。 サブタスクは、カードが表すWorkfront タスクにも追加されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 親カード ID]</td> 
   <td>サブタスクの追加先となるカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>サブタスクの追加先となるカードを含むボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>新しいサブタスクの名前を入力またはマッピングします。</p></td> 
  </tr> 
 </tbody> 
</table>

#### カードの作成

Workfrontのボード上に新しいカードを作成します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>カードを追加するボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列 ID]</td> 
   <td>サブタスクを追加する列の ID を入力またはマッピングします。<p>列 ID は、ボードを読み取りモジュールから返される情報で見つけることができます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>新しいカードの名前を入力またはマッピングします。</p></td> 
  </tr> 
 </tbody> 
</table>

#### カードの移動

このアクションモジュールは、カードを同じボード上の別の列に移動します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>移動するカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>移動するカードを含むボードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 宛先列 ID]</td> 
   <td>カードの移動先の列の ID を入力またはマッピングします。<p>列 ID は、ボードを読み取りモジュールから返される情報で見つけることができます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL からインデックスへ ]</td> 
   <td>新しい列にカードを配置する位置を入力またはマップします。<p>インデックス 0 の列の一番上の位置。</p></td> 
  </tr> 
 </tbody> 
</table>

#### カードを読み取る

このアクションモジュールは、特定のカードに関する情報を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>読み取るカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
 </tbody> 
</table>

#### カードの更新

このアクションモジュールは、指定したカードの情報を更新します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>更新するカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>更新するカードを含むボードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>カードの新しい名前を入力またはマッピングします。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>カードの新しい説明を入力またはマッピングします。</p></td> 
  </tr> 
 </tbody> 
</table>

### ボード

* [ボードを作成](#create-a-board)
* [ボードを読み取る](#read-a-board)

#### ボードを作成

Workfrontにボードを作成します。 作成するボードのタイプを指定できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ボード名 ]</td> 
   <td>新しいボードの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td>作成するボードのタイプを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### ボードを読み取る

このアクションモジュールは、ボードのカード、列、タグ、メンバーなど、1 つのボードに関する情報を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>情報を取得するボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
 </tbody> 
</table>

### 列

* [列の作成](#create-a-column)
* [列の検索](#search-for-a-column)
* [列の更新](#update-a-column)

#### 列の作成

このアクションモジュールは、指定されたボードに新しい列を作成します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>列を追加するボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列 ID]</td> 
   <td>更新する列の ID を入力またはマッピングします。<p>列 ID は、ボードを読み取りモジュールから返される情報で見つけることができます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列名 ]</td> 
   <td>列の新しい名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL の WIP 制限 ]</td> 
   <td>列の新しい WIP 制限を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### 列の検索

この検索モジュールは、指定された名前を持つ列に関する情報を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>取得する列を含むボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列名 ]</td> 
   <td>取得する列の名前を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### 列の更新

このアクションモジュールは、指定された列の名前または WIP 制限を更新します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>取得する列を含むボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列名 ]</td> 
   <td>取得する列の名前を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### タグ

* [カードにタグを追加](#add-card-tag)
* [タグの作成](#create-a-tag)

#### カードにタグを追加

このアクションモジュールは、カードにタグを追加します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>タグの追加先となるカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>タグの追加先となるカードを含んだボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag ID]</td> 
   <td>追加するタグの ID を入力またはマッピングします。<p>タグ ID は、ボードを読み取りモジュールから返される情報で見つけることができます。</p></td> 
  </tr> 
 </tbody> 
</table>

#### タグの作成

このアクションモジュールは、新しいタグを作成し、カラーを割り当てます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>タグを作成するボードの ID を入力またはマッピングします。<p>Workfrontでボードを表示する際に、URL にボード ID が含まれています。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タグ名 ]</td> 
   <td>新しいタグの名前を入力またはマッピングします。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タグの色 ]</td> 
   <td>このタグのカラーを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### コメント

* [コメントの作成](#create-a-comment)
* [カードコメントを読む](#read-card-comments)

#### コメントの作成

このアクションモジュールは、指定されたカードにコメントを作成しました。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>コメントを追加するカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>追加するコメントのテキストを入力またはマップします。</p></td> 
  </tr> 
 </tbody> 
</table>

#### カードコメントを読む

このアクションモジュールは、指定されたカードからコメントを取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>コメントを取得するカードの ID を入力またはマッピングします。<p>Workfrontでカードを表示すると、URL にカード ID が表示されます。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>1 回の実行サイクルでモジュールに返すコメントの最大数を入力します。</p></td> 
  </tr> 
 </tbody> 
</table>

### その他

#### カスタム API 呼び出しの実行

このアクションモジュールは、Workfront Boards API へのカスタム呼び出しを行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
      <td> <p>既存のWorkfront接続を使用してWorkfront Boards に接続することも、特定のWorkfront Boards 接続を使用することもできます。 </p><p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、こちらの <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Workfront ボードへの接続の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p><code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code> への相対パスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p><p>ほとんどのボードの場合、メソッドはPOSTです。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。これにより、リクエストのコンテンツタイプが決まります。</p> <p>例：<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>Workfront ボードの場合、このセクションは通常、空のままになります。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>API 呼び出しの本文コンテンツを JSON 埋め込み Graphql の形式で追加します </p> <p>例：</p><p>次の使用例は、列名を更新します。 <code>boardId</code> と <code>columnId</code> を、ハードコードされた GUID または以前のモジュールからマッピングされた GUID として含めることができます。<p><pre>{

  &quot;query&quot;: &quot;mutation { updateColumn （boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }） { id name }}&quot;

}</pre><p>メモ：  <p><code>if などの条件文を使用する場合</code> json で、条件文の外に引用符を付けます。</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
