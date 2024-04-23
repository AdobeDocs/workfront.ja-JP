---
title: レコードタイプの編集
description: レコードタイプは、保存後に編集できます。 レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 32%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# レコードタイプの編集

{{maestro-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。 自分または他のユーザーが作成したレコードタイプの外観を編集できます。 Workfront Planning レコード・タイプの作成の詳細は、次を参照してください。 [レコードタイプの作成](../architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>Adobe Workfront Planning レコードタイプをExperience Manager Assetsに接続するには、Adobe Experience Manager Assets ライセンスが必要で、組織のWorkfront インスタンスがAdobeの Business Platform またはAdobe Admin Consoleにオンボーディングされている必要があります。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning クローズドベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Workfront Planning には、アクセス レベルの制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限を管理</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## レコードタイプの編集

{{step1-to-maestro}}

最後にアクセスしたワークスペースが、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードの種類を編集するワークスペースを選択します。
1. レコードタイプのカードにポインタを合わせて、 **詳細** メニュー ![](assets/more-menu.png) レコードタイプカードの右上隅のをクリックします **編集**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. が含まれる **レコードタイプを編集** ボックスで、次の情報を更新します。

   * 必要に応じて、レコードタイプ名を編集します。 <!--did they add a field label for this? -->
   * **説明**：レコードタイプの説明を編集または追加し、その詳細を設定します。
   * レコードタイプに関連付けられたアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードタイプを識別するためのカラーを選択します。 これがレコードタイプアイコンの色になります。デフォルトでは、灰色が選択されています。
      * リストからアイコンを選択するか、何を表しているかを示すアイコン名を入力していき、目的のアイコンが表示されたら選択します。これがレコードタイプのアイコンになります。デフォルトでは、ファイルアイコンが選択されています。

     ![](assets/update-record-type-box.png)

1. 「**保存**」をクリックします。
1. （オプション）ワークスペース領域からレコードタイプカードをクリックして、レコードタイプのページを開きます。
1. 「」をクリックします **詳細** レコードタイプ名の右側にあるメニューをクリックし、 **編集** レコードタイプに関する情報を更新します。

   >[!TIP]
   >
   >   ヘッダーでレコードタイプの名前を変更できます。

   ![](assets/more-menu-options-from-record-details-page.png)

   <!--check this screen shot - not sure this is valid ???-->

1. （省略可能） レコードの種類の名前の右側にある下向き矢印を展開し、編集する別のレコードの種類を選択します。
