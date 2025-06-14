---
title: 削除されたレコードを復元
description: Adobe Workfront Planning の「最近削除されたレコード」領域から削除されたレコードを復元できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 19%

---

# 削除されたレコードを復元

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning の「最近削除されたレコード」領域から削除されたレコードを復元できます。

レコードの削除について詳しくは、[ レコードの削除 ](/help/quicksilver/planning/records/delete-records.md) を参照してください。

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
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
   <td>   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> に対する投稿以上の権限 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p></td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 削除されたレコードの復元に関する考慮事項

* レコードは、最近削除された bin に 30 日間保存されます。 30 日後、レコードはWorkfront Planning から完全に削除されます。
* 削除されたレコードが他のレコードにリンクされている場合、リンクされているレコードは削除されませんが、削除されたレコードの情報も削除されます。 削除したレコードを復元すると、接続されたレコードから情報が復元されます。
* レコードを一括で復元できます。
* レコードを削除すると、次の情報が最近削除された bin に格納されます。
   * **名前**：これは、レコードのプライマリフィールド内の情報です。 レコードプライマリフィールドについて詳しくは、[プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   * **削除日**：レコードが削除された日時。
   * **最近削除された時間**: レコードが削除されてからの時間。 現在の日付より 30 日以上前に削除されたレコードは、「最近削除された項目」ビンに表示されません。
   * **削除者**: レコードを削除したユーザーの名前。

## 削除されたレコードを復元

1. レコードを削除したレコードタイプ ページに移動します。
1. 任意のレコードタイプのページビューの右上隅にある **取り消し** アイコン ![ 取り消しアイコン ](assets/undo-icon.png) をクリックしてから、**最近削除された項目** をクリックします。

   **最近削除された項目** ボックスが表示されます。

   ![ 最近削除されたボックス ](assets/recently-deleted-box.png)

1. 削除するレコードを選択し、**復元**/**復元** をクリックします。 複数のレコードを選択できます。

   復元が成功すると、画面の下部に成功通知が表示されます。
1. テーブル表示に移動し、復元されたレコードを確認します。
