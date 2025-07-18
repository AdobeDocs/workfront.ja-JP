---
title: 重複レコード
description: テーブル表示で既存のレコードを複製できます。 既存のレコードの同一のコピーがレコードタイプページに追加されます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 27%

---

# 重複レコード

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

テーブル表示で既存のレコードを複製できます。 既存のレコードの同一のコピーがレコードタイプページに追加されます。

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
   <td>   <p>ワークスペースおよびレコードタイプに対する投稿以上の権限 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## レコードの複製 <!--in a record type table (I don't think you can create them elsewhere right now)-->

既存のレコードを複製することで、レコードタイプページのテーブル表示でレコードを作成できます。 既存のレコードと同一のレコードが作成され、元のレコードの下に追加されます。


{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがビューに表示されます。

1. （条件付き）テーブル表示を選択します。

1. 次のいずれかの操作を行います。

   * レコード名にポインタを合わせ、レコード名とインラインで **詳細** メニューをクリックしてから、**複製** アイコン ![ 複製アイコングレー ](assets/duplicate-icon-gray.png) をクリックします。

     ![ テーブル表示のレコードからの「詳細」メニュー ](assets/more-menu-from-record-in-table-view.png)

   * レコードを選択し、ページ下部のツールバーにある **複製** アイコン ![ 白と青の複製アイコン ](assets/duplicate-icon-white-and-blue.png) をクリックします。

     ![ テーブル表示のツールバーの複製アイコン ](assets/duplicate-icon-in-toolbar-in-table-view.png)

   元のレコードの下に、同じ名前の同じレコードが作成されます。 新しいレコードのすべてのフィールドには、元のレコードと同じ情報が入力されます。

1. （オプション）「テーブル」ビューで使用可能なフィールド内の新しいレコードに関する情報の更新を開始するか、レコードをクリックしてレコードのプレビューまたはページ内の情報を更新します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクするときにレコードを識別すると便利なので、レコードの主フィールドの情報を追加することをお勧めします。 主フィールドについて詳しくは、[ テーブル表示の管理 ](/help/quicksilver/planning/views/manage-the-table-view.md) および [プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

   レコードの編集の詳細については、「[ レコードの編集 ](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

1. （オプション）テーブル表示で新しいレコードやその情報を追加する際に、それらの追加の取り消しまたはやり直しを行うには、次のキーボードショートカットを使用します。

   * CTRL + Z （Macの場合は ⌘ + Z）
   * CTRL + Shift + Z （Macの場合は ⌘ + Shift + Z）。変更をやり直すことができます。
