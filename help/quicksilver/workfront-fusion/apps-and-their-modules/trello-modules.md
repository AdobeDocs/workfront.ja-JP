---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Trello モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオ内では、Trello を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '5095'
ht-degree: 91%

---

# [!UICONTROL Trello] モジュール

[!DNL Adobe Workfront Fusion] シナリオでは、[!UICONTROL Trello] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。

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

[!DNL Trello] モジュールを使用するには、[!UICONTROL Trello] アカウントが必要です。

## [!UICONTROL Trello] を [!DNL Workfront Fusion] に接続

[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、[ [!DNL Adobe Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

## [!UICONTROL Trello] モジュールとそのフィールド

[!UICONTROL Trello] モジュールを設定すると、[!DNL Workfront Fusion] には以下のフィールドが表示されます。これらとともに、アプリやサービスのアクセスレベルなどの要因に応じて、追加の「[!UICONTROL Trello]」フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [ボード](#boards)
* [リスト](#lists)
* [カード](#cards)
* [メンバー](#members)
* [チェックリスト](#checklists)
* [ラベル](#labels)
* [コメント](#comments)

### ボード

+++ **[!UICONTROL ボードを監視]**

このトリガーモジュールは、新しいボードが追加されるとシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すボードの最大数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードを作成]**

このアクションモジュールは、選択した設定で新しいボードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>新しいボードの名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>必要に応じて、ボードの説明を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>組織の ID を入力またはマッピングします。Watch Activities モジュールなどの別のモジュールを使用して組織 ID を取得できます。</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Permission level]</p> </td> 
   <td> <p>ボードには、権限レベルごとに異なる投票ルールおよびコメントルールがあります。例えば、ボードが [!UICONTROL Private] で、投票ルールとコメントルールを [!UICONTROL All] として設定した場合、エラーが発生します。 </p> <p>投票とコメントは、権限レベルごとに次のグループに制限されます。</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>：
      --&gt;メンバー、メンバーおよびオブザーバー</li> 
     <li><strong>[!UICONTROL For organization]</strong>：
      --&gt;メンバー、メンバーおよびオブザーバー、組織のメンバー</li> 
     <li><strong>[!UICONTROL Public]</strong>：
      --&gt;メンバー、メンバーおよびオブザーバー、組織のメンバー、すべて</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>このボードで投票できるユーザーを、オプションを選択して指定します。権限レベルでの投票の制限については、「[!UICONTROL Permission level]」フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>このボードのカードにコメントできるユーザーを、オプションを選択して指定します。権限レベルでのコメントの制限については、「[!UICONTROL Permission level]」フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitations]</p> </td> 
   <td> <p>他のユーザーをこのボードに招待できるユーザーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-join]</p> </td> 
   <td> <p>チームメンバーが自分でボードに参加できるか、招待される必要があるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Default labels]</p> </td> 
   <td> <p>新しいボードにデフォルトのラベルセットを使用するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Default lists]</p> </td> 
   <td> <p>デフォルトのリストセットをボードに追加するかを選択します（[!UICONTROL To Do]、[!UICONTROL Doing]、[!UICONTROL Done]）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board source ID]</p> </td> 
   <td> <p>新しいボードにコピーするボードの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card Covers]</p> </td> 
   <td> <p>ボードのカードカバーを有効にする場合は、「<strong>[!UICONTROL Yes]</strong>」を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Background]</p> </td> 
   <td> <p>背景のカラーまたはカスタム背景を選択します。</p> <p>メモ：カスタム背景は、[!UICONTROL Trello Gold and Business Class] のサブスクライバーのみが使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>カードの期間経過を表す 2 つのモードから選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>：カードは期間が経過するにつれ、徐々に透明になります。 </li> 
     <li><strong>[!UICONTROL Pirate]</strong>：カードは期間が経過するにつれ、古びた海賊の地図のように、裂け、黄ばみ、ひび割れます。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードの編集]**

