---
title: ワークスペースの共有
description: ワークスペースを他のユーザーと共有して、Adobe Workfront Planning で作業する際のコラボレーションを確保できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 8%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Planning as a product ??-->

# ワークスペースの共有

{{maestro-important-intro}}

ワークスペースを他のユーザーと共有して、Adobe Workfront Planning で作業する際のコラボレーションを確保できます。

>[!NOTE]
>
>ワークスペースに権限を付与しても、レコードタイプページのビューに対する他のユーザーの権限は付与されません。 他のユーザーと共有するには、レコードタイプのページ内の個々のビューに権限を付与する必要があります。 詳しくは、 [ビューの共有](/help/quicksilver/maestro/access/share-views.md).


## アクセス要件

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Adobe Workfront Planning クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>新規：標準</p>
   または
   <p>現在：プラン </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> Adobe Workfront Planning のアクセス制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューの「計画」領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、 <a href="/help/quicksilver/maestro/access/access-overview.md">アクセスの概要</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

## ワークスペースに対する権限の共有

以下のユーザーは、ワークスペースを他のユーザーと共有できます。

* システム管理者は、作成しなかったワークスペースを含め、すべてのワークスペースを共有できます。
* 他のすべてのユーザーは、管理権限を持つワークスペースのみを共有できます。

ワークスペースを他のユーザーと共有するには：

{{step1-to-maestro}}

1. 共有するワークスペースを開き、「 **共有** をクリックします。

   ![](assets/share-button-on-workspace-top-right.png)

1. Adobe Analytics の **ワークスペースへのアクセス権の付与** フィールドにユーザーまたはグループの名前を入力し、リストに表示されたらクリックします。

   ![](assets/sharing-ui-with-groups.png)

1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 参加
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、 [Adobe Workfront Planning での共有権限の概要](../access/sharing-permissions-overview.md).
1. クリック **リンクをコピー** をクリックして、ワークスペースへのリンクをクリップボードにコピーします。
1. コピーしたリンクを他のユーザーと共有します。 このワークスペースにアクセスするには、リンクを受け取ったユーザーがアクティブユーザーであり、Workfrontにログインする必要があります。
1. 「**保存**」をクリックします。


## ワークスペースに対する権限の削除


{{step1-to-maestro}}

1. 権限を削除するワークスペースを開き、「 **共有** をクリックします。
1. ユーザー名またはグループ名の右にあるドロップダウンメニューをクリックし、 **削除**.
1. 「**保存**」をクリックします。

   削除されたユーザーまたはグループに属するユーザーは、ワークスペースまたはそのオブジェクトにアクセスできなくなりました。