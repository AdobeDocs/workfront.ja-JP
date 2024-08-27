---
title: Adobe Workfront計画リクエストの発行
description: Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 18183b53c783366f467e7330159923372b51deb6
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 10%

---

# レコードを作成するためのAdobe Workfront Planning 要求の発行

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。

Workfront ユーザーと外部ユーザーは、Planning レコードタイプに対してリクエストを送信し、レコードを作成できます。<!--double check on the external users-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

Workfront Planning にアクセスするには、次のものが必要です：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfrontの計画<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
<p>次のいずれかのWorkfront プラン：</p>
<ul><li>選択</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront計画*</p></td>
   <td>
<p>任意 </p>  
<p>各Workfront Planning プランに含まれる内容の詳細については、<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfrontの価格とパッケージ </a> を参照してください。 </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>外部、コントリビューター、ライト、または標準のライセンス</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>Workfront ユーザーの場合は、ワークスペースに対する以上の権限を表示します。</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontのプランニング エリアにアクセスするには、メインメニューのプランニング エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>
   <p> ただし、Workfront Planning にリクエストを送信するために Planning エリアにアクセスする必要はありません。 </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

Workfront Planning 要求フォームに要求を送信するには、次の手順を実行する必要があります。

* Workfront Planning には、次のものが存在する必要があります。

   * ワークスペース
   * リクエストフォームに関連付けられたレコードタイプ。 詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

* リクエストフォームは、アクセスできる方法でリンクと共有する必要があります。 次のシナリオが存在します。

   * Workfront アカウントをお持ちの場合、リンクは社内ユーザーとのみ共有され、自身も Workspace にアクセスできます。 Workfront外のユーザーは、社内で共有されているリンクにアクセスできません。
   * Workfront アカウントがない場合、リンクは外部のユーザーと共有されています。 Workfrontのユーザーは、外部のユーザーと共有されているリンクを使用することもできます。

* フォームへのリンクは期限切れにできません。

## Workfront Planning への要求の送信に関する考慮事項

* フォームへのリンクがないと、Workfront Planning 要求の要求フォームにアクセスできません。
* リクエストをWorkfront Planning に送信した後に編集することはできません。
* 送信された各リクエストは、使用するフォームに関連付けられたレコードタイプのレコードを作成します。
* リクエストフォームを送信して作成されたレコードを、他の方法で追加されたレコードと区別することはできません。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

## Workfront Planning への要求の発行

1. Workfront Planning レコードタイプから共有されたリンクに移動します。

1. フォームで使用可能なフィールドを更新します。 アスタリスクの付いたフィールドは必須です。

   >[!TIP]
   >
   >   Workfrontの **件名** フィールドが使用可能な場合、Workfront Planning に表示されないことがあります。 新しいレコードがレコードタイプに追加された際に識別できるように、リクエスト内の可能な限り多くのフィールドを更新することをお勧めします。

1. 「**送信**」をクリックします。

   フォームが送信され、新しいレコードがフォームに関連付けられたレコードタイプに追加されます。





