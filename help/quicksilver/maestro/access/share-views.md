---
title: ビューの共有
description: 他のユーザーとビューを共有して、Adobe Workfront Maestro で作業する際のコラボレーションを確保できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 1%

---


<!--*****************ADD TO TOC AND MINITOC WHEN RELEASING*********************-->

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# ビューの共有

他のユーザーとビューを共有して、Adobe Workfront Maestro で作業する際のコラボレーションを確保できます。

ワークスペースに権限を付与しても、レコードタイプページのビューに対する他のユーザーの権限は付与されません。 他のユーザーと共有するには、レコードタイプのページ内の個々のビューに権限を付与する必要があります。

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
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> AdobeMaestro のアクセス制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>オブジェクトの権限</p></td>
   <td> <p>ビューに対する権限の管理</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 </p>  
</td>
  </tr>
 </tbody>
</table>

## ビューに対する権限の共有

管理権限を持つ作成または表示を共有できます。

>[!NOTE]
>
>システム管理者は、自分で作成しなかったビューを表示または共有できません。 ユーザーは、自分と共有されているビューの表示や共有のみを行うことができます。


他のユーザーとビューを共有するには：

{{step1-to-maestro}}

1. 表示を共有するワークスペースを開き、「レコードタイプ」カードをクリックします。

   レコードタイプのページが開きます。

1. 「表示」ドロップダウンメニューで、共有する表示の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) ビュー名の右に移動し、 **共有**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Adobe Analytics の **にビューアクセスを許可** フィールドにユーザーまたはグループの名前を入力し、リストに表示されたらクリックします。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、 [AdobeMaestro での共有権限の概要](../access/sharing-permissions-overview.md).
1. 「**保存**」をクリックします。


## ビューに対する権限の削除


{{step1-to-maestro}}

1. 表示を共有するワークスペースを開き、「レコードタイプ」カードをクリックします。

   レコードタイプのページが開きます。

1. 「表示」ドロップダウンメニューで、共有する表示の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) ビュー名の右に移動し、 **共有**.

1. 削除するユーザーまたはグループを見つけ、「 **削除** （ユーザーまたはグループの名前の右側にある権限ドロップダウンメニュー）

1. 「**保存**」をクリックします。

   削除されたユーザーまたはグループに属するユーザーは、ビューにアクセスできなくなります。