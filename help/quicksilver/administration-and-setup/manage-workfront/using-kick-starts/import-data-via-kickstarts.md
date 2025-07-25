---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: キックスタートテンプレートを使用したWorkfrontへのデータの読み込み
description: キックスタートは、Workfront に読み込むデータを入力できる特別な形式の Excel ワークブックです。「キックスタートデータインポーター」で説明されているように、Adobe Workfront には、そのためのキックスタートテンプレートが用意されています。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '2851'
ht-degree: 92%

---

# キックスタートテンプレートを使用したWorkfrontへのデータの読み込み

<!--Audited: 12/2023-->

キックスタートは、Workfront に読み込むデータを入力できる特別な形式の Excel ワークブックです。[キックスタートデータインポーター](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md)で説明されているように、Adobe Workfront には、そのためのキックスタートテンプレートが用意されています。

このプロセスは、3 つの主なタスクに分かれています。

* まず、キックスタートテンプレートをスプレッドシートファイルとして書き出します。
* 次に、スプレッドシートにデータを入力します
* 最後に、入力済みのスプレッドシートを Workfront に読み込みます

この記事では、これらの手順について、適切な順序で説明します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p> 新規：標準</p>
   または
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 制限事項

キックスタートテンプレートを使用して、Workfront に多数のオブジェクトを読み込むことができます。ただし、次の制限事項に注意してください。

* この方法でデータを読み込んでも、Workfront に既に存在するレコードの情報は更新されません。
* 読み込めるのは、新しいレコードとその情報のみです。
* 読み込みがタイムアウトしないように、一度に読み込むレコードを 2,000 件以下にします

## キックスタートテンプレートをスプレッドシートファイルとして書き出す

キックスタートテンプレートを書き出すと、空の Excel スプレッドシートワークブックが表示されます。スプレッドシートがコンピューターにダウンロードされたら、それを使用して情報を入力し、再び Workfront に読み込むことができます。

キックスタートテンプレートを書き出すには、次の手順に従います。

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  -->

1. **システム**／**データを読み込み（キックスタート）**&#x200B;をクリックします。

