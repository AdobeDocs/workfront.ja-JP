---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: トレロモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Trello を使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5039'
ht-degree: 0%

---

# [!UICONTROL トレロ] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL トレロ]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Trello] モジュールの場合、 [!UICONTROL トレロ] アカウント

## 接続 [!UICONTROL トレロ] から [!DNL Workfront Fusion]

接続方法 [!UICONTROL トレロ] アカウント [!DNL Workfront Fusion]を参照してください。 [への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL トレロ] モジュールとそのフィールド

設定時に [!UICONTROL トレロ] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!UICONTROL トレロ] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [ボード](#boards)
* [リスト](#lists)
* [カード](#cards)
* [メンバー](#members)
* [チェックリスト](#checklists)
* [ラベル](#labels)
* [コメント](#comments)

### ボード

+++ **[!UICONTROL ウォッチボード]**

このトリガーモジュールは、新しいボードが追加されるとシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>ボードの最大数 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードの作成]**

このアクションモジュールは、選択した設定で新しいボードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>新しいボードの名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ]</td> 
   <td> <p>必要に応じて、ボードの説明を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 組織 ID]</p> </td> 
   <td> <p>組織の ID を入力またはマッピングします。 組織 ID は、監視アクティビティモジュールなど、別のモジュールを使用して取得できます。</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 権限レベル ]</p> </td> 
   <td> <p>ボードには、権限レベルごとに異なる投票およびコメントルールがあります。 例：ボードが [!UICONTROL Private] で、投票ルールとコメントルールを [!UICONTROL All] として設定している場合は、エラーが表示されます。 </p> <p>投票とコメントは、権限レベルごとに次のグループに制限されます。</p> 
    <ul> 
     <li><strong>[!UICONTROL プライベート ]</strong>:—&gt; メンバー、メンバーおよび監視者</li> 
     <li><strong>[!UICONTROL 組織用 ]</strong>:—&gt; メンバー、メンバーおよび監視者、組織メンバー</li> 
     <li><strong>[!UICONTROL パブリック ]</strong>:—&gt; メンバー、メンバーおよび監視者、組織メンバー、すべて</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 投票 ]</p> </td> 
   <td> <p>このボードで投票できる人を指定するオプションを選択します。 権限レベルでの投票制限については、「 [!UICONTROL 権限レベル ] 」フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL コメント ]</p> </td> 
   <td> <p>このボードのカードにコメントできるユーザーを指定するオプションを選択します。 権限レベルの制限については、 [!UICONTROL 権限レベル ] フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL の招待 ]</p> </td> 
   <td> <p>他のユーザーをこのボードに招待できるユーザーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 自己結合 ]</p> </td> 
   <td> <p>チームメンバーが自分でボードに参加できるか、招待する必要があるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL デフォルトのラベル ]</p> </td> 
   <td> <p>新しいボードにデフォルトのラベルセットを使用するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL デフォルトリスト ]</p> </td> 
   <td> <p>デフォルトのリストセットをボードに追加するか（[!UICONTROL タスク ]、[!UICONTROL 実行 ]、[!UICONTROL 完了 ]）を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ボードソース ID]</p> </td> 
   <td> <p>新しいボードにコピーするボードの ID を選択またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL カードカバー ]</p> </td> 
   <td> <p>選択 <strong>[!UICONTROL はい ]</strong> ボードのカードカバーを有効にする場合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 背景 ]</p> </td> 
   <td> <p>背景の色またはカスタムの背景を選択します。</p> <p>注意：カスタム背景は、[!UICONTROL Trello Gold および Business Class] の購読者のみが使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL カードの古いバージョン ]</p> </td> 
   <td> <p>2 つのカードエージングモードから選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>:カードは年を取るにつれて徐々に透明になる。 </li> 
     <li><strong>[!UICONTROL Priate]</strong>:カードは年をとるにつれて、古い海賊の地図のように裂け、黄色く、き裂ける。</li> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ボード ID]</p> </td> 
   <td> <p>モジュールで作成するボードの一意の [!UICONTROL Trello] ID を入力またはマッピングします。 ボード ID は、Watch Boards モジュールなど、別のモジュールを使用して取得できます</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しい名前 ]</td> 
   <td> <p> ボードの新しい名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しい説明 ]</td> 
   <td> <p> 必要に応じて、新しいボードの説明を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 組織 ID]</p> </td> 
   <td> <p>モジュールで編集するボードの一意の [!UICONTROL Trello] ID を入力またはマッピングします。 ボード ID は、 [!DNL Watch Activities] モジュール。</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 購読 ] </td> 
   <td> <p>オプションを選択して、代理ユーザーがボードを購読するかどうかを指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 権限レベル ]</p> </td> 
   <td> <p>ボードには、権限レベルごとに異なる投票およびコメントルールがあります。 例：ボードが [!UICONTROL Private] で、投票ルールとコメントルールを [!UICONTROL All] として設定している場合は、エラーが表示されます。 </p> <p>投票とコメントは、権限レベルごとに次のグループに制限されます。</p> 
    <ul> 
     <li><strong>[!UICONTROL プライベート ]</strong>:—&gt; メンバー、メンバーおよび監視者</li> 
     <li><strong>[!UICONTROL 組織用 ]</strong>:—&gt; メンバー、メンバーおよび監視者、組織メンバー</li> 
     <li><strong>[!UICONTROL パブリック ]</strong>:—&gt; メンバー、メンバーおよび監視者、組織メンバー、すべて</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 投票 ]</p> </td> 
   <td> <p>このボードで投票できる人を指定するオプションを選択します。 権限レベルでの投票制限については、「 [!UICONTROL 権限レベル ] 」フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL コメント ]</p> </td> 
   <td> <p>このボードのカードにコメントできるユーザーを指定するオプションを選択します。 権限レベルの制限については、 [!UICONTROL 権限レベル ] フィールドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の招待 ] </td> 
   <td> <p>このボードに人を招待できるユーザーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 自己結合 ]</td> 
   <td> <p> チームメンバーが自分でボードに参加できるか、招待する必要があるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カードカバー ]</td> 
   <td> <p> このボードにカードカバーを表示するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 背景 ] </td> 
   <td> <p>背景の色またはカスタムの背景を選択します。</p> <p>注意：カスタム背景は、[!UICONTROL Trello Gold および Business Class] の購読者のみが使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 背景 ID]</td> 
   <td> <p> 「[!UICONTROL 背景 ]」フィールドでカスタム背景の使用を選択した場合は、使用する背景の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL カードの古いバージョン ]</p> </td> 
   <td> <p>2 つのカードエージングモードから選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>:カードは年を取るにつれて徐々に透明になる。 </li> 
     <li><strong>[!UICONTROL Priate]</strong>:カードは年をとるにつれて、古い海賊の地図のように裂け、黄色く、き裂ける。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダーフィードが有効になっています ]</td> 
   <td> <p> カレンダーフィードを有効にするかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;color&gt; ラベル名 ]</td> 
   <td> <p> 目的のカラーラベルに名前を割り当てます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アーカイブ ] </td> 
   <td> <p>ボードをアーカイブ（閉じる）するかどうかを指定するオプションを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードの取得]**

