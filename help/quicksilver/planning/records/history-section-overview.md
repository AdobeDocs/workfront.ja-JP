---
title: 履歴セクションの概要
description: Adobe Workfront Planning のレコードの右パネルで、レコードに対して行われ、システムによって記録された変更を確認できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 71%

---

# 履歴セクションの概要

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードに関する共同作業を行うことができます。また、レコードに加えられた他の変更やシステムにより記録された他の変更を、このエリアに表示することもできます。

レコードの右側のパネルには、次のセクションが表示されます。

* **コメント**：ユーザーがレコードに追加したコメントおよび返信を表示します。Workfront Planning レコードでのコメントの管理について詳しくは、[レコードのコメントの管理](/help/quicksilver/planning/records/manage-record-comments.md)を参照してください。
* **履歴**：ユーザーがレコードのフィールドに対して行い、システムで記録された変更を表示します。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
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
   <td> <p>コントリビューター以上のライセンス</p>
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
   <td>   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> </a> に対する表示以上の権限 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> 
   <p>実稼動環境では、システム管理者を含むすべてのユーザーを、計画領域を含むレイアウトテンプレートに割り当てる必要があります。</p>
   <div class="preview">
<p> プレビュー環境では、ライトまたはコントリビューターライセンスを持つユーザーには、Planning を含むレイアウトテンプレートを割り当てる必要があります。</p>

<p>標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</p></div>

<p>詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">レイアウトテンプレートを作成および管理</a>を参照してください。</p>
    </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードの履歴セクションを見つける

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、カードにレコードタイプが表示されます。

1. レコードタイプのカードをクリックします。
レコードタイプのページが開き、そのタイプのすべてのレコードが表示されます。

1. 任意のビューで、レコードの名前をクリックします。

   レコードのページが開きます。コメントエリアがデフォルトで右パネルに開きます。
1. **履歴を表示** アイコン ![ 履歴を表示アイコン ](assets/show-history-icon.png) をクリックします。 レコードのフィールドに加えられたすべての変更が、最新の変更を先頭にして右パネルに表示されます。
1. （オプション） **履歴を非表示** アイコン ![ 履歴を非表示アイコン ](assets/hide-history-icon.png) をクリックして、右側のパネルを閉じます。

## 履歴セクションに関する考慮事項

レコードのフィールドに加えた変更は、レコードのページの右パネルにある「履歴」セクションで確認できます。

![ コメントの履歴領域 ](assets/history-area-in-comments.png)

* Workfront Planning は、次の情報を「履歴」セクションに記録します。

   * フィールドの変更

   * 値が変更されたときの、フィールドの古い値と新しい値。古い値は、打ち消し線付きで表示されます。

   * 変更を加えたユーザーのフルネーム

   * 変更が発生した日時スタンプ

* 次のタイプのフィールドでは、常に古いの値（打ち消し線付きの形式）と新しい値が表示されます。

   * テキスト
   * 段落
   * 通貨
   * 日付
   * 数値
   * パーセンテージ
   * 単一選択

* 次のタイプのフィールドは、複数の値のうち少なくとも 1 つが削除された場合にのみ、打ち消し線付きの形式で古い値を表示します。

   * 複数選択
   * リンクされたレコードフィールド
   * ユーザー

  変更によってフィールドに値が追加されただけの場合、古い値は表示されず、新しいフィールド値のみが表示されます。

* チェックボックスタイプのフィールドでは、以前の値が打ち消し線付きの形式で表示されることはありません。フィールドが編集された場合は、変更が行われた時点の状態のみが表示されます。

  Workfront Planning フィールドについて詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

* 次のタイプのフィールドに対する変更は、「履歴」セクションに表示されません。

   * リンクされた（ルックアップ）フィールド
   * 式
   * 作成者
   * 作成日
   * 最終変更者
   * 最終変更日

* フィールドがシステムから削除されても、そのフィールドに対して行われた更新は「履歴」セクションに残ります。レコードの「履歴」セクションでフィールドが削除されたことを示すものはありません。
