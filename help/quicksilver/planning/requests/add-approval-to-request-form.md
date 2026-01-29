---
title: Adobe Workfront Planning の要求フォームへの承認の追加
description: Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '1192'
ht-degree: 5%

---

# Adobe Workfront Planning でリクエストフォームに承認を追加する

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。

この記事では、ワークスペースマネージャーがレコードタイプに関連付けられたリクエストフォームに承認を追加する方法について説明します。

Adobe Workfront Planning でのリクエストフォームの作成について詳しくは、[Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

レコードを作成するレコード・タイプにリクエストを発行する方法は、「レコードを作成するためのAdobe Workfront Planning リクエストの発行 [&#x200B; を参照してください &#x200B;](/help/quicksilver/planning/requests/submit-requests.md)。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfront パッケージと任意の Planning パッケージ</p>
または
<p>任意のワークフローパッケージと任意の Planning パッケージ</p>

<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限とレコードタイプの管理 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## リクエストフォームへの承認の追加に関する考慮事項

* リクエストフォームには、1 人または複数の承認者を追加できます。 承認者として追加できるのはユーザーのみです。
* リクエストフォームを送信して作成したレコードの承認情報を、「承認者」および「承認日」フィールドに表示できます。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。
* リクエストフォームに複数の承認者を追加する場合、Workfront Planning でレコードを作成する前に、すべての承認者がリクエストを承認する必要があります。
* すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプに対してレコードが作成されます。
* 少なくとも 1 人の承認者がリクエストを拒否し、他の全員がそのリクエストを承認した場合、Workfrontの「リクエスト」領域に対してリクエストが作成されますが、リクエストフォームに関連付けられたレコードタイプに対しては、レコードが作成されません。
* リクエストフォームへの承認の追加はオプションです。 リクエストフォームが承認と関連付けられていない場合、リクエストの送信時にWorkfront Planning によって即座にレコードが作成されます。

## 実稼動環境でのリクエストフォームへの承認の追加

1. [Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. **設定** をクリックします。

   **設定** 領域が表示されます。

   ![&#x200B; 「設定」タブ &#x200B;](assets/configuration-tab.png)
1. **承認者** フィールドに、承認者として設定するユーザーまたはチームの名前の入力を開始し、リストに表示されたら選択します。
1. （オプションおよび条件付き）複数の承認者を設定し、決定を行う承認者が 1 人だけの場合は、「**1 つの決定のみが必要**」オプションを有効にします。

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* リクエストフォームには、1 人または複数の承認者を追加できます。
   >
   >* 複数の承認者を追加し、「1 人の承認が必要」オプションが有効になっていない場合、Workfront Planning でレコードが作成される前に、すべての承認者がリクエストを承認する必要があります。
   >
   >* 少なくとも 1 人の承認者が要求を拒否した場合、要求は拒否され、レコードは作成されません。 リクエストは、Workfrontのリクエスト エリアに残ります。
   >
   >* 複数の承認者を追加し、「必要な決定が 1 つのみ」オプションが有効になっていない場合、リクエストが承認または却下される前に、すべての承認者が決定を行う必要があります。
   >
   >* チームが承認者として設定されている場合、チームからの決定は 1 つだけ必要です。


1. （任意）リクエストフォームを共有したことがない場合は、「**公開**」をクリックします。

   または

   「**共有**」をクリックしてフォームを共有し、「**リンクをコピー**」をクリックします。
1. （任意）ユーザーが共有リンクを使用してリクエストを送信すると、Workfront Planning からアプリ内承認通知とメールが承認者に送信されます。

   >[!NOTE]
   >
   >   組織のWorkfront インスタンスは、ユーザーがメールおよびアプリ内通知を受信できるように、Adobe統合エクスペリエンスにオンボーディングされている必要があります。


   リクエストの承認について詳しくは、[&#x200B; リクエストの承認 &#x200B;](/help/quicksilver/planning/requests/approve-request.md) を参照してください。

<div class="preview">

## リクエストフォームに承認ルールを追加する

>[!NOTE]
>
>この機能は、プレビュー環境でのみ使用できます。

承認ルールは、送信されたリクエストのフィールド値に基づいて承認プロセスを定義します。

例えば、リクエストフォームに「キャンペーンタイプ」フィールドがある場合、フィールドの値が「デジタル」の場合は 1 人のユーザーにリクエストを送信し、値が「印刷」の場合は別のユーザーにリクエストを送信するルールを作成できます。

承認ルールを追加する際は、次の点を考慮してください。

* 承認ルールには、1 人または複数の承認者を追加できます。
* 少なくとも 1 人の承認者が要求を拒否した場合、要求は拒否され、レコードは作成されません。 リクエストは、Workfrontのリクエスト エリアに残ります。
* 複数の承認者を追加し、「必要な決定が 1 つのみ」オプションが有効になっていない場合、リクエストが承認または却下される前に、すべての承認者が決定を行う必要があります。
* チームが承認者として設定されている場合、チームの 1 人のメンバーに対して必要な決定は 1 つだけです。

リクエストフォームの承認ルールを設定するには：

1. [Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. 「**設定**」をクリックします。

   「設定」タブが表示されます。

1. 承認ルールの設定を開始するには、左側のパネルで **承認** ![&#x200B; 承認アイコン &#x200B;](assets/approvals-icon-on-form.png) をクリックします。

1. （オプション）デフォルトの承認プロセスを設定する場合は、「**デフォルトの承認ルール**」領域の「**承認者**」フィールドに少なくとも 1 人のユーザーまたはチームを追加し、デフォルト承認者のいずれかが承認した後にレコードを作成するには、「**決定は 1 つだけ必要**」チェックボックスをクリックします。

   ![&#x200B; デフォルトの承認ルール領域 &#x200B;](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. （任意）承認ルールの追加を開始します。 承認ルールごとに、次の操作を行います。

   1. 「**承認ルールを追加**」をクリックします
   1. プレースホルダータイトル **名称未設定の承認ルール** をクリックし、承認ルールの名前を入力します。
   1. **フィールドを選択** をクリックし、ルールをアクティブにするフィールドを選択します。
   1. ルールの演算子を選択します。 演算子は、フィールドのタイプによって異なります。
   1. 選択した演算子に値が必要な場合は、プラスアイコンをクリックして 1 つ以上の値を追加します。
   1. （任意）「**条件を追加**」をクリックして条件を追加し、手順 C～E のように追加の条件を設定して **And** または **Or** ステートメントで接続します。
   1. 承認ルールの **アクション** 領域にある **承認者** フィールドに、条件が満たされたときに承認者に設定するユーザーまたはチームを少なくとも 1 つ追加します。
   1. （条件付き）承認者の 1 人が承認した後にレコードを作成する場合は、「**決定は 1 つだけ必要**」チェックボックスをオンにします。

1. 「**保存**」をクリックして、承認ルールを保存します。
1. （任意）リクエストフォームを共有したことがない場合は、「**公開**」をクリックします。

</div>
