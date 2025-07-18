---
title: Adobe Workfrontからのフィールドのインポート
description: Adobe Workfront Planning では、レコードタイプの種類ごとにカスタムフィールドを作成できます。そしてフィールドを Workfront Planning レコードに関連付けることができます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 24%

---

<!--add to TOC-->

# Adobe Workfrontからのフィールドのインポート

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->


{{planning-important-intro}}

既存のWorkfront フィールドのコピーを読み込むことができます。 Workfrontからフィールドを読み込むと、Workfront Planning レコードタイプの各フィールドのコピーが作成されます。


## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <td><p> 標準 </p>
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
   <td>   <p>ワークスペースに対する権限とレコードタイプの </a> の管理 </p>  
   <p>システム管理者は、自分が作成したものでないものも含めて、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## Workfrontからのフィールドの読み込みに関する考慮事項

* Workfront Planning のレコードタイプに、ネイティブまたはカスタムのWorkfront フィールドを読み込むことができます。
* Workfront フィールドを読み込むと、同じフィールドのコピーが作成され、Workfront Planning のフィールド名が保持されます。 Workfront Planning にコピーされた後、これらのフィールドは元のWorkfrontフィールドから独立しており、情報を共有しません。
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* 次のWorkfront オブジェクトからネイティブフィールドまたはカスタムフィールドを追加できます。
   * ポートフォリオ
   * プログラム
   * プロジェクト
   * タスク
   * イシュー
   * ドキュメント
   * 会社
   * グループ
   * ユーザー
   * 担当業務
   * 割り当て
   * 時間
   * 請求記録
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * 費用
   * イテレーション
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Workfront フィールドは、Workfront Planning にインポートされた後、フィールドタイプが保持されない場合があります。

  次の表に、Workfrontのフィールドタイプと、対応するWorkfront Planning のフィールドタイプを示します。

  | Workfrontのフィールドタイプ | Workfront計画フィールドタイプ |
  |------------------------------------------|-------------------------------|
  | テキスト形式の 1 行テキスト | 1 行テキスト |
  | 数値の書式設定された 1 行テキスト | 数値 |
  | 通貨書式の 1 行のテキスト | 通貨 |
  | 段落 | 段落 |
  | 書式付きテキスト | 段落 |
  | 単一選択ドロップダウン | 単一選択 |
  | 複数選択ドロップダウン | 複数選択 |
  | ユーザー先行入力フィルターはサポートされていません | ユーザー |
  | 計算済み* | 式 |
  | 日付 | 日付 |
  | チェックボックスグループ | 複数選択 |
  | ラジオボタン | 複数選択 |

  *計算フィールドは後日使用できるようになります。
それ以外のWorkfront フィールドタイプは、Workfront Planning ではすべてサポートされていません。


## Workfront からのフィールドを読み込み

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. フィールドを作成するレコードタイプのワークスペースをクリックします。

   ワークスペースが開き、レコードタイプが表示されます。

1. レコードタイプのカードをクリックします。

   そのレコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。

   >[!TIP]
   >
   >    一部のフィールドが非表示になっている可能性があります。 「**フィールド**」をクリックし、テーブルビューに列として表示するフィールドの切り替えを有効にします。

1. テーブルビューの右上隅にある「**+**」アイコンをクリックします

   または

   任意の列のヘッダーにポインタを合わせ、フィールド名の後の下向き矢印をクリックしてから、「**左に挿入** または **右に挿入** をクリックして新しいフィールドを追加します。
1. **新規フィールド** タブの右下隅にある「**既存を追加** をクリックします。<!--check UI - did they change this??-->

   ![Workfrontから既存のフィールドを追加モーダル ](assets/add-existing-fields-from-workfront-modal.png)

1. 検索領域に既存のWorkfront フィールドの名前の入力を開始し、リストに表示されたら **+** をクリックします。
1. （オプション）別のフィールドを入力し、リストに表示されたら **+** をクリックします。
1. （任意） **フィルター** アイコン ![ インポートフィールドのフィルター ](assets/filters-in-import-fields-icon.png) アイコンをクリックして、次のフィールドの一方または両方を更新します。

   * オブジェクトタイプ：フィールドを読み込むWorkfront オブジェクトタイプを選択します。
   * カスタムフォーム：Workfrontから 1 つまたは複数のカスタムフォームを選択します。 最初にオブジェクトタイプを選択しなくても、カスタムフォームを選択できます。
1. 「**+**」をクリックし、「**フィールドを追加** をクリックします。
フィールドがテーブル ビューおよびレコードの詳細ページに追加されます。

   >[!IMPORTANT]
   >
   >    レコードタイプのフィールドは 500 個までです。 既存のフィールドと読み込まれたフィールドがこの制限に貢献します。

   追加されたフィールドはWorkfront フィールドのコピーであり、Workfrontの元のフィールドには接続されなくなります。