このアクションモジュールは、既存のボードの設定を編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>モジュールで作成するボードの一意の [!UICONTROL Trello] ID を入力またはマッピングします。Watch Boards モジュールなどの別のモジュールを使用してボード ID を取得できます。</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td> <p> ボードの新しい名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New description]</td> 
   <td> <p> 必要に応じて、ボードの説明を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>モジュールで編集するボードの一意の [!UICONTROL Trello] ID を入力またはマッピングします。[!DNL Watch Activities] モジュールなどの別のモジュールを使用してボード ID を取得できます。</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>オプションを選択して、代理ユーザーがボードに登録しているかどうかを指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Permission level]</p> </td> 
   <td> <p>ボードには、権限レベルごとに異なる投票ルールおよびコメントルールがあります。例えば、ボードが [!UICONTROL Private] で、投票ルールとコメントルールを [!UICONTROL All] として設定した場合、エラーが発生します。 </p> <p>投票とコメントは、権限レベルごとに次のグループに制限されます。</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>：
      --&gt;メンバー、メンバーおよびオブザーバー</li> 
     <li><strong>[!UICONTROL For organization]</strong>：
      --&gt;メンバー、メンバーおよびオブザーバー、組織のメンバー</li> 
     <li><strong>[!UICONTROL Public]</strong>：
      --&gt;メンバー、メンバーおよびオブザーバー、組織のメンバー、すべて</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>このボードで投票できるユーザーを、オプションを選択して指定します。権限レベルでの投票の制限については、「[!UICONTROL Permission level]」フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>このボードのカードにコメントできるユーザーを、オプションを選択して指定します。権限レベルでのコメントの制限については、「[!UICONTROL Permission level]」フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitations] </td> 
   <td> <p>このボードにユーザーを招待できる担当者を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-join]</td> 
   <td> <p> チームメンバーが自分でボードに参加できるか、招待される必要があるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card covers]</td> 
   <td> <p> このボードにカードの表紙を表示するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background] </td> 
   <td> <p>背景のカラーまたはカスタム背景を選択します。</p> <p>メモ：カスタム背景は、[!UICONTROL Trello Gold and Business Class] のサブスクライバーのみが使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> [!UICONTROL Background] フィールドでカスタム背景の使用を選択した場合は、使用する背景の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>カードの期間経過を表す 2 つのモードから選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>：カードは期間が経過するにつれ、徐々に透明になります。 </li> 
     <li><strong>[!UICONTROL Pirate]</strong>：カードは期間が経過するにつれ、古びた海賊の地図のように、裂け、黄ばみ、ひび割れます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar feed enabled]</td> 
   <td> <p> カレンダーフィードを有効にするかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Color&gt; label name]</td> 
   <td> <p> 目的のカラーラベルに名前を割り当てます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>ボードをアーカイブする（閉じる）かどうかを示すオプションを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードを取得]**

このアクションモジュールは、ボードの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>情報を取得するボードの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

この検索モジュールは、指定したボードに関する情報を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>情報を取得するボードの名前（または名前の一部）を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned boards]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 回の実行サイクルで返すボードの最大数を入力します。この値は、1000 以下にする必要があります。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partial] </p> </td> 
   <td> <p>デフォルトでは、このモジュールは、クエリ内の各単語の完全一致をメンバーコンテンツで検索します。[!UICONTROL Partial] が有効な場合、モジュールはクエリ内の任意の単語で始まるコンテンツを検索します。</p> <p> 例えば、「development」という単語を使用して「My Development Status Report」というタイトルのボードを検索する場合、デフォルトでは単語全体を検索する必要があります。[!UICONTROL Partial] を有効にしている場合、「dev」を検索することはできますが、「velopment」を検索することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Boards] </td> 
   <td> <p>「mine」と入力するか、ボード ID のコンマ区切りリストをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードのアーカイブまたはアーカイブ解除]**

このアクションモジュールは、指定したボードを閉じるか、再び開きます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> 閉じる、または再度開くボードの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive or unarchive]</td> 
   <td> <p> ボードを閉じる（アーカイブ）か、再び開く（アーカイブ解除）かを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メンバーをボードに割り当て]**