1. 含める情報のタイプを選択します。

   選択した各オプションは、書き出されたスプレッドシート内の複数のタブのコレクションを表します。たとえば、「**レポート**」オプションを選択した場合は、レポートの作成に必要なすべてのオブジェクト（ビュー、フィルター、グループ化、レポート）がスプレッドシートに含まれます。

   下記のすべてのオブジェクトタイプを使用して、データを Workfront に読み込むことができます。（唯一の例外は、「アクセスレベル」オプションです。書き出されたアクセスレベルデータシートは、参照用に提供されています。ID に基づいて、新しいユーザーアカウントにアクセスレベルを割り当てることができます）。

   各オブジェクトタイプのテンプレートは、次のファイル形式で書き出すことができ、次のシートを含んでいます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>オブジェクト</strong> </p> </th> 
      <th> <p><strong>書き出し形式</strong> </p> </th> 
      <th> <p><strong>書き出されたスプレッドシート内のシート</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>ダッシュボード</p> <p>システム内の公開されている共有ダッシュボードはすべてエクスポートできます。 システム全体で共有されていないダッシュボードは書き出せません。 1 回の書き出しで最大 100 個の特定のダッシュボードを選択できます。</p> </td> 
      <td scope="col">ZIP ファイルとして書き出し</td> 
      <td scope="col"> <p>パラメーター</p> <p>説明テキスト</p><p>パラメーターオプション</p> <p>パラメーターグループ</p> <p>カテゴリパラメーター</p> <p>カテゴリ</p> <p>レポート</p> <p>ポータルのタブセクション</p> <p>ダッシュボード</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>レポート</p> <p>システム内のすべてのレポートを書き出すことができます。1 回の書き出しで、最大 100 個の特定のレポートを選択できます。</p> <p>キックスタートは、テキストモードのフィルターやグループ化をサポートしていません。 正常に書き出すには、レポートフィルターとグループ化を標準モードに切り替える必要があります。</p> </td> 
      <td scope="col">ZIP ファイルとして書き出し </td> 
      <td scope="col"> <p scope="col">パラメーター</p> <p scope="col">説明テキスト</p> <p scope="col">パラメーターオプション</p> <p scope="col">パラメーターグループ</p> <p scope="col">カテゴリパラメーター</p> <p scope="col">カテゴリ</p> <p scope="col">レポート</p> <p scope="col">環境設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>承認</p> </td> 
      <td scope="col"> <p>Excel ファイルとして書き出し</p> </td> 
      <td scope="col"> <p>ステージ承認者</p> <p>承認ステージ</p> <p>承認</p> <p>承認プロセス</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>カスタムデータ</p> </td> 
      <td scope="col"> <p>Excel ファイルとして書き出し</p> </td> 
      <td scope="col"> <p>パラメーター</p> <p>説明テキスト</p>  <p>パラメーターオプション</p> <p>パラメーターグループ</p> <p>カテゴリパラメーター</p> <p>カテゴリ</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>費用タイプ</p> </td> 
      <td scope="col"> <p>Excel ファイルとして書き出し</p> </td> 
      <td> <p>費用タイプ</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td> <p>時間タイプ</p> </td> 
      <td scope="col"> <p>Excel ファイルとして書き出し</p> </td> 
      <td> <p>時間タイプ</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td> <p>チーム</p> </td> 
      <td scope="col"> <p>Excel ファイルとして書き出し</p> </td> 
      <td> <p> チームメンバー</p> <p>チーム</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>ユーザー</p> </td> 
      <td> <p>Excel ファイルとして書き出します。オプションの完全なリストを表示するには、「<strong>その他のオプション</strong>」をクリックします。</p> </td> 
      <td> <p>ユーザー</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td>アクセスレベル</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p>アクセスレベル</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td>割り当て</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p>割り当て</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td>会社</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> 会社</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>メールテンプレート</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p>メールテンプレート</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>費用</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> 費用'</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>外部ページ</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> 外部ページ</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>フィルター</td> 
      <td>ZIP ファイルとして書き出し</td> 
      <td> <p> フィルター</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>グループ</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> グループ</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>グループ化</td> 
      <td>ZIP ファイルとして書き出し</td> 
      <td> <p> グループ化</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>時間</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> 時間</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>イシュー</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> イシュー</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>担当業務</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> 担当業務</p> <p>環境設定 </p> </td> 
     </tr>

   <tr> 
      <td>マイルストーンパス</td> 
      <td> Excel ファイルとして書き出し</td> 
      <td> <p> マイルストーン</p> <p>マイルストーンパス</p> <p>環境設定 </p> </td> 
     </tr>

   <tr> 
      <td>メモ</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> メモ</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>ポートフォリオ</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> ポートフォリオ</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>プロジェクト</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> キュー</p> <p>プロジェクト</p> <p>ルーティングルール</p> <p>キューのトピック</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>リソース見積り</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> リソース見積り</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>リスク</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> リスク</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>リスクタイプ</td> 
      <td> Excel ファイルとして書き出し</td> 
      <td> <p> リスクタイプ</p> <p>環境設定</p> </td> 
     </tr> 
     <tr> 
      <td>スコアカード</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p>スコアカードの質問</p> <p>スコアカード オプション</p> <p>スコアカード</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>タスク</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> タスク</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>テンプレート</td> 
      <td> Excel ファイルとして書き出し</td> 
      <td> <p> キュー</p> <p>テンプレート</p> <p>ルーティングルール</p> <p>キューのトピック</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>テンプレートの割り当て</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> テンプレートの割り当て</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>テンプレートタスク</td> 
      <td>Excel ファイルとして書き出し</td> 
      <td> <p> テンプレート タスク</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>タイムシート</td> 
      <td> Excel ファイルとして書き出し</td> 
      <td> <p> 定期タイムシート</p> <p>タイムシート</p> <p>環境設定 </p> </td> 
     </tr> 
     <tr> 
      <td>表示 </td> 
      <td> <p>ZIP ファイルとして書き出し</p> </td> 
      <td> <p> 表示</p> <p>環境設定 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**ダウンロード**」をクリックします。
