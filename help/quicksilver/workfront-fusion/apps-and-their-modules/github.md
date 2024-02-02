---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: GitHub モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオでは、GitHub を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1844'
ht-degree: 100%

---

# [!DNL GitHub] モジュール

[!DNL Adobe Workfront Fusion] シナリオでは、[!UICONTROL GitHub] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select]または[!UICONTROL Prime]の [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL GitHub] モジュールを使用するには、[!DNL GitHub] アカウントが必要です。

## [!DNL GitHub] から [!DNL Workfront Fusion] への接続

[!DNL GitHub] アカウントを [!UICONTROL Workfront Fusion] に接続する手順に関しては、[[!UICONTROL Adobe Workfront Fusion] への接続を作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

## [!DNL GitHub] モジュールとそのフィールド。

[!DNL GitHub] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL GitHub] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

* [[!UICONTROL イシューを監視]](#watch-issues)
* [[!UICONTROL リポジトリーを監視]](#watch-repositories)
* [[!UICONTROL フォークを監視]](#watch-forks)
* [[!UICONTROL コメントを監視]](#watch-comments)
* [[!UICONTROL 取得リクエストを監視]](#watch-pull-requests)

#### [!UICONTROL イシューを監視]

このモジュールは、新しいイシューが追加されたり、既存のイシューが変更されたりするとトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub]アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to watch]</td> 
   <td>すべてのリポジトリーを監視するか、1 つのリポジトリーのみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>1 つのリポジトリーのみのイシューの監視を選択している場合は、監視するリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned issues]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数を設定します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>新しいイシューのみを監視するか、新しいイシューとすべての変更を監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>監視するイシューを、そのイシューとどのように関係しているかによってフィルタリングできます。</p> 
    <ul> 
     <li>[!UICONTROL All issues]</li> 
     <li>[!UICONTROL Only issues assigned to me]</li> 
     <li>[!UICONTROL Only issues created by me]</li> 
     <li>[!UICONTROL Only issues mentioning me]</li> 
     <li>[!UICONTROL Only issues I'm subscribed to updates for]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>未完了のイシューのみを閲覧するか、クローズされたイシューのみを閲覧するかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>タグを追加します。モジュールは、このタグが付いたイシューを監視します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リポジトリーを監視]

このモジュールは、リポジトリーの作成時または変更時にトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続を作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned repositories]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数を設定します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>新しいリポジトリーとすべての変更を監視するか、新しいリポジトリーのみを監視するかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォークを監視]

このモジュールは、新しいフォークが作成されたときにトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続を作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>フォークを監視するリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned forks]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数を設定します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを監視]

このモジュールは、新しいコメントが追加されたり、既存のコメントが変更されたりするとトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続を作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>監視するリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue number]</td> 
   <td>特定のイシューに対して行われた新しいコメントのみを検索するように検索を制限する場合は、イシューの番号を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned issues]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数を設定します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>新しいコメントのみを監視するか、コメントとすべての変更を監視するかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得リクエストを監視]

