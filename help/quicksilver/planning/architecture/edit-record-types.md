---
title: レコードタイプの編集
description: 保存後にレコードタイプを編集できます。レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 57%

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

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。自分または他のユーザーが作成したレコードタイプの外観を編集できます。Workfront Planning レコードタイプの作成について詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

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
   <p> Adobe Workfront</p> <p>Adobe Workfront Planning のレコードタイプを Experience Manager Assets に接続するには、Adobe Experience Manager Assets ライセンスが必要です。組織の Workfront インスタンスが Adobe Business Platform または Adobe Admin Console にオンボーディングされている必要があります。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
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
   <td> <p>Workfront Planning に対するアクセスレベルのコントロールはありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## レコードタイプの編集

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。

   ワークスペースが開き、レコードタイプが表示されます。
1. レコードタイプのカードの上にマウスポインターを置き、レコードタイプのカードの右上隅にある **詳細** メニュー ![](assets/more-menu.png) ージをクリックしてから、**編集** をクリックしてください。

   ![](assets/more-menu-options-from-record-type-card.png)

1. **レコードタイプを編集** ボックスで、次の情報を更新します。

   * 必要に応じて、レコードタイプ名を編集します。<!--did they add a field label for this? -->
   * **説明**：詳しい情報を含むレコードタイプの説明を編集または追加します。
   * レコードタイプに関連付けられたアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードタイプを識別するための色を選択します。これは、レコードタイプアイコンの色です。灰色はデフォルトで選択されています。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。

     ![](assets/update-record-type-box.png)

1. **保存**&#x200B;をクリックします。
1. （オプション）ワークスペースエリアでレコードタイプカードをクリックして、レコードタイプのページを開きます。
1. レコードタイプ名の右側にある **詳細** メニューをクリックし、**編集** をクリックして、レコードタイプに関する情報を更新します。

   >[!TIP]
   >
   >   ヘッダーでレコードタイプの名前を変更できます。

   ![](assets/more-menu-options-from-record-type-page.png)

   <!--check this screen shot - not sure this is valid ???-->

1. （オプション）別のレコードの種類を編集するには、レコードの種類名の右側にある下向き矢印を展開し、レコードの種類を検索してから、一覧に表示されたら選択します。