このアクションモジュールは、ボードの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ボード ID]</p> </td> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ ] </td> 
   <td> <p>情報を取得するボードの名前（または名前の一部）を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されるボードの最大数 ]</td> 
   <td> <p> ボードの最大数を入力 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。 この値は 1000 以下にする必要があります。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partial] </p> </td> 
   <td> <p>デフォルトでは、このモジュールは、クエリ内の各単語の完全一致をメンバーコンテンツで検索します。 [!UICONTROL の一部 ] が有効な場合、モジュールはクエリ内の任意の単語で始まるコンテンツを検索します。</p> <p> 例えば、「development」という単語を使用して「My Development Status Report」というタイトルのボードを検索する場合、デフォルトでは単語全体を検索する必要があります。 [!UICONTROL Partial] を有効にしている場合、「dev」を検索することはできますが、「development」を検索することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ] </td> 
   <td> <p>"mine"と入力するか、ボード ID のコンマ区切りリストをマップします。</p> </td> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ID]</td> 
   <td> <p> 閉じる、または再度開くボードの ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アーカイブまたはアーカイブ解除 ]</td> 
   <td> <p> ボードを閉じる（アーカイブ）か、再び開く（アーカイブ解除）かを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メンバーをボードに割り当てる]**

このアクションモジュールは、指定したボードにメンバーを割り当てます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ID]</td> 
   <td> <p> メンバーを追加するボードを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 電子メールアドレス ]</td> 
   <td> <p> ボードに追加するメンバーのメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メンバータイプ ]</p> </td> 
   <td> <p>ボードに追加するメンバーのタイプを選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>:ボード管理者は、ボード上で任意のボード操作を実行できます。</li> 
     <li><strong>[!UICONTROL 標準 ]</strong>:通常の部材は、単に基板の部材である。</li> 
     <li><strong>[!UICONTROL 監視者 ]</strong>:監視者は、ボードに対する読み取り専用アクセス権を持つメンバーです。 <br>オブザーバーは、[!UICONTROL Trello Business Class] のチームでのみ使用できます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フルネーム ]</td> 
   <td> <p> ボードに追加するユーザーのフルネームを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ボードからのメンバーの割り当て解除]**