このアクションモジュールは、指定したボードにメンバーを割り当てます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> メンバーを追加するボードを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email address]</td> 
   <td> <p> ボードに追加するメンバーのメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Member type]</p> </td> 
   <td> <p>ボードに追加するメンバーのタイプを選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>：ボード管理者は、ボード上で任意のボードアクションを実行できます。</li> 
     <li><strong>[!UICONTROL Normal]</strong>：通常のメンバーは、ボードのただのメンバーです。</li> 
     <li><strong>[!UICONTROL Observer]</strong>：オブザーバーは、ボードに対する読み取り専用アクセス権を持つメンバーです。<br>オブザーバーは、[!UICONTROL Trello Business Class] を持っているチームのみが使用できます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Full name]</td> 
   <td> <p> ボードに追加するユーザーのフルネームを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メンバーをボードから割り当て解除]**

このアクションモジュールは、ボードからメンバーを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> ユーザーを削除するボードの ID を入力（マッピングまたは選択）します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>ボードから削除するメンバーを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### リスト

+++ **[!UICONTROL リストに移動されたカードを監視]**

このトリガーモジュールは、カードが特定のリストに移動されるとアクティブ化されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>カードを監視するリストを含むボードを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>カードを監視するリストを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すボードの最大数。</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL リストを作成]**

このアクションモジュールは、指定したボードにリストを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> リストを作成するボードの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>新しいリストの名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>リストを上に追加するか、カードの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy list]</td> 
   <td> <p> コピーするリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>手動で入力</strong> </p> <p><strong>[!UICONTROL List ID]</strong> フィールドに、コピーするリストの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>選択</strong> </p> <p>コピーするリストを含むボードを選択し、リストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL リストを編集]**

このアクションモジュールは、既存のリストを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> 更新するリストの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>リストの新しい名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> リストを移動するボードをマッピングまたは選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>リストを上に追加するか、カードの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribed]</td> 
   <td> <p>アクティブなメンバーをリストに登録する場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL リストを取得]**

このアクションモジュールは、特定のリストに関する詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>情報を取得するリストの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### カード

+++ **[!UICONTROL カードを監視]**

このトリガーモジュールは、新しいカードが追加されると有効になります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched object]</td> 
   <td> <p>カードを監視する場所を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL All cards]</strong> </li> 
     <li> <p><strong>特定のボード上のカード</strong> </p> <p>カードを監視するボードを選択します</p> </li> 
     <li> <p><strong>[!UICONTROL Cards on specific list]</strong> </p> <p>カードを監視するリストが含まれているボードを選択し、リストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すボードの最大数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードを作成]**

このアクションモジュールは、選択したリストにカードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a list ID]</td> 
   <td> <p> カードを追加するリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL List ID]</strong> フィールドに、カードを追加するリストの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>コピーするリストを含むボードを選択し、リストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>カードに追加するラベルごとに、ラベルの ID を入力します。ID は、例えば [!UICONTROL Retrieve Labels] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members]</td> 
   <td>カードに追加する各メンバーに対して、メンバーの ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>新しいカードの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Description]</p> </td> 
   <td> <p>カードの説明を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>カードをリストの一番上に追加するか、[!UICONTROL append] カードをリストの下部に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due date]</td> 
   <td> <p> カードの期限を入力します。サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due complete]</td> 
   <td> <p> カードが期限に達したことを示すには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td> <p>カードに添付ファイルとして追加するファイルの URL を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Source file]</p> </td> 
   <td> <p>カードに添付ファイルとして追加するファイルの情報を入力またはマッピングします。</p> 
    <ul> 
     <li>[!UICONTROL File name]：ファイル拡張子を含むファイル名を入力またはマッピングします。</li> 
     <li> 
     <p>前のモジュールからファイルを選択するか、ファイルの名前とデータをマッピング</p> 
     <p>メモ：ファイルのアップロードには、添付ファイルあたり 10 MB の制限があります。ただし、[!UICONTROL Business Class] のメンバーと [!UICONTROL Trello Gold] のメンバーには、添付ファイル あたり 250MB のアップロード制限があります。</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy card]</td> 
   <td> <p> コピーするカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL Card ID]</strong> フィールドに、コピーするカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>コピーするカードを含むボードを選択し、そのカードを含むリストを選択して、カードを選びます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードを編集]**