このモジュールは、新しい取得リクエストが追加されたり、または既存の取得リクエストが変更されたりするとトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>監視するリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned pull requests]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数を設定します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>[!UICONTROL only open pull]リクエスト、[!UICONTROL only closed ones]またはすべてのプルリクエストのどれを監視するかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>新規のプルリクエストのみを監視するか、新規のリクエストとすべての変更を監視するかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL イシューの検索]](#search-for-an-issue)
* [[!UICONTROL 問題の作成]](#create-an-issue)
* [[!UICONTROL イシューの更新]](#update-an-issue)
* [[!UICONTROL イシューの取得]](#get-an-issue)
* [[!UICONTROL 割り当て先の追加]](#add-assignees)
* [[!UICONTROL 割り当て先の削除]](#remove-assignees)
* [[!UICONTROL イシューへのラベルの追加]](#add-labels-to-an-issue)
* [[!UICONTROL イシューからのラベルの削除]](#remove-a-label-from-an-issue)
* [[!UICONTROL コメントの作成]](#create-a-comment)
* [[!UICONTROL コメントの一覧表示]](#list-comments)

#### [!UICONTROL イシューの検索]

このモジュールでは、検索条件に一致するイシューを検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned issues]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数（シナリオ実行あたりの繰り返し回数）を設定します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>検索結果の並べ替え方法を選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Best match] </p> </li> 
     <li>[!UICONTROL Date created]</li> 
     <li>[!UICONTROL Date updated]</li> 
     <li>[!UICONTROL Number of comments]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort direction]</td> 
   <td> <p>昇順または降順を選択します。 </p> <p>日付の場合、<strong>[!UICONTROL descending]</strong>を選択すると、最新の日付が最初に返されます。 </p> <p>[!UICONTROL number of comments]の場合、<strong>[!UICONTROL descending]</strong>を選択すると、コメントが最も多いイシューが最初に返されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>検索クエリを入力またはマッピングします。検索オプションについて詳しくは、[!DNL GitHub] ヘルプサイトの<a href="https://docs.github.com/ja/github/searching-for-information-on-github/searching-issues-and-pull-requests">Issue およびプルリクエストを検索する</a>を参照してください。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 問題の作成]

このモジュールでは、選択したリポジトリに新しいイシューを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>イシューを作成するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>イシューに割り当てる担当者を選択します。対応可能な担当者には、リポジトリへの書き込み権限を持つすべてのユーザーや、リポジトリへの読み取り権限を持つ組織のメンバーが含まれます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>新しいイシューに関連付けるマイルストーンを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>新しいイシューに適用するラベルを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>新しいイシューのタイトルを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>説明や追加情報など、イシューの本文の入力またはマッピング</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イシューを更新]

このモジュールは、既存の [!DNL GitHub] イシューを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>イシューを更新するリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>イシューに割り当てる担当者を選択します。対応可能な担当者には、リポジトリーへの書き込み権限を持つユーザーや、リポジトリーへの読み取り権限を持つ組織のメンバーが含まれます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>イシューに関連付けるマイルストーンを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>イシューに適用するラベルを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>更新するイシューのイシュー番号を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>イシューの更新先のステートを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>イシューのタイトルを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>説明や追加情報など、イシューの本文の入力またはマッピング</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イシューを取得]

このモジュールは、指定されたイシューに関する詳細を取得します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>詳細を取得するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>詳細を取得するイシューの問題番号を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 割り当て先を追加]

このモジュールは、指定されたイシューに割り当て先を追加します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>割り当て先を追加するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>イシューに割り当てる担当者を選択します。対応可能な担当者には、リポジトリーへの書き込み権限を持つユーザーや、リポジトリーへの読み取り権限を持つ組織のメンバーが含まれます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>担当者を追加するイシューのイシュー番号を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 割り当て先を削除]

このモジュールは、指定されたイシューから割り当て先を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>割り当て先を削除するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>イシューから削除するユーザーを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>割り当て先を削除するイシューのイシュー番号を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イシューにラベルを追加]

このモジュールは、イシューにラベルを追加します。ラベルはリポジトリーレベルで定義され、リポジトリーへの書き込みアクセス権を持つユーザーのみが作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>ラベルを追加するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>イシューに追加するラベルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>ラベルを追加するイシューのイシュー番号を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イシューからラベルを削除]

このモジュールは、1 つのラベルをイシューから削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>ラベルを削除するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>イシューから削除するラベルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>ラベルを削除するイシューのイシュー番号を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを作成]

このモジュールは、指定されたイシューに対するコメントを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>コメントを作成するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>コメントを作成するイシューのイシュー番号を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>コメントの内容を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを一覧表示]

このモジュールは、指定されたイシューに関するすべてのコメントを一覧表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>コメントを一覧表示するイシューを含むリポジトリーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>コメントを一覧表示するイシューのイシュー番号を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>モジュールは、この日付以降に作成されたコメントを返します。サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での強制型変換を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned comments]</td> 
   <td>[!DNL Workfront Fusion] が 1 サイクルの間に連携する結果の最大数を設定します。 </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