1. 「[スプレッドシートテンプレートにデータを入力する](#populate-the-spreadsheet-template-with-your-data)」に進み、空のテンプレートのスプレッドシートに情報を入力します。

## スプレッドシートテンプレートにデータを入力する {#populate-the-spreadsheet-template-with-your-data}

* [スプレッドシートに含まれるタブ（データシート）の概要](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [レコードを読み込む](#import-a-record)
* [日付を含める](#include-dates)
* [ワイルドカードを使用](#use-wildcards)
* [ID の属性名の置換](#attribute-name-substitution-for-ids)

### スプレッドシートに含まれるタブ（データシート）の概要

>[!TIP]
>
>キックスタートテンプレートにデータを入力するときに、各列の情報をどのようにフォーマットする必要があるかをより深く理解するには、読み込もうとしているオブジェクトの既存の Workfront データを含むキックスタートを書き出して、練習を実行することを検討してください。手順については、[キックスタートを介して Adobe Workfront からデータを書き出す](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)を参照してください。

空のキックスタートテンプレートを開くと、多数のタブ（データシート）を使用できます。これらは、ダウンロード対象として選択したオブジェクトによって異なります。各オブジェクトは、プロジェクト、タスク、時間、ダッシュボード、ユーザーなど、アプリケーション内の 1 つのオブジェクトを表します。

これらのタブの 1 つを開くと、行 2 には読み込み時に設定できる各オブジェクトのフィールドが表示されます。列ヘッダーでは、「設定」という単語の後に、データベース内での表示に従ってフィールドの名前が表示されます。これらのフィールドは、列ヘッダーとして機能します。

>[!IMPORTANT]
>
>エラーを回避するには、次の点を確認します。
>
>* キックスタートスプレッドシートの最初の空行を削除しないでください。
>* これらのフィールド（列のヘッダー）は削除、変更、入れ替えを行わないでください。例えば、順序や名前は変更しないでください。
>* 列ヘッダーに太字で表示されるすべてのフィールドに値を追加します。これらは必須フィールドを表します。
>
>     ただし、必須フィールドにシステム環境設定で設定されたデフォルト値が含まれている場合は、入力する必要はありません。
>
>     例えば、「**PROJ プロジェクト**」タブ、「**setCondition**」および「**setConditionType**」フィールドを空のままにすることはできますが、「**setGroupID**」および「**setName**」列ではできません。
>
>* **setResourceRevenue** と **setEnteredByID** などの特定のフィールドは、システムによって自動的に生成されます。スプレッドシートのこれらのフィールドにデータを入力しても、スプレッドシートをアップロードする際にキックスタートプロセスによって上書きされます。

### レコードを読み込む  {#import-a-record}

シートの各行は、一意のオブジェクトに対応します。

1. **isNew** 列に情報を追加します。

   * 読み込むオブジェクトが新規の場合は、**TRUE** と入力して行にデータを読み込みます。この値は大文字と小文字が区別され、常に大文字の英字である必要があります
   * Workfront に既にオブジェクトがある場合は、**isNew** 列に **FALSE** と入力して行を無視します。この値は大文字と小文字が区別され、常に大文字の英字である必要があります

      * Workfront に既に存在するレコードは更新されません。
      * Workfront からデータを含むテンプレートをダウンロードした場合、既存のオブジェクトにはあらかじめ **FALSE** が付けられます。
      * 空のテンプレートをダウンロードした場合は、既存のオブジェクトに新しい行を追加する必要はありません。

1. 次のいずれかの方法で、**ID** 列に情報を追加します。

   * 読み込むオブジェクトが新規であり、**isNew** 列に **TRUE** と入力した場合は、ID に任意の数値を入力します。この数値は、スプレッドシート内で一意である必要があります。例えば、3 つのオブジェクトを読み込む場合、それぞれの ID に 1、2、3 を指定できます。

   * Workfront に既にオブジェクトが存在し、**isNew** 列に **FALSE** と入力し、かつ既存のオブジェクトに関する新しい情報を読み込む場合、ID は、Workfront に存在するそのオブジェクトの英数字の GUID である必要があります。

   >[!TIP]
   >
   > Workfront でオブジェクトの一意の GUID を調べるには、そのオブジェクトのレポートを作成してそのレポートに ID 列を追加します。その列の各オブジェクトの値は、オブジェクトの GUID です。

   * Workfront に既に存在するレコードは更新されません。
   * データを含むテンプレートをダウンロードした場合、既存のオブジェクトには GUID が既に ID として含まれています。
   * 既存のオブジェクトに基づいて新しいオブジェクトを読み込むには、**isNew** 列で **FALSE** を **TRUE** に変更し、ID を変更し、読み込む前に必要なデータの補正を行います。

   ![グループのサンプル ID](assets/kick-start-group-example.png)

   * プロジェクトを読み込む際には、グループ ID を指定する必要があります。

      * Workfront に既にグループが存在する場合は、プロジェクトの **setGroupID** フィールドに一意の ID を追加する必要があります。
      * Workfront にグループが存在しない場合は、**グループ**&#x200B;シートを読み込むファイルに追加し、グループシートの **isNew** フィールドを **TRUE** に設定し、**ID** 列で新規グループの数値 ID を指定します。新規プロジェクトの **setGroupID** フィールドは新規グループの数値 **ID** と一致する必要があります。

     **例：**&#x200B;プロジェクトの場合、**setGroupID** 列に表示される値は、次のいずれかに該当する必要があります。

      * Workfront インスタンス内の既存のグループの GUID
      * インポート中に新しいグループを作成する場合は、**「GROUP」グループ**&#x200B;シートの ID 列の値（数値）

1. 必須フィールドおよび読み込み時に入力するその他のフィールドの値を入力します。
1. （オプション）カスタムデータを追加するには、次の手順に従います。

   * 読み込み処理に含める各カスタムフィールドに対して新しい列を作成します。
   * 対応するカスタムフィールドの新しい各列に、**DE: [Workfront に表示されるカスタムフィールド名]**&#x200B;のように名前を付けます。例えば、「DE: 部門」というカスタムフィールドを作成できます。
   * **setCategoryID** 列に、このカスタムフィールドが存在する既存のカスタムフォームの GUID を入力します。このフィールドは、カスタムデータを読み込む際に必須です。
   * カスタムフィールドに複数のデータ値（ラジオボタン、チェックボックス、リストなど）を追加する必要がある場合は、「環境設定」タブに表示される縦棒のカスタムデータ区切り記号「|」を使用して値を区切ります。

     **例：** DE:Departments 列の下に A|D と入力すると、カスタムフォームに部門 A と部門 D が入力されます。

     >[!NOTE]
     >
     >区切り文字「|」のみを使用して、カスタムフィールドの値を区切ります。 **setCategoryID** など、他のスプレッドシート列では使用できません。

### 日付を含める  {#include-dates}

Workfront は、ほとんどの日付形式を処理できます。ただし、スプレッドシートの日付列が日付形式であることを確認する必要があります。列の形式が一般、数値、テキストの場合、読み込みは失敗します。

>[!TIP]
>
>最も一般的な形式は、MM/DD/YYYY 形式です。
>
>例：07/10/2023

Workfront では、日付の一部として時間値も使用できます。

例：07/10/2022 01:30 または 07/10/2022 1:00 PM

日付の時刻を省略した場合、Workfront は次のいずれかを実行します。

* 時刻が深夜の午前零時であると仮定します。期待する日付の結果を確認するには、システムのタイムゾーンがお使いのタイムゾーンと一致している必要があります。
* スケジュールに関連付けられたオブジェクト上にある場合、時間は、スケジュールが許可する最も早い時間に従います。

>[!NOTE]
>
>UNIX タイムスタンプを使用する場合、値の末尾に 3 つの追加のゼロを含める必要があります。
>
>例えば、タイムスタンプが 7336899000 の場合は、セルに 7336899000000 と入力します。

### ワイルドカードを使用 {#use-wildcards}

キックスタートテンプレートのスプレッドシートに入力する際に、以下のワイルドカードを使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>ワイルドカード</strong> </p> </th> 
   <th> <p><strong>動作</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p><strong>setDate</strong> フィールドに使用する場合、このワイルドカードは、キックスタートを読み込んだ日の午前 0 時に日付を設定します。</p> <p>ワイルドカードは、フィルターでワイルドカードと共に使用できる標準構文を使用して変更できます。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>実際に読み込みを実行する日に関係なく、読み込む週の月曜日にプロジェクトを開始する場合は、<strong>$$TODAYbw</strong> を使用します。これにより、プロジェクトの予定開始日が日曜日午前 12:00 に設定されます。プロジェクトのスケジュールは、その時点では作業を許可していない可能性があるので、月曜日の朝の 9 時に開始します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p><strong>setDate</strong> に使用する場合、このワイルドカードは、キックスタートの読み込み時にレコードを作成した時刻に従って日付を設定します。</p> <p>ワイルドカードは、フィルターでワイルドカードと共に使用できる標準構文を使用して変更できます。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>プロジェクトを読み込んでから 3 時間後に開始する場合は、<strong>$$NOW+3 h</strong> を使用します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p><strong>setAssignedToID</strong> または他の userID ベースのフィールドで使用する場合、このワイルドカードは作業を割り当てるか、レコードの読み込みを実行する個人に関連付けます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>このワイルドカードは、特にキックスタートユーザーの読み込み用に追加されました。Workfront アカウントを作成すると、システム管理者のアクセスレベルを持つユーザーが作成されます。デフォルトの管理者に割り当てられたユーザー名は、アカウントで他のユーザーを作成する際に接頭辞として使用できます。</p> <p>ユーザー名はすべての顧客で一意である必要があるため、これは、ユーザー名が「jsmith」の可能性がある John Smith など、非常に一般的なユーザー名を持つ複数の個人がいる場合に便利です。ユーザー名割り当ての前にデフォルトの管理者ユーザー名を付けると、各ユーザー名が一意であることが保証されます（例：<strong>$$CUSTOMER.jsmith</strong>）。</p> <p>ヒント：ユーザー名がシステム全体で一意であることを保証するより洗練された方法は、「<strong>setUsername</strong>」フィールドに個人のメールアドレスを入力することです。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ID の属性名の置換  {#attribute-name-substitution-for-ids}

可能な限り ID を使用することがベストプラクティスですが、**setAttributeID** 値を設定する際に、あるシートから別のシートへ ID を相互参照するのが不便な場合があります。列ヘッダーを変更するだけで、名前で値を参照できます。

**例：**

* **プロジェクトのインポート**

  プロジェクトを読み込む場合は、**GROUP Group** シートに移動してプロジェクトの **setGroupID** を設定し、それぞれのグループ ID をメモして **PROJ プロジェクト**&#x200B;シートの正しいセル（**setGroupID** 列）に貼り付けます。

  これは、少数のグループとプロジェクトで作業する場合に実行できますが、それぞれのグループを複数使用する場合は、実用的ではありません。

  上記の例で属性名の置換を行うには、**setGroupID** 列ヘッダーを **#setGroupID グループ名**&#x200B;に変更します。これにより、各プロジェクトのグループを名前で参照できるようになります。

  >[!NOTE]
  >
  >属性名の置き換えを使用するオプションは、既存のレコードの参照にのみ制限されます。同じ読み込みで作成するオブジェクトには、名前の置き換えを使用できません。

* **ユーザーの読み込み**

  ユーザーを読み込む際に、「**ROLE Role**」タブの役割のリストから **setRoleID** を入力します。

  役割 ID の一部は、アカウントに既に存在するレコード用で、その他は読み込み中に作成されます。

  既存の役割に割り当てられた新しいユーザーレコードに対して、名前の置換を使用できます。新しく読み込まれた役割に割り当てられた新しいユーザーレコードに対しては使用できません。

  同じ読み込みファイルで両方のメソッドを使用する方法を次に示します。

   * スプレッドシートの **setRoleID** 列の左側に列を追加します。
   * 新しい列に **#setRoleID ROLE name** という名前を付けます。
   * 既存のレコードに役割を割り当てる場合は、**#setRoleID ROLE name** 列に役割名を入力します。

     新しい役割レコードへの役割割り当ての場合は、ROLE Role シートの setRoleID に割り当てた ID を入力します。

     ![ユーザーの役割 ID](assets/set-role-id.png)

## スプレッドシートデータを Workfront に読み込む

Excel テンプレートにデータを入力した後、そのデータを Workfront にアップロードできます。

キックスタート読み込みでは、次のファイルタイプをサポートしています。

* Excel（.xls または .xlsx）
* 圧縮（.zip）ファイル（.xlsx ファイルまたは .xls ファイルのみを含む）

  >[!NOTE]
  >
  >次のオブジェクトを参照する Excel スプレッドシートをインポートする場合は、.zip ファイルを使用する必要があります。
  >
  >* レポート
  >* ドキュメント
  >* アバター
  >* プロパティファイルの表示、フィルタリング、グループ化
  >
  >zip 形式の読み込みファイルを使用する場合、.zip ファイルは .xlsx ファイルや .xls ファイルと同じ名前にする必要があり、すべてのファイルが同じ構造レベル（フォルダーなし）である必要があります。

テンプレートスプレッドシートデータを Workfront に読み込むには、以下の手順を実行します。

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. **システム**／**データを読み込み（キックスタート）**&#x200B;の順にクリックします。

1. **Kick-Start スプレッドシートを使用してデータをアップロードする** セクションで **ファイルを選択** をクリックし、入力されたスプレッドシートを参照して選択します。

   ファイルは自動的にアップロードされ、読み込みが成功したという通知が表示されます。

   Excel ファイルをWorkfrontにアップロードするのに 5 分以上かかる場合、アプリケーションはタイムアウトし、Workfrontはファイルをアップロードできません。 小さなオブジェクトのバッチでデータを読み込んでみてください。

1. （条件付き）読み込みに失敗した場合は、問題を示すエラーメッセージが表示されます。 問題が発生したフィールド、シート、および行番号を特定し、Excel ファイルの情報を修正します。 次に、もう一度ファイルを読み込んでみます。
1. （条件付き）Workfront Fusion を使用している場合、読み込みが完了したときに FLO またはシナリオを有効にできるようになりました。
