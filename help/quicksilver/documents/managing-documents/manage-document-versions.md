---
product-area: documents
navigation-topic: manage-documents
title: ドキュメントバージョンの管理
description: Workfront では、複数のバージョンのドキュメントを管理できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 45%

---

# ドキュメントバージョンの管理

<!-- Audited: 5/2025 -->

Workfront では、複数のバージョンのドキュメントを管理できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>投稿者以上</p>
   <p>リクエスト以上 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを表示</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントに対する表示アクセス権</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* この記事では、ドキュメントに複数のバージョンが含まれていることを前提としています。

  ドキュメントの新しいバージョンを Workfront にアップロードする方法について詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。

## ドキュメントのすべてのバージョンのリストを表示

{{step1-to-documents}}

1. **ドキュメント** ページで、リスト内のドキュメントを選択します。

1. ページの右上隅にある **概要を開く** アイコン ![ 概要を開くアイコン ](assets/qs-summary-in-new-toolbar-small.png) をクリックします。 **ドキュメントの概要** サイドパネルが開きます。

1. 「**バージョン**」セクションまでスクロールすると、すべてのドキュメントバージョンが表示されます。

## 以前のバージョンのドキュメントの詳細の表示と管理

{{step1-to-documents}}

1. ドキュメントにポインタを合わせ、「**ドキュメントの詳細**」をクリックします。

1. **ドキュメントの詳細** ページの上部付近で、名前の横にあるドロップダウンメニューをクリックし、表示および管理するバージョンの名前をクリックします。

   ![ ドキュメントの詳細ページのバージョンドロップダウン ](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   バージョンの詳細を表示するだけでなく、名前、メタデータ、プルーフ設定（ドキュメントプルーフの場合）など、バージョンに変更を加えることができます。

## 単一のドキュメントバージョンのダウンロード

{{step1-to-documents}}

1. **ドキュメント** ページで、リスト内のドキュメントを選択します。

1. ページの右上隅にある **概要を開く** アイコン ![ 概要を開くアイコン ](assets/qs-summary-in-new-toolbar-small.png) をクリックします。 **ドキュメントの概要** サイドパネルが開きます。

1. [**バージョン**] セクションで、バージョンの右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-icon.png) をクリックし、表示されるドロップダウン リストで **ダウンロード** をクリックします。

   ![1 つのドキュメントのダウンロード ](assets/more-versions-350x143.png)

## ドキュメントのすべてのバージョンをダウンロード

{{step1-to-documents}}

1. **ドキュメント** ページで、リスト内のドキュメントを選択します。

1. ページの右上隅にある **概要を開く** アイコン ![ 概要を開くアイコン ](assets/qs-summary-in-new-toolbar-small.png) をクリックします。 **ドキュメントの概要** サイドパネルが開きます。

1. 「**バージョン**」セクションまでスクロールし、「**すべてダウンロード**」をクリックします。

## ドキュメントのバージョンを削除

ドキュメントのバージョンを誤ってアップロードした場合や、バージョンが不要になった場合は、バージョンを削除して元のドキュメントを維持できます。

>[!IMPORTANT]
>
>個別に削除したドキュメントのバージョンは復元できません。

ドキュメントのバージョンを削除する場合は、次の点に注意してください。

* 一度に削除できるバージョンは 1 つだけです。バージョンを削除すると、このアクションはドキュメントの [ 更新 ] セクションに表示されます。
* バージョンを削除した後に新しいバージョンをアップロードすると、新しいバージョンには次の連番が振られます。例えば、1 つのドキュメントに 3 つのバージョンがあり、バージョン 3 を削除した場合、次にアップロードされるドキュメントはバージョン 4 になります。
* バージョンに対して行われたシステム更新やコメントは、バージョンが削除された後も Workfront で保持されます。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

ドキュメントのバージョンを削除するには：

{{step1-to-documents}}

1. **ドキュメント** ページで、リストからドキュメントを選択します。

1. ページの右上隅にある **概要を開く** アイコン ![ 概要を開くアイコン ](assets/qs-summary-in-new-toolbar-small.png) をクリックします。 **ドキュメントの概要** サイドパネルが開きます。

1. 「**バージョン**」セクションまでスクロールすると、すべてのドキュメントバージョンが表示されます。
1. [**バージョン**] セクションで、バージョンの右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-icon.png) をクリックし、表示されるドロップダウン リストで **削除** をクリックします。

   >[!NOTE]
   >
   >* 「**削除**」オプションは、バージョンが少なくとも 2 つある場合にのみ表示されます。
   >* ドキュメントが外部のソースにリンクされている場合、そのリンクは削除され、Workfront を介してドキュメントにアクセスできなくなります。

   ![ ドキュメント バージョンの削除 ](assets/more-versions-350x143.png)
