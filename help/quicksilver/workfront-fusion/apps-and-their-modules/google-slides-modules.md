---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Slides モジュール
description: Adobe Workfront Fusion Google Slides モジュールを使用すると、プレゼンテーションの作成、更新、リスト作成、削除をおこなったり、Google Slides アカウントでプレゼンテーションに画像をアップロードしたりできます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# [!DNL Google Slides] モジュール

この [!DNL Adobe Workfront Fusion] [!DNL Google Slides] モジュールを使用すると、プレゼンテーションの作成、更新、リスト、削除や、および内のプレゼンテーションへの画像のアップロードが可能です [!DNL Google Slides] アカウント

を使用するには [!DNL Google Slides] と [!DNL Workfront Fusion]の場合、 [!DNL Google] アカウント 次の条件を満たさない場合、 [!DNL Google] アカウントはまだ、 [!DNL Google] アカウントヘルプページ。

また、 [!DNL Google Slides] の [!DNL Google Drive].

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

使用する [!DNL Google Slides] モジュールの場合、 [!DNL Google] アカウント

## [!DNL Google Slides] モジュールとそのフィールド

設定時に [!DNL Google Slides] モジュール、Workfront Fusion には、以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Slides] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [表示域](#presentation)
* [その他](#other)

### 表示域

* [[!UICONTROL ウォッチPresentations]](#watch-presentations)
* [[!UICONTROL リストPresentations]](#list-presentations)
* [[!UICONTROL プレゼンテーションの取得]](#get-a-presentation)
* [[!UICONTROL ページ/サムネールの取得]](#get-a-pagethumbnail)
* [[!UICONTROL テンプレートからプレゼンテーションを作成する]](#create-a-presentation-from-a-template)
* [[!UICONTROL プレゼンテーションに画像をアップロード]](#upload-an-image-to-a-presentation)
* [[!UICONTROL グラフの更新]](#refresh-a-chart)
* [[!UICONTROL スライドの追加/削除]](#adddelete-a-slide)

#### [!UICONTROL ウォッチPresentations]

トリガー：新しいプレゼンテーションが作成または更新されたとき。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチ ] </td> 
   <td> <p>プレゼンテーションを見るには、次のオプションを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL 作成日 ]</p> </li> 
     <li> <p>[!UICONTROL 変更日 ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>1 つのシナリオの実行サイクルで返されるプレゼンテーションの最大数Workfront Fusion。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストPresentations]

すべてのプレゼンテーションのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブの場所を選択 ]</td> 
   <td> <p>を選択します。 [!DNL Google Drive] リストするプレゼンテーションの場所は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有</li> 
     <li>[!UICONTROL [!DNL Google] 共有ドライブ ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID]</td> 
   <td> <p>リストするプレゼンテーションのフォルダの場所を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>プレゼンテーションの最大数 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL プレゼンテーションの取得]

指定したプレゼンテーションの最新バージョンを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>を選択します。 [!DNL Google Drive] リストするプレゼンテーションの場所は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有</li> 
     <li>[!UICONTROL [!DNL Google] 共有ドライブ ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーション ID]</td> 
   <td> <p> 取得するプレゼンテーションを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ページ/サムネールの取得]

指定したページの最新バージョン、またはプレゼンテーション内のページのサムネールを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーション ID]</td> 
   <td> <p> 取得するプレゼンテーション ID を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page Object ID]</td> 
   <td> <p> ページオブジェクトの詳細を表示するスライドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ページのサムネールを表示 ]</td> 
   <td> <p> ページのサムネール情報を表示する場合は、このチェックボックスを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テンプレートからプレゼンテーションを作成する]

次のようなすべてのタグを置き換えて、新しいプレゼンテーションを作成します。 `{{Name}}`, `{{Email}}` 指定されたデータを含むテンプレート内。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイトル ] </td> 
   <td> <p>新しいプレゼンテーションの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーションをコピー ]</td> 
   <td> <p> 既存のプレゼンテーションをコピーする場合は、「 」オプションを選択します。</p> 
    <ul> 
     <li>[!UICONTROL マッピングによる ]</li> 
     <li>[!UICONTROL ドロップダウン別 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 既存のプレゼンテーション ID のコピー ]</td> 
   <td> <p> コピーする既存のプレゼンテーションのパスまたはプレゼンテーション ID を入力します。 このフィールドは、[!UICONTROL By Mapping] プレゼンテーションを作成する場合に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>を選択します。 [!DNL Google Drive] リストするプレゼンテーションの場所は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有</li> 
     <li>[!UICONTROL [!DNL Google] 共有ドライブ ]</li> 
    </ul> <p>このフィールドは、[!UICONTROL By Dropdown] プレゼンテーションを作成する場合に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーション ID]</td> 
   <td> <p> テンプレートとして使用するプレゼンテーションのプレゼンテーション ID を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値 ] </td> 
   <td> <p>値を追加します。</p> 
    <ul> 
     <li><strong>[!UICONTROL タグ ]</strong>:プレゼンテーションで置き換えるタグを入力します。 以下に例を挙げます。 <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL 置換された値 ]</strong>:既存のタグを置き換える値を入力します。 例えば、文字列 <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL プレゼンテーションに画像をアップロード]

