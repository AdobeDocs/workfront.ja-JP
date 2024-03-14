---
title: ビューの共有
description: 他のユーザーとビューを共有して、Adobe Workfrontの計画機能を使用する際のコラボレーションを確実におこなうことができます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 7%

---


<!--update the metadata and description when we turn this article live-->

# ビューの共有

{{maestro-important-intro}}

他のユーザーとビューを共有して、Adobe Workfrontの計画機能でレコードを操作する際のコラボレーションを確保できます。

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
<p>組織は、Adobe Workfront Planning 機能クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> Adobe Workfront Planning 機能に対するアクセス制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td> <p>ビューに対する権限を管理</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontの管理者を含むすべてのユーザーには、メインメニューの Maestro 領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、 <a href="/help/quicksilver/maestro/access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## ビューに対する権限の共有

管理権限を持つ作成または表示を共有できます。

>[!NOTE]
>
>システム管理者は、自分で作成しなかったビューを表示または共有できません。 ユーザーは、自分と共有されているビューに対してのみアクセスまたは共有できます。
>
>システム管理者は、1 つのビューに対する管理権限のみを持つことができます。

{{step1-to-maestro}}

1. 表示を共有するワークスペースを開き、レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 「表示」タブで、共有する表示の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) ビュー名の右に移動し、 **共有**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Adobe Analytics の **にビューアクセスを許可** フィールドにユーザーまたはグループの名前を入力し、リストに表示されたらクリックします。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、 [Adobe Workfrontの計画機能での共有権限の概要](../access/sharing-permissions-overview.md).

     <!--System administrators always receive Manage permissions to views shared with them.-->

1. クリック **リンクをコピー** をクリックして、ビューへのリンクをクリップボードにコピーします。
1. コピーしたリンクを他のユーザーと共有します。 レコードタイプのページにアクセスして選択したビューに表示するには、リンクを受け取ったユーザーがアクティブユーザーであり、Workfrontにログインしている必要があります。
1. 「**保存**」をクリックします。

## ビューに対する権限の削除

{{step1-to-maestro}}

1. 表示を共有するワークスペースを開き、レコードタイプのカードをクリックします。 レコードタイプのページが開きます。
1. 「表示」ドロップダウンメニューで、共有する表示の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) ビュー名の右に移動し、 **共有**.
1. 削除するユーザーまたはグループを見つけ、「 **削除** （ユーザーまたはグループの名前の右側にある権限ドロップダウンメニュー）
1. クリック **保存**.
削除されたユーザーまたはグループに属するユーザーは、ビューにアクセスできなくなります。 ビューへのアクセスから削除されたユーザーには通知はありません。