このアクションモジュールは、既存のカードを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Card ID]</td> 
   <td> <p> 編集するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL Card ID]</strong> フィールドに、編集するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>編集するカードを含むボードを選択し、そのカードを含むリストを選択して、カードを選びます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td> <p>カードの新しい名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL New description]</p> </td> 
   <td> <p>カードの新しい説明を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Move a card]</p> </td> 
   <td> <p>カードを移動するボードまたはボードとリストを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>カードに追加するラベルの ID を追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>カードをリストの一番上に追加するか、[!UICONTROL append] カードをリストの下部に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due date]</td> 
   <td> <p> カードの期限を入力します。サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due complete]</td> 
   <td> <p> このオプションを有効にすると、カードは期限日に完了とマークされます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members] </td> 
   <td> <p>カードに追加するメンバーの ID を追加またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment cover ID]</p> </td> 
   <td> <p>カードの表紙として使用する画像添付ファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>メンバーをカードに登録するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>カードをアーカイブ（クローズ）するかどうかを示すオプションを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードを入手]**

このアクションモジュールは、選択したカードの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p>詳細を取得するカードが含まれるボードの ID を入力します。この ID によって、ボードのカスタムフィールドの名前を確認できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> 詳細を取得するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>「<strong>[!UICONTROL Card ID]</strong>」フィールドに、詳細を取得するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>詳細を取得するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードを検索]**

このアクションモジュールは、検索クエリに一致するカードを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>検索するボードを選択します。ボードが選択されていない場合は、すべてのボードが検索されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Query]</p> </td> 
   <td> <p>検索クエリを入力します。次の検索演算子を使用すると、検索を絞り込むことができます。</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>「-」を任意の演算子に追加して、除外検索を実行できます。例えば、<code>[!UICONTROL -has:members]</code> を使用すると、メンバーが割り当てられていないカードを検索できます。</p> </li> 
     <li><code><strong>@name</strong></code> <p>メンバーに割り当てられたカードを返します。<code>member:</code> を使用することもできます。カードのみを含めるには <code>@me</code> を使用します。</p> </li> 
     <li><code><strong>#label</strong></code> <p>ラベル付きのカードを返します。<code>label:</code> を使用することもできます。例えば、<code>label:"FIX IT"</code> は「FIX IT」というラベルのカードを返します。</p> </li> 
     <li><code><strong>board:id</strong></code> <p>特定のボード内のカードを返します。例えば、<code>board:Trello</code> は、ボード名に [!UICONTROL Trello] が含まれるボードのカードを返します。</p> </li> 
     <li><code><strong>list:name</strong></code> <p>「name」という名前のリスト内のカードを返します。</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>添付ファイル付きのカードを返します。<code>has</code>: 演算子は、<code>has:description</code>、<code>has:cover</code>、<code>has:members</code> または <code>has:stickers</code> などの他の属性と併用することもできます。</p> </li> 
     <li><code><strong>due:day</strong></code> <p>24 時間以内に期限が切れるカードを返します。<code>due:</code> 演算子は、<code>due:week</code>、<code>due:month</code>、<code>due:overdue</code> などの他の時間枠でも使用できます。また、特定の日の範囲を検索することもできます。例えば、次の 14 日以内に期限が切れるカードを含めるには、検索に <code>due:14</code> を追加します。</p> </li> 
     <li><code><strong>created:day</strong></code> <p>過去 24 時間以内に作成されたカードを返します。<code> created:</code> 演算子は、<code>created:week</code> または <code>created:month</code> などの他の時間枠でも使用できます。また、特定の日の範囲を検索することもできます。例えば、過去 14 日間に作成されたカードを含めるには、検索に <code>created:14</code> を追加します。</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>過去 24 時間に編集されたカードを返します。<code>edited:</code> 演算子は、<code>edited:week</code> や <code>edited:month</code> などの他の時間枠でも使用できます。また、特定の日の範囲を検索することもできます。例えば、過去 21 日間に編集されたカードを含めるには、検索に <code>edited:21</code> を追加します。</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>カードの説明、チェックリスト、コメント、名前のテキストに一致するカードを返します。例えば、comment:"FIX IT" はコメントに「FIX IT」を含むカードを返します。</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>オープンなカード、またはアーカイブされているカードを返します。いずれも指定されていない場合、[!UICONTROL Trello] は両方のタイプを返します。</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>スター付きのボードのカードのみが含まれます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned cards]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 回の実行サイクルで返すカードの最大数。この値は、1000 以下にする必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>デフォルトでは、このモジュールは、クエリ内の各単語の完全一致をメンバーコンテンツで検索します。[!UICONTROL Partial] が有効な場合、モジュールはクエリ内の任意の単語で始まるコンテンツを検索します。</p> <p> 例えば、「development」という単語を使用して「My Development Status Report」というタイトルのボードを検索する場合、デフォルトでは単語全体を検索する必要があります。[!UICONTROL Partial] を有効にしている場合、「dev」を検索することはできますが、「velopment」を検索することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cards] </td> 
   <td> <p>具体的に検索したいカードを追加します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードをアーカイブまたはアーカイブ解除]**

このアクションモジュールは、カードをアーカイブするか、ボードに送り返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card ID]</td> 
   <td> <p> アーカイブするかボードに送り返すカードの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive or unarchive]</td> 
   <td> <p> カードを閉じる（アーカイブ）か、ボードに送り返す（アーカイブ解除）かを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 添付ファイルの追加]**

このアクションモジュールは、選択されたカードに添付ファイルを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> 詳細を取得するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>手動で入力</strong> </p> <p>詳細を取得するカードの ID を「<strong>[!UICONTROL Card ID]</strong>」フィールドに入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>詳細を取得するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment type]</p> </td> 
   <td> <p>ファイルを直接アップロードするか、ファイルの URL を指定するかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File]</strong> </p> <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>ファイルの URL を入力し、添付ファイルの名前を指定します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### メンバー

+++ **[!UICONTROL ボードへのメンバーの割り当て]**

[ボード](#boards)の節の「[!UICONTROL ボードへのメンバーの割り当て]」を参照してください。

+++

+++ **[!UICONTROL ボードからのメンバーの割り当て解除]**

[ボード](#boards)の節の「[!UICONTROL ボードからのメンバーの割り当て解除]」を参照してください。

+++

+++ **[!UICONTROL カードへのメンバーの追加]**

このアクションモジュールは、指定のメンバーを指定のカードに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Enter card ID and member ID]</p> </td> 
   <td> <p>カード ID とメンバー ID の入力方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>「<strong>[!UICONTROL Card ID]</strong>」と「<strong>[!UICONTROL Member ID]</strong>」を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>メンバーの追加先となるカードが含まれるボードを選択し、カード、カード自体およびカードに追加するメンバーを含んだリストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メンバーの検索]**

このアクションモジュールは、[!UICONTROL Trello] メンバーに関する情報を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>検索するユーザーのフルネームまたはユーザー名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>デフォルトでは、このモジュールは、クエリ内の各単語の完全一致をメンバーコンテンツで検索します。[!UICONTROL Partial] が有効な場合、モジュールはクエリ内の任意の単語で始まるコンテンツを検索します。</p> <p> 例えば、「development」という単語を使用して「My Development Status Report」というタイトルのボードを検索する場合、デフォルトでは単語全体を検索する必要があります。[!UICONTROL Partial] を有効にしている場合、「dev」を検索することはできますが、「velopment」を検索することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned members]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 回の実行サイクルで返すメンバーの最大数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### チェックリスト

+++ **[!UICONTROL チェックリストの作成]**

このアクションモジュールは、選択されたカードにチェックリストを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> チェックリストを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>「<strong>[!UICONTROL Card ID]</strong>」フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>チェックリストの名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>チェックリストをカードの上部に追加するか、[!UICONTROL append the] チェックリストをカードの下部に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Enter checklist ID]</p> </td> 
   <td> <p>新規チェックリストにコピーするソースチェックリストの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL チェックリスト項目を作成]**

このアクションモジュールは、特定のチェックリストに項目を追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter checklist ID]</td> 
   <td> <p> 項目を追加するチェックリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>「<strong>[!UICONTROL Checklist ID]</strong>」フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カード、チェックリストの順に選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Item name]</p> </td> 
   <td> <p>新しい項目の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>項目をチェックリストの上部に追加するか、[!UICONTROL append] をチェックリストの下部に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Checked]</p> </td> 
   <td> <p>既にオンになっている項目を追加する場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL チェックリスト項目を編集]**

このアクションモジュールは、既存のチェックリストを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a Card ID and Checklist Item ID]</td> 
   <td> <p> 項目を編集するカードとチェックリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>「<strong>[!UICONTROL Checklist ID]</strong>」フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。</p> <p>「<strong>[!UICONTROL Checklist Item ID]</strong>」フィールドに、チェックリストの ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カード、チェックリストの順に選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checklist ID]</td> 
   <td>チェックリスト項目を移動するチェックリストを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Item name]</p> </td> 
   <td> <p>新しい項目の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>項目を上に追加するか、チェックリストの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>チェックリスト項目が完了したか未完了であるかを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### ラベル

+++ **[!UICONTROL カードにラベルを追加]**

このアクションモジュールは、選択したカードにラベルを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> チェックリストを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>「<strong>[!UICONTROL Card ID]</strong>」フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。「<strong>[!UICONTROL Label ID]</strong>」フィールドに、追加するラベルの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。 </p> <p>カードに追加するラベルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### コメント

+++ **[!UICONTROL コメントを監視]**

指定された場所に新しいコメントがある場合に、コメントの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched object]</td> 
   <td> <p>コメントを監視する場所を選択します。</p> 
    <ul> 
     <li><strong>あらゆる場所の [!UICONTROL All cards]</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>コメントを監視するボードを選択します</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>コメントを監視するリストが含まれるボードを選択し、リストを選択します。</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>コメントを監視するカードが含まれるボードを選択し、そのカードが含まれるリストを選択して、カードを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すコメントの最大数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードでコメントを作成]**

このアクションモジュールは、選択したカードにコメントを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> コメントを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL Card ID]</strong> フィールドに、コメントを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>コメントを追加するカードが含まれるボードを選択し、そのカードを含むリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment] </td> 
   <td> <p>選択したカードに追加するコメントを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カード内のコメントをリスト]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> コメントを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p><strong>[!UICONTROL Card ID]</strong> フィールドに、コメントを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>コメントを追加するカードが含まれるボードを選択し、そのカードを含むリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned comments]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 回の実行サイクルで返すコメントの最大数を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>コメントが作成された期間の開始日を設定します。サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before] </td> 
   <td> <p>コメントが作成された期間の終了日を設定します。サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] オブジェクト ID

* [ [!DNL Trello] でカードの ID やショートリンクを見つける方法](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [ [!DNL Trello] で他のオブジェクトの ID を見つける方法](#how-to-find-ids-of-other-objects-in-trello)

### [!DNL Trello] でカードの ID やショートリンクを見つける方法

カードを編集したり新しいコメントを作成したりする場合は、カードの ID やショートリンクを知っておく必要があります。[!UICONTROL 新しいカード]トリガーの出力から、この情報を入手できます。カードのショートリンクは、カードを開き、「[!UICONTROL 共有]」ボタンをクリックすることによっても取得できます。ショートリンクは、[!UICONTROL このカードへのリンク]ボックスで、`https://trello.com/c/` の後の URL 末尾にあります。

![](assets/share-and-more-350x575.png)

### [!DNL Trello] で他のオブジェクトの ID を見つける方法

ボード ID、リスト ID、コメント ID は、トリガーを使用してのみ取得できます。[!DNL trello.com] web サイトには、これらの ID は表示されません。