このアクションモジュールは、ボードからメンバーを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ID]</td> 
   <td> <p> ユーザーを削除するボードの ID を入力（マップまたは選択）します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メンバー ] </td> 
   <td> <p>ボードから削除するメンバーを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### リスト

+++ **[!UICONTROL ウォッチカードがリストに移動しました]**

このトリガーモジュールは、カードが特定のリストに移動されるとアクティブになります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ]</td> 
   <td>カードを監視するリストを含むボードを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト ]</td> 
   <td>カードを監視するリストを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>カードの最大数 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL リストの作成]**

このアクションモジュールは、指定したボードにリストを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ID]</td> 
   <td> <p> リストを作成するボードの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>新しいリストの名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 位置 ] </td> 
   <td> <p>リストを上に追加するか、カードの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リストをコピー ]</td> 
   <td> <p> コピーするリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>手動で入力</strong> </p> <p>内 <strong>[!UICONTROL リスト ID]</strong> 」フィールドに、コピーするリストの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>コピーするリストを含むボードを選択し、リストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL リストの編集]**

このアクションモジュールは、既存のリストを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト ID]</td> 
   <td> <p> 更新するリストの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>リストの新しい名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ID]</td> 
   <td> <p> リストを移動するボードをマッピングまたは選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 位置 ] </td> 
   <td> <p>リストを上に追加するか、カードの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 購読済み ]</td> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL リスト ID]</p> </td> 
   <td> <p>情報を取得するリストの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### カード

+++ **[!UICONTROL 名刺]**

このトリガーモジュールは、新しいカードが追加されると有効になります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 監視オブジェクト ]</td> 
   <td> <p>カードを監視する場所を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL すべてのカード ]</strong> </li> 
     <li> <p><strong>特定のボードのカード</strong> </p> <p>カードを監視するボードを選択します</p> </li> 
     <li> <p><strong>[!UICONTROL 特定のリストのカード ]</strong> </p> <p>カードを監視するリストが含まれているボードを選択し、リストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>カードの最大数 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードの作成]**

このアクションモジュールは、選択したリストにカードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト ID を入力 ]</td> 
   <td> <p> カードを追加するリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL リスト ID]</strong> フィールドに、カードを追加するリストの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>コピーするリストを含むボードを選択し、リストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ] </td> 
   <td> <p>カードに追加するラベルごとに、ラベルの ID を入力します。 ID は、例えば [!UICONTROL ラベルの取得 ] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メンバー ]</td> 
   <td>カードに追加する各メンバーに対して、メンバーの ID を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>新しいカードの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 説明 ]</p> </td> 
   <td> <p>カードの説明を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 位置 ] </td> 
   <td> <p>カードを上に追加するか、[!UICONTROL 追加 ] を使用してリストの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 期限 ]</td> 
   <td> <p> カードの期限を入力します。 サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 期限 ]</td> 
   <td> <p> カードが期限に達したことを示すには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル URL]</td> 
   <td> <p>カードに添付ファイルとして追加するファイルの URL を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ソースファイル ]</p> </td> 
   <td> <p>カードに添付ファイルとして追加するファイルの情報を入力またはマップします。</p> 
    <ul> 
     <li>[!UICONTROL ファイル名 ]:ファイル拡張子を含むファイル名を入力またはマッピングします。</li> 
     <li> 
     <p>前のモジュールからファイルを選択するか、ファイルの名前とデータをマップします</p> 
     <p>注意：ファイルのアップロードには、添付ファイルあたり 10 MB の制限があります。 ただし、[!UICONTROL Business Class] メンバーと [!UICONTROL Trello Gold] メンバーには、添付ファイルあたり 250 MB のファイルアップロード制限があります。</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カードをコピー ]</td> 
   <td> <p> コピーするカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> 」フィールドに、コピーするカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>コピーするカードが含まれるボードを選択し、そのカードを含むリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードの編集]**