指定したデータを使用して画像をアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーションの選択 ]</td> 
   <td> <p>画像のアップロード先のプレゼンテーションを選択する方法を選択します。</p> 
    <ul> 
     <li>[!UICONTROL マッピングによる ]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>を選択します。 [!DNL Google Drive] リストするプレゼンテーションの場所は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有</li> 
     <li>[!UICONTROL [!DNL Google] 共有ドライブ ]</li> 
    </ul> <p>このフィールドは、[!UICONTROL By Dropdown] プレゼンテーションを作成する場合に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーション ID]</td> 
   <td> <p> 画像のアップロード先のプレゼンテーションのプレゼンテーション ID を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値 ]</td> 
   <td> <p>値値を追加します。</p> 
    <ul> 
     <li><strong>[!UICONTROL タグ ]</strong>:URL を追加するタグを入力します。</li> 
     <li><strong>[!UICONTROL 画像 URL]</strong>:アップロードする画像のパスまたは URL を入力します。</li> 
    </ul> <p>注意：画像のサイズは 50MB 未満、25 メガピクセルを超えることはできず、PNG、JPEG、GIFのいずれかの形式にする必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL グラフの更新]

ID で指定されたプレゼンテーションに保存されているグラフデータを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>を選択します。 [!DNL Google Drive] リストするプレゼンテーションの場所は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有</li> 
     <li>[!UICONTROL [!DNL Google] 共有ドライブ ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーション ID]</td> 
   <td> <p>更新するグラフを含むプレゼンテーションのプレゼンテーション ID を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL グラフオブジェクト ID]</td> 
   <td> <p> 更新するグラフを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL スライドの追加/削除]

指定したプレゼンテーションの空のスライドを作成するか、既存のスライドを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッドを選択 ]</td> 
   <td> <p>新しいスライドを追加するか、スライドを削除するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>スライドを追加または削除するプレゼンテーションのプレゼンテーション ID を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 定義済みレイアウトタイプ ]</td> 
   <td> <p> 追加したスライドで使用する定義済みのスライドレイアウトを選択します。 追加のフィールド（[!UICONTROL タイトル ] など）の値を指定します。</p> 
    <ul> 
     <li>[!UICONTROL 空白のレイアウト（プレースホルダーなし）]</li> 
     <li>[!UICONTROL 下部にキャプションを表示するレイアウト ]</li> 
     <li>[!UICONTROL タイトルとサブタイトルを含むレイアウト ]</li> 
     <li>[!UICONTROL タイトルと本文を含むレイアウト ]</li> 
     <li>[!UICONTROL タイトルと 2 列のレイアウト ]</li> 
     <li>[!UICONTROL タイトルのみのレイアウト ]</li> 
     <li>[!UICONTROL セクションタイトルを含むレイアウト ]</li> 
     <li>[!UICONTROL 一方にタイトルとサブタイトルが付き、もう一方に説明が付くレイアウト ]</li> 
     <li>[!UICONTROL レイアウト。1 つのタイトルと 1 つの本文が含まれ、1 つの列に配置されます ]</li> 
     <li>[!UICONTROL メインポイントを含むレイアウト ]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>このフィールドは、スライドを追加する場合に選択できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)
* [[!UICONTROL プレゼンテーションにリンクを挿入する]](#insert-links-in-a-presentation)

#### [!UICONTROL API 呼び出しを実行する]

許可された任意の API 呼び出しを実行します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>https://developers.google.com/slides/に対する相対パスを入力します。 例：プレゼンテーション。</p> <p>使用可能なエンドポイントの一覧については、 <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API ドキュメント</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>目的のリクエストヘッダーを入力します。 認証ヘッダーを追加する必要はありません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> リクエストクエリ文字列を入力します。</p> </td> 
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

>[!INFO]
>
>**例：** API 呼び出しを使用して、入力したプレゼンテーション ID のプレゼンテーションの詳細を取得できます。 プレゼンテーション ID は、URL 内で [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>次の API 呼び出しは、プレゼンテーションの詳細を返します。
>
>![](assets/presentation-details.png)
>
>検索結果は、モジュールの「出力」の「 [!UICONTROL バンドル] > [!UICONTROL 本文] > [!UICONTROL presentationId].
>
>この例では、要求されたプレゼンテーションの詳細が返されました。
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL プレゼンテーションにリンクを挿入する]

このモジュールは、プレゼンテーション内のすべてのリンクをクリック可能にするか、一致するすべての入力テキストにリンクを挿入します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Slides] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーションの選択 ]</td> 
   <td> <p>画像のアップロード先のプレゼンテーションを選択する方法を選択します。</p> 
    <ul> 
     <li>[!UICONTROL マッピングによる ]</li> 
     <li>[!UICONTROL ドロップダウン別 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブを選択 ]</td> 
   <td> <p>を選択します。 [!DNL Google Drive] リストするプレゼンテーションの場所は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有</li> 
     <li>[!UICONTROL [!DNL Google] 共有ドライブ ]</li> 
    </ul> <p>このフィールドは、[!UICONTROL By Dropdown] プレゼンテーションを作成する場合に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プレゼンテーション ID]</td> 
   <td> <p>リストするプレゼンテーションのフォルダの場所を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 選択 ]</td> 
   <td> <p>プレゼンテーション内のすべてのリンクをクリック可能にするか、すべての一致する入力テキストにリンクを挿入するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テキスト入力 ]</td> 
   <td>リンクを追加する各テキスト項目に対して、項目と、関連するリンクをリストに追加します。 アイテムがプレゼンテーションに表示されるたびに、指定したサイトに自動的にリンクされます。</td> 
  </tr> 
 </tbody> 
</table>
