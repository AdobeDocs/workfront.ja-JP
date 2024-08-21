---
title: Adobe Workfront Planning でのリクエストフォームの作成
description: Adobe Workfrontの計画エリアでレコードタイプを選択した後、そのレコードタイプに関連付けられたリクエストフォームを作成し、そのレコードタイプへのリンクを他の内部ユーザーまたは外部ユーザーと共有できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 21%

---

# Adobe Workfront Planning でのリクエストフォームの作成

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Adobe Workfrontの計画エリアでレコードタイプを選択したら、リクエストフォームを作成して、そのレコードタイプに関連付けることができます。 その後、リンクを他の社内ユーザーや外部ユーザーと共有できます。<!--double-check on the external part of it-->

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
<p>任意 </p>   </td>

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
   <p>標準</p>
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
   <ul>
   <li><p>ワークスペースに対する権限の管理</p></li>
    <li><p>システム管理者は、自分が作成していないワークスペースを管理できます。 </p></li>
    </ul>
   <p>Workfront Planning オブジェクトの共有権限について詳しくは、
<a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a>を参照してください。 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードタイプ用のリクエストフォームの作成

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側 ![](assets/more-menu.png) ある **詳細** メニューをクリックし、「**リクエストフォームを作成**」をクリックします。
1. リクエストフォームの名前を更新します。 デフォルトでは、フォームの名前は **名称未設定のリクエストフォーム** です。<!--check this; you logged a bug to rename it to this but was it fixed?-->
1. （オプション）リクエストフォームに **説明** を追加します。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 「**作成**」をクリックします。選択したレコードタイプのリクエストフォームが開きます。

   リクエストフォームには、デフォルトで次の情報が含まれています。

   * **デフォルトセクション**：これは、Workfrontがリクエストフォームに適用するデフォルトのセクション区切りです。 既定のセクションの名前を変更したり、削除することはできません。
   * **件名** フィールド：Workfrontでリクエストを識別するフィールド。 この機能は、まだ利用できません。
   * レコードタイプに関連付けられているすべてのフィールド。

   リクエストフォームに含まれるフィールドは、このレコードタイプにリクエストを送信するすべてのユーザーに表示されます。

1. （任意）「**件名**」フィールドはWorkfront Planning には表示されないので、削除します。<!--remove this step when we connect intake with the Requests area in Workfront-->
1. 削除するフォーム上のフィールドの上にポインタを合わせます。 これらは、フォームの左側にある **フィールド** タブに追加されます。
1. 任意のフィールドをクリックし、フォームの右側のコントロールを使用して、フィールドに関する次の情報を定義します。

   * **ラベル**：リクエストフォームに表示されるフィールドの名前です。 レコードフィールドの名前は変更されません。
   * **手順**：フィールドに関する詳細情報を追加します。
   * **必須フィールドにする**：選択する場合、フィールドには値が必要です。 追加されていない場合、フォームを送信できません。
   * **ロジックの追加**：フィールドを表示または非表示にするには、どの条件を満たす必要があるかを定義します。

1. フォームの右側の「コンテンツ要素」タブをクリックし、次の要素のいずれかを追加します。

   * 説明テキスト
   * セクション区切り

   カスタムフォームの作成について詳しくは、「[ フォームデザイナーを使用したフォームのデザイン ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。