このアクションモジュールは、既存のカードを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> 編集するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> フィールドに、編集するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>編集するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しい名前 ]</td> 
   <td> <p>カードの新しい名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 新しい説明 ]</p> </td> 
   <td> <p>カードの新しい説明を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL カードの移動 ]</p> </td> 
   <td> <p>ボードまたはボードを選択し、カードを移動する場所のリストを表示します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ] </td> 
   <td> <p>カードに追加するラベルの ID を追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 位置 ] </td> 
   <td> <p>カードを上に追加するか、[!UICONTROL 追加 ] を使用してリストの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 期限 ]</td> 
   <td> <p> カードの期限を入力します。 サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 期限 ]</td> 
   <td> <p> このオプションを有効にすると、カードは期限に完了とマークされます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メンバー ] </td> 
   <td> <p>カードに追加するメンバーの ID を追加またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイルカバー ID]</p> </td> 
   <td> <p>カードのカバーとして使用する画像添付ファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 購読 ] </td> 
   <td> <p>メンバーがカードを購読する必要があるかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アーカイブ ] </td> 
   <td> <p>カードをアーカイブ（閉じる）するかどうかを指定するオプションを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードの入手]**

このアクションモジュールは、選択したカードの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ID]</td> 
   <td> <p>詳細を取得するカードが含まれるボードの ID を入力します。 これにより、ボードのカスタムフィールドの名前を確認できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> 詳細を取得するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> 「 」フィールドに、詳細を取得するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>詳細を取得するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ボード ] </td> 
   <td> <p>検索するボードを選択します。 ボードが選択されていない場合は、すべてのボードが検索されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL クエリ ]</p> </td> 
   <td> <p>検索クエリを入力します。 次の検索演算子を使用して、検索を絞り込むことができます。</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>「 — 」を任意の演算子に追加して、除外検索 ( 例： <code>[!UICONTROL -has:members]</code> をクリックして、メンバーが割り当てられていないカードを検索します。</p> </li> 
     <li><code><strong>@name</strong></code> <p>メンバーに割り当てられたカードを返します。 また、 <code>member:</code>. 用途 <code>@me</code> カードのみを含める場合。</p> </li> 
     <li><code><strong>#label</strong></code> <p>ラベル付きのカードを返します。 また、 <code>label:</code>. 例： <code>label:"FIX IT"</code> は「FIX IT」というラベルのカードを返します。</p> </li> 
     <li><code><strong>board:id</strong></code> <p>特定のボード内のカードを返します。 例： <code>board:Trello</code> は、ボード名に [!UICONTROL Trello] が含まれるボードにカードを返します。</p> </li> 
     <li><code><strong>list:name</strong></code> <p>「name」という名前のリスト内のカードを返します。</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>添付ファイル付きのカードを返します。 この <code>has</code>:演算子は、 <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>または <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>24 時間以内に期限切れのカードを返します。 この <code>due:</code> 演算子は、 <code>due:week</code>, <code>due:month</code>または <code>due:overdue</code>. また、特定の日の範囲を検索することもできます。 例： <code>due:14</code> 検索には、今後 14 日以内に期限が切れるカードが含まれます。</p> </li> 
     <li><code><strong>created:day</strong></code> <p>過去 24 時間に作成されたカードを返します。 この<code> created:</code> 演算子は、 <code>created:week</code> または <code>created:month</code>. また、特定の日の範囲を検索することもできます。 例： <code>created:14</code> 「 」では、過去 14 日間に作成されたカードが検索に含まれます。</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>過去 24 時間に編集されたカードを返します。 この <code>edited:</code> 演算子は、 <code>edited:week</code> または <code>edited:month</code>. また、特定の日の範囲を検索することもできます。 例： <code>edited:21</code> を検索するには、過去 21 日間に編集されたカードが含まれます。</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>カードの説明、チェックリスト、コメント、名前のテキストに一致するカードを返します。 例えば、comment:"FIX IT"はコメントに"FIX IT"を含むカードを返します。</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>開いているまたはアーカイブされているカードを返します。 どちらも指定されていない場合、[!UICONTROL Trello] は両方の型を返します。</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>スター付きのボードのカードのみが含まれます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されるカードの最大数 ]</td> 
   <td> <p> カードの最大数 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。 この値は 1000 以下にする必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>デフォルトでは、このモジュールは、クエリ内の各単語の完全一致をメンバーコンテンツで検索します。 [!UICONTROL の一部 ] が有効な場合、モジュールはクエリ内の任意の単語で始まるコンテンツを検索します。</p> <p> 例えば、「development」という単語を使用して「My Development Status Report」というタイトルのボードを検索する場合、デフォルトでは単語全体を検索する必要があります。 [!UICONTROL Partial] を有効にしている場合、「dev」を検索することはできますが、「development」を検索することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ] </td> 
   <td> <p>特に検索するカードを追加します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードのアーカイブまたはアーカイブ解除]**

このアクションモジュールは、カードをアーカイブするか、ボードに送り返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID]</td> 
   <td> <p> アーカイブするカードの ID を入力またはマッピングするか、ボードに送り返します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アーカイブまたはアーカイブ解除 ]</td> 
   <td> <p> カードを閉じる（アーカイブ）か、ボードに送り返す（アーカイブ解除）かを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 添付ファイルを追加]**

このアクションモジュールは、選択したカードに添付ファイルを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> 詳細を取得するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>手動で入力</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> 「 」フィールドに、詳細を取得するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>詳細を取得するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイルの種類 ]</p> </td> 
   <td> <p>ファイルを直接アップロードするか、ファイルの URL を指定するかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル ]</strong> </p> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>ファイルの URL を入力し、添付ファイルの名前を指定します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### メンバー

+++ **[!UICONTROL メンバーをボードに割り当てる]**

参照：[!UICONTROL メンバーをボードに割り当てる]」の下に [ボード](#boards).

+++

+++ **[!UICONTROL ボードからのメンバーの割り当て解除]**

参照：[!UICONTROL ボードからのメンバーの割り当て解除]」の下に [ボード](#boards).

+++

+++ **[!UICONTROL カードへのメンバーの追加]**

このアクションモジュールは、指定されたメンバーを指定されたカードに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL カード ID とメンバー ID を入力 ]</p> </td> 
   <td> <p>カード ID とメンバー ID の入力方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL カード ID]</strong> そして <strong>[!UICONTROL メンバー ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>メンバーを追加するカードが含まれるボードを選択し、カードを含むリスト、カード自体、およびカードに追加するメンバーを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メンバーを検索]**

このアクションモジュールは、 [!UICONTROL トレロ] メンバー。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ ] </td> 
   <td> <p>検索するユーザーのフルネームまたはユーザー名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>デフォルトでは、このモジュールは、クエリ内の各単語の完全一致をメンバーコンテンツで検索します。 [!UICONTROL の一部 ] が有効な場合、モジュールはクエリ内の任意の単語で始まるコンテンツを検索します。</p> <p> 例えば、「development」という単語を使用して「My Development Status Report」というタイトルのボードを検索する場合、デフォルトでは単語全体を検索する必要があります。 [!UICONTROL Partial] を有効にしている場合、「dev」を検索することはできますが、「development」を検索することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されるメンバーの最大数 ]</td> 
   <td> <p> メンバーの最大数 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### チェックリスト

+++ **[!UICONTROL チェックリストを作成]**

このアクションモジュールは、選択したカードにチェックリストを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> チェックリストを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>チェックリストの名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 位置 ] </td> 
   <td> <p>チェックリストを上に追加するか、[!UICONTROL] チェックリストをカードの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL チェックリスト ID を入力 ]</p> </td> 
   <td> <p>新しいチェックリストにコピーするソースチェックリストの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL チェックリスト項目の作成]**

