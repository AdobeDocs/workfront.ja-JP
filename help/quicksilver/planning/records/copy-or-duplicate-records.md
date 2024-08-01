---
title: 重複レコード
description: テーブル表示で既存のレコードを複製できます。 既存のレコードの同一のコピーがレコードタイプページに追加されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 32%

---


# 重複レコード

<!--update the metadata after GA-->

{{planning-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

テーブル表示で既存のレコードを複製できます。 既存のレコードの同一のコピーがレコードタイプページに追加されます。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 契約</p></td>
   <td>
<p>Workfront Planning の早期アクセス段階に登録されている必要があります </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>新規：標準</p>
   <p>現在：プラン</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する参加以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*詳しくは、[Workfrontのアクセス要件ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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

   * レコード名にポインタを合わせ、レコード名とインラインで **詳細** メニューをクリックしてから、![](assets/duplicate-icon-gray.png) にある **複製** アイコンをクリックします。

     ![](assets/more-menu-from-record-in-table-view.png)

   * レコードを選択し、ツールバーのページ下部にある **複製** アイコン ![](assets/duplicate-icon-white-and-blue.png) をクリックします。

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   元のレコードの下に、同じ名前の同じレコードが作成されます。 新しいレコードのすべてのフィールドには、元のレコードと同じ情報が入力されます。

1. （オプション）「テーブル」ビューで使用可能なフィールド内の新しいレコードに関する情報の更新を開始するか、レコードをクリックしてレコードのプレビューまたはページ内の情報を更新します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクするときにレコードを識別すると便利なので、レコードの主フィールドの情報を追加することをお勧めします。 主フィールドについて詳しくは、[ テーブル表示の管理 ](/help/quicksilver/planning/views/manage-the-table-view.md) および [プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

   レコードの編集の詳細については、「[ レコードの編集 ](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

1. （オプション）テーブル表示で新しいレコードやその情報を追加する際に、それらの追加の取り消しまたはやり直しを行うには、次のキーボードショートカットを使用します。

   * Ctrl + Z（Mac の場合は ⌘ + z）で、変更を取り消します
   * CTRL + Shift + Z （Macの場合は⌘ + Shift + Z）。変更をやり直すことができます。