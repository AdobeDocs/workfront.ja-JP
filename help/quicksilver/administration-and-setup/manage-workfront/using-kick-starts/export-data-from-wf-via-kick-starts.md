---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 「キックスタート」を使用してAdobe Workfrontからデータを書き出す
description: Adobe Workfront管理者は、Kick-Starts データエクスポータを使用してWorkfrontからデータを書き出すことができます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# 「キックスタート」を使用してAdobe Workfrontからデータを書き出す

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Adobe Workfront管理者は、Kick-Starts データエクスポータを使用してWorkfrontからデータを書き出すことができます。 書き出し後に他のアプリケーションで使用できます。

キックスタートを通じてデータを書き出すと、各オブジェクトに関連付けられているフィールド、これらのフィールドのコーディング方法、およびこれらのフィールドの値がデータベース内でどのように書式設定されるかを理解するのに役立ちます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## キックスタートを使用してデータを書き出すメリットとデメリット

Workfront内でデータを書き出すには、次の 2 つの方法があります。

* レポートまたはリストからのデータのエクスポート

   レポートまたはリストからのデータのエクスポートについて詳しくは、 [データを書き出し](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* キックスタートを使用したデータのエクスポート

次の表に、各方法の利点と欠点を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>エクスポートされたデータには、オブジェクトとフィールド値が含まれます</p> </th> 
   <th> <p>複数のオブジェクトタイプに関するデータを同時にエクスポートする機能</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>リスト表示からのデータのエクスポート</strong> </p> <p>リストからのデータのエクスポートについて詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">データを書き出し</a></p> </td> 
   <td> <p>はい</p> <p>Workfrontのネイティブフィールドと、オブジェクトに関連付けられているカスタムフィールドの両方が書き出されます。</p> </td> 
   <td> <p>いいえ</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>キックスタートを使用したデータのエクスポート</strong> </p> </td> 
   <td> <p>はい（限定）</p> <p>オブジェクトに関連付けられたWorkfrontのネイティブフィールドのほとんどは書き出されますが、書き出されないものもあります。 例えば、プロジェクトのキックスタートエクスポートを通じて、スケジュール、プロジェクト所有者、プロジェクトスポンサーの各フィールドをエクスポートすることはできません。</p> <p>カスタムフォームが添付されたプロジェクトでは、フォーム上のフィールドに入力されたデータは書き出されません。</p> <p>ただし、カスタムフォームを書き出すことはできます。 結果のファイルには、テキストボックスやラジオボタンなど、フォームに設定されたフィールドが一覧表示されます。</p> </td> 
   <td> <p>はい</p> <p>キックスタートを使用してWorkfrontデータをエクスポートすると、複数のオブジェクトタイプに関連するデータを 1 つのエクスポートでエクスポートできます。 例えば、タスク、イシューおよびプロジェクトを 1 回のエクスポートに含めることができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 書き出し制限

キックスタートを使用してデータを書き出す場合は、次の制限があります（データは Excel ファイル形式で書き出されます）。

* **50,000 行：** ファイルで許可される行数。
* **65,530 ハイパーリンク：** これは、65,530 個を超えるハイパーリンクを含むドキュメントに対して Excel が課す制限です。 これらのドキュメントは、書き出し後は開くことができません。 Excel ドキュメントのデータは 200 行に過ぎませんが、ドキュメント内に 65,530 個を超えるリンクがある場合、ドキュメントは開きません。

## キックスタートを使用したデータのエクスポート

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **キックスタート** 次に、 **データを書き出す。**

1. 書き出すオブジェクトを選択します。
1. クリック **その他のオプション** オブジェクトの完全なリストを表示するには、を参照してください。

   ここに示すすべてのオブジェクトは、データをWorkfrontにインポートする際にも使用できます。

   唯一の例外は **アクセスレベル** オブジェクト。 エクスポートに含まれる Access Levels データシートは、参照用としてのみ提供されています。 ID を使用して、新しいユーザーアカウントにアクセスレベルを割り当てることができます。

   キックスタートを使用してWorkfrontにデータを読み込む方法について詳しくは、 [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). 次に、キックスタートを使用して書き出すことができるすべてのオブジェクトのリストを示します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>オブジェクト</p> </th> 
      <th> <p>Excel ファイルのエクスポート済みシート</p> </th> 
      <th> <p>書き出し形式</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">アクセスレベル</td> 
      <td scope="col" valign="top">アクセスレベル<br>環境設定</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">割り当て</td> 
      <td scope="col" valign="top">割り当て<br>環境設定</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">会社</td> 
      <td scope="col" valign="top"> 会社<br>環境設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">E メール テンプレート</td> 
      <td scope="col" valign="top"> メールテンプレート<br>環境設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">費用</td> 
      <td valign="top"> 費用<br>環境設定 </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">外部ページ</td> 
      <td valign="top"> 外部ページ<br>環境設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">フィルター</td> 
      <td valign="top"> フィルター<br>環境設定 </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">グループ</td> 
      <td valign="top"> グループ<br>環境設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">グループ化</td> 
      <td valign="top"> グループ化<br>環境設定 </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">時間</td> 
      <td valign="top"> 時間<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">問題</td> 
      <td valign="top"> 問題<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">担当業務</td> 
      <td valign="top"> ジョブの役割<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">マイルストーン パス</td> 
      <td valign="top"> マイルストーン<br>マイルストーンパス<br>環境設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">メモ</td> 
      <td valign="top"> 注意<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">ポートフォリオ</td> 
      <td valign="top"> Portfolio<br>環境設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">プロジェクト</td> 
      <td valign="top"> キュー<br>プロジェクト<br>ルーティングルール<br>トピックをキュー<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">リソース見積り</td> 
      <td valign="top"> リソースの推定<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">リソース プール</td> 
      <td valign="top"> リソースプール<br>環境設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">危険</td> 
      <td valign="top"> リスク<br>環境設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">危険タイプ</td> 
      <td valign="top"> リスクタイプ<br>環境設定  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">スコアカード</td> 
      <td valign="top">スコアカードに関する質問<br>スコアカードオプション<br>スコアカード<br>環境設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">タスク</td> 
      <td valign="top"> タスク<br>環境設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">テンプレート</td> 
      <td valign="top"> キュー<br>テンプレート<br>ルーティングルール<br>トピックをキュー<br>環境設定 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">テンプレート割り当て</td> 
      <td valign="top"> テンプレート割り当て<br>環境設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">テンプレート タスク</td> 
      <td valign="top"> テンプレートタスク<br>環境設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">タイムシート</td> 
      <td valign="top"> タイムシートプロファイル<br>タイムシート<br>環境設定 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> ビュー </td> 
      <td valign="top"> 表示<br>環境設定  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **ダウンロード。**

   書き出されたキックスタートファイルは、Excel ファイルまたはとしてコンピューターにダウンロードされます。 複数の Excel およびプロパティファイルを含む zip ファイル。 各 Excel ファイルはシートの集まりで、各シートは選択したオブジェクトに関連付けられたフィールドを表します。 ここに **プロパティ** すべての書き出しに関連付けられたシート。

   この **ダッシュボード** および **レポート** 「 」オプションを使用すると、ダウンロードに含める特定のダッシュボードとレポートを選択できます。 書き出しできるのは、システム全体で共有されるダッシュボードのみです。

   マトリックスレポートを書き出すことはできません。 マトリックスレポートの詳細については、 [マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   1 回の書き出しで、最大 100 個のダッシュボードと 100 個のレポートを選択できます。

   ![](assets/kickstart-export-350x381.png)

   一度に複数のオブジェクトを書き出すことができます。

   デフォルトでは、次のオブジェクトが **含めるもの** ラベル（クリックする前） **その他のオプション**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>オブジェクト</strong> </p> </th> 
      <th> <p><strong>Excel ファイルのエクスポート済みシート</strong> </p> </th> 
      <th> <p> <strong>書き出し形式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>ダッシュボード</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>パラメータ<br>パラメーターオプション<br>パラメータグループ<br>カテゴリパラメータ<br>カテゴリ<br>レポート<br>「ポータル」タブセクション<br>ダッシュボード<br>環境設定</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>レポート</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">パラメータ<br>パラメーターオプション<br>パラメータグループ<br>カテゴリパラメータ<br>カテゴリ<br>レポート<br>環境設定</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>承認</p> </td> 
      <td scope="col" valign="top"> <p>ステップ承認者<br>承認ステップ<br>承認<br>承認プロセス<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>カスタムデータ</p> </td> 
      <td scope="col" valign="top"> <p>パラメータ<br>パラメーターオプション<br>パラメータグループ<br>カテゴリパラメータ<br>カテゴリ<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>費用タイプ</p> </td> 
      <td valign="top"> <p>費用タイプ<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>時間タイプ</p> </td> 
      <td valign="top"> <p>時間タイプ<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>チーム</p> </td> 
      <td valign="top"> チームメンバー<br>チーム<br>環境設定 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>ユーザー</p> </td> 
      <td valign="top"> <p>ユーザー<br>環境設定</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Excel ファイルのエクスポート済みシート</strong> </p> </th> 
      <th> <p> <strong>書き出し形式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>ダッシュボード</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>パラメータ<br>パラメーターオプション<br>パラメータグループ<br>カテゴリパラメータ<br>カテゴリ<br>レポート<br>「ポータル」タブセクション<br>ダッシュボード<br>環境設定</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>レポート</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">パラメータ<br>パラメーターオプション<br>パラメータグループ<br>カテゴリパラメータ<br>カテゴリ<br>レポート<br>環境設定</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>承認</p> </td> 
      <td scope="col" valign="top"> <p>ステップ承認者<br>承認ステップ<br>承認<br>承認プロセス<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>カスタムデータ</p> </td> 
      <td scope="col" valign="top"> <p>パラメータ<br>パラメーターオプション<br>パラメータグループ<br>カテゴリパラメータ<br>カテゴリ<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>費用タイプ</p> </td> 
      <td valign="top"> <p>費用タイプ<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>時間タイプ</p> </td> 
      <td valign="top"> <p>時間タイプ<br>環境設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>チーム</p> </td> 
      <td valign="top"> チームメンバー<br>チーム<br>環境設定 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>ユーザー</p> </td> 
      <td valign="top"> <p>ユーザー<br>環境設定</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （推奨）エクスポートされたデータを分析し、表示するはずのすべての情報がエクスポートされたことを確認します。

   大規模な書き出しの場合、Workfrontはバックグラウンドで Excel ファイルを生成し、遅延に関する警告メッセージを表示します。 ダウンロードが完了すると、キックスタートファイルが電子メールで送信されます。

   ![](assets/large-kick-start-file-warning-350x65.png)