このアクションモジュールは、特定のチェックリストに項目を追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チェックリスト ID を入力 ]</td> 
   <td> <p> 項目を追加するチェックリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL チェックリスト ID]</strong> フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択し、チェックリストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 項目名 ]</p> </td> 
   <td> <p>新しい項目の名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 位置 ]</p> </td> 
   <td> <p>チェックリストの上部に項目を追加するか、下部に [!UICONTROL append] を追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL チェック済み ]</p> </td> 
   <td> <p>既にオンにして項目を追加する場合は、このオプションを有効にします。</p> </td> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID とチェックリスト項目 ID を入力 ]</td> 
   <td> <p> 項目を編集するカードとチェックリストの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL チェックリスト ID]</strong> フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。</p> <p>内 <strong>[!UICONTROL チェックリスト項目 ID]</strong> フィールドに、チェックリストの ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択し、チェックリストを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チェックリスト ID]</td> 
   <td>チェックリスト項目を移動するチェックリストを選択またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 項目名 ]</p> </td> 
   <td> <p>新しい項目の名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 位置 ]</p> </td> 
   <td> <p>項目を上に追加するか、チェックリストの下に追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 状態 ]</p> </td> 
   <td> <p>チェックリスト項目が完了したか不完全であるかを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### ラベル

+++ **[!UICONTROL カードへのラベルの追加]**

このアクションモジュールは、選択したカードにラベルを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> チェックリストを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> フィールドに、チェックリストを追加するカードの ID を入力またはマッピングします。 内<strong>[!UICONTROL ラベル ID]</strong> 「 」フィールドで、追加するラベルの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>チェックリストを追加するカードが含まれるボードを選択し、カードが含まれるリストを選択して、カードを選択します。 </p> <p>カードに追加するラベルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### コメント

+++ **[!UICONTROL コメントを見る]**

指定された場所に新しいコメントがある場合に、コメントの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 監視オブジェクト ]</td> 
   <td> <p>コメントを監視する場所を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL すべてのカード ] を至る所に</strong> </li> 
     <li> <p><strong>[!UICONTROL ボード ]</strong> </p> <p>コメントを監視するボードを選択</p> </li> 
     <li> <p><strong>[!UICONTROL リスト ]</strong> </p> <p>コメントを監視するリストが含まれるボードを選択し、リストを選択します。</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>コメントを閲覧するカードが含まれるボードを選択し、そのカードが含まれるリストを選択して、カードを選択します。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>コメントの最大数 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カードでのコメントの作成]**

このアクションモジュールは、選択したカードにコメントを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> コメントを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> 「 」フィールドで、コメントを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>コメントを追加するカードが含まれるボードを選択し、そのカードを含むリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コメント ] </td> 
   <td> <p>選択したカードに追加するコメントを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カード内のコメントのリスト]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>[!UICONTROL Trello] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カード ID を入力 ]</td> 
   <td> <p> コメントを追加するカードの ID を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL カード ID]</strong> 「 」フィールドで、コメントを追加するカードの ID を入力またはマッピングします。<br></p> </li> 
     <li> <p><strong>[!UICONTROL 選択 ]</strong> </p> <p>コメントを追加するカードが含まれるボードを選択し、そのカードを含むリストを選択して、カードを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されたコメントの最大数 ]</td> 
   <td> <p> コメントの最大数を入力 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>コメントが作成された期間の開始日を設定します。 サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before] </td> 
   <td> <p>コメントが作成された期間の終了日を設定します。 サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL トレロ] オブジェクト ID

* [でカードの ID やショートリンクを見つける方法 [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [で他のオブジェクトの ID を見つける方法 [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### でカードの ID やショートリンクを見つける方法 [!DNL Trello]

カードを編集したり新しいコメントを作成したりする場合は、カードの ID またはそのショートリンクを知っておく必要があります。 この情報は、 [!UICONTROL 新しいカード] トリガー。 カードのショートリンクは、カードを開き、 [!UICONTROL 共有] 」ボタンをクリックします。 ショートリンクは [!UICONTROL このカードへのリンク] ボックスに、URL の末尾に `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### で他のオブジェクトの ID を見つける方法 [!DNL Trello]

ボード ID、リスト ID、コメント ID は、トリガーを使用してのみ取得できます。 この [!DNL trello.com] web サイトには、これらの ID は表示されません。
