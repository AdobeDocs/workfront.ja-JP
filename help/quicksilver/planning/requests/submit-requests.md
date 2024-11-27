---
title: Adobe Workfront計画リクエストの発行
description: Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: d7c7b09b033705142b2c658c9d275e63299d3fd0
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 13%

---


# レコードを作成するためのAdobe Workfront Planning 要求の発行

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。

Workfront ユーザーと外部ユーザーは、Planning レコードタイプに対してリクエストを送信し、レコードを作成できます。<!--double check on the external users-->

この記事では、新しいレコードをレコードタイプに追加するリクエストを送信する方法について説明します。

ワークスペースマネージャーがリクエストフォームを作成し、レコードタイプに関連付ける方法について詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td>
   <td>
<p>任意 </p>  
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </td>
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

   * Workfront アカウントをお持ちの場合、リンクは社内ユーザーとのみ共有されており、ワークスペースに対する投稿以上のアクセス権を持っています。 Workfront外のユーザーは、社内で共有されているリンクにアクセスできません。
   * Workfront アカウントがない場合、リンクは外部のユーザーと共有されています。 また、Workfront ユーザーは、外部のユーザーと共有されているリンクにアクセスすることもできます。

* フォームへのリンクは期限切れにできません。

## Workfront Planning への要求の送信に関する考慮事項

* Workfront Planning 要求の要求フォームには、フォームへのリンクからのみアクセスできます。
* リクエストをWorkfront Planning に送信した後に編集することはできません。
* 送信された各リクエストは、使用するフォームに関連付けられたレコードタイプのレコードを作成 <!--<span class="preview">if the form is not associated with an approval, or if the approval has been granted.</span> --> ます
* リクエストフォームを送信して作成されたレコードを、他の方法で追加されたレコードと区別することはできません。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* <span class="preview"> 送信されたリクエストは、Workfront </span> の「リクエスト」領域にある「送信済み」セクションの「計画」タブに表示されます。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some incosistency between unified-approvals-service and intake-approvals-flow.-->


## Workfront Planning への要求の発行

1. Workfront Planning レコードタイプから共有されたリンクに移動します。

1. フォームで使用可能なフィールドを更新します。 アスタリスクの付いたフィールドは必須です。

   >[!TIP]
   >
   >   **件名** フィールドが使用可能な場合、リクエストの送信後に、Workfront Planning に表示されません。
   >
   >新しいレコードがWorkfront Planning のレコードタイプに追加された際に識別可能になるように、リクエストのできるだけ多くのフィールドを更新することをお勧めします。

1. 「**送信**」をクリックします。

   フォームが送信され、次の処理が行われます。

   * <!--If the request form was not associated with an approval, or <span class="preview">if the approval was granted</span>, a-->新しいレコードが、フォームに関連付けられたレコードタイプに追加されます。


   * <!--If the request form was not associated with an approval, the--> <span class="preview"> リクエストが「Workfront リクエスト」領域の「送信済み」セクションに追加され、新しいレコードがレコードタイプページに追加されます。</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview"> 少なくとも 1 つのワークスペースへのアクセス権を持つすべてのユーザーは、リクエスト エリアの「計画」タブを表示できます。 表示できるのは、自分が送信した要求のみです。 Workfront管理者は、システム内のすべてのリクエストを表示できます。</span> <!--ensure this is correct; asking team in slack-->

   <!--
   * <span class="preview">If the request form was associated with an approval, the request is temporarily saved to the Planning tab in the Submitted section of the Workfront Requests area. No record is created for the record type associated with the request form.</span>

      <span class="preview">For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>  
   -->
   <!--

   * <span class="preview">You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.</span> 
   * <span class="preview">If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.</span> 
   -->



