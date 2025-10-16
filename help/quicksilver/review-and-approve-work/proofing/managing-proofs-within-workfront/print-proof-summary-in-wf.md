---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Adobe Workfront 内でプルーフの概要を印刷
description: プルーフの概要を印刷したり、PDF として保存したり、Adobe Reader 向けに最適化された XLS ファイルまたは PDF ファイルとして書き出したりできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 90%

---

# Adobe Workfront 内でプルーフの概要を印刷

プルーフの概要を印刷したり、PDF として保存したり、Adobe Reader 向けに最適化された XLS ファイルまたは PDF ファイルとして書き出したりできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>標準</p>
   <p>作業またはプラン</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プルーフの概要を印刷または PDF ファイルとして保存

プルーフの概要は、ドキュメントリストから直接印刷できます。

>[!NOTE]
>
>* 1 GB を超えるサマリーはサポートされていません。
>* ドキュメントリストから複数のプルーフの概要を同時に印刷することはできません。

1. プルーフを含むドキュメントリストから、ドキュメントを含む行の上にポインタを合わせて、「**概要の印刷**」をクリックします。

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   または

   プルーフビューアでプルーフを表示している間に、左側のツールバーの **印刷** アイコン ![ 印刷アイコン ](assets/print-icon-in-pv.png) をクリックします。 （左側のツールバーが表示されていない場合は、プルーフビューアの左上隅にあるメニューアイコン ![ メニューアイコン ](assets/menu-icon-in-pv.png) をクリックします。）

1. 次のいずれかのオプションを使用します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">表示</td> 
      <td> <p>印刷する内容を指定します。</p> 
       <ul> 
        <li>プルーフの<strong>現在のバージョン</strong>または<strong>全バージョン</strong></li> 
        <li><strong>コメント付きのページ</strong>のみまたは<strong>全ページ</strong></li> 
        <li><strong>ページサムネール</strong>（各ページの小さなレンダリング）のみまたは<strong>全ページ</strong>（プルーフの完全なレンダリング）<br></li> 
        <p>メモ：印刷出力のマークアップにピン番号を表示するには、ページサムネールではなく全ページを選択する必要があります。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コメントの並べ替え基準</td> 
      <td> <p>（上記でページサムネイルを選択した場合にのみ利用可能）プルーフのコメントを印刷する順序を指定します。</p> 
       <ul> 
        <li><strong>最も古い</strong>：最初のコメントから最後のコメントまで</li> 
        <li><strong>最新</strong>：最後のコメントから最初のコメントまで</li> 
        <li><strong>ページ</strong>：ページ別、最初のページから最後のページまで、または最後のページから最初のページまで</li> 
        <li><strong>作成者</strong>：追加したユーザーの名前順（A から Z または Z から A）</li> 
       </ul> <p>これらのオプションは、XLS ファイルまたは PDF ファイルとして書き出す場合の出力には影響しません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コメントの絞り込み</td> 
      <td> <p>これらのオプションを任意に組み合わせて使用すると、印刷または XLS ファイルや PDF ファイルとして書き出す場合の出力に特定のコメントのみを含めることができます。</p> 
       <ul> 
        <li>選択した入力者（デフォルト）</li> 
        <li>選択したアクション</li> 
        <li><strong>未解決</strong>のステータス</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ワークフロー</td> 
      <td> <p>（プルーフに自動化ワークフローが設定されている場合にのみ使用可能）「<strong>ダイアグラムを表示</strong>」をクリックすると、プルーフのステージと各ステージで下された決定を示すダイアグラムを印刷出力に含めることができます。表示されるダイアグラムにおいて、各ステージで下された決定は色で表されます。</p> <p><strong>緑</strong>：承認済み</p> <p><strong>青</strong>：決定を保留中</p> <p><strong>赤</strong>：決定には変更が必要</p> <p><strong>灰色</strong>：未開始</p> <p><strong>黄</strong>：変更して承認済み</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**印刷**」をクリックします。
1. 概要を印刷する場合は、表示されるウィンドウの右パネルで、**宛先**&#x200B;メニューをクリックし、次に「**結果をもっと表示**」をクリックします。表示されるリストで、使用するプリンターをクリックし、「**印刷**」をクリックします。

   または

   概要を PDF ファイルとして保存する場合は、**宛先**&#x200B;メニューをクリックし、「**PDF として保存**」、「**保存**」の順にクリックします

## XLS または PDF 形式でのプルーフ概要の書き出し

静的コンテンツのプルーフ概要を XLS ファイルまたは PDF ファイルとしてエクスポートできます。プルーフの書き出しには、プルーフの内容のみが含まれます。

1. プルーフを含むドキュメントリストから、ドキュメントを含んだ行にポインタを合わせて、「**概要の印刷**」をクリックします。

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. ページの右上隅付近にある「XLS」アイコンまたは「PDF」アイコンをクリックします。

   ![XLS PDF アイコン ](assets/xls-pdf-icons-350x136.png)

書き出したファイルの準備が整うと、ファイルのダウンロード方法を示すメールが届きます。

概要を PDF ファイルとして書き出した場合、プルーフに関するコメントが PDF リーダーに表示されます。コメントに複数のマークアップが関連付けられている場合、コメントはコメントリストに複数回表示されます（マークアップごとに 1 回）。
