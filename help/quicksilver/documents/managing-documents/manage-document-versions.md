---
product-area: documents
navigation-topic: manage-documents
title: ドキュメントバージョンの管理
description: Workfront では、複数のバージョンのドキュメントを管理できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 46%

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
   <td> <p>従来のWorkfront ストレージを使用してドキュメントを管理するWorkfront パッケージ</p>
<p>Adobe エンタープライズストレージを使用してドキュメントを管理するワークフローパッケージ</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>コントリビューター以上</p>
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

1. On the **Documents** page, select a document in the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. Scroll down to the **Versions** section to view all the document versions.

## 以前のバージョンのドキュメントの詳細の表示と管理

{{step1-to-documents}}

1. ドキュメントにポインタを合わせ、「**ドキュメントの詳細**」をクリックします。

1. Near the top of the **Document Details** page, click the drop-down menu next to the name, then click the name of the version you want to view and manage.

   ![Version drop-down on the Document Details page](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Along with viewing the version&#39;s details, you can make changes to the version, such as its name, metadata, and proofing settings (if it&#39;s a document proof).

## 単一のドキュメントバージョンのダウンロード

{{step1-to-documents}}

1. On the **Documents** page, select a document in the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. In the **Versions** section, click the click the **More** menu ![More menu](assets/more-icon.png) to the right of the version, then click **Download** in the drop-down list that appears.

   ![Download a single document](assets/more-versions-350x143.png)

## ドキュメントのすべてのバージョンをダウンロード

{{step1-to-documents}}

1. On the **Documents** page, select a document in the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. Scroll down to the **Versions** section and then click **Download All**.

## ドキュメントのバージョンを削除

ドキュメントのバージョンを誤ってアップロードした場合や、バージョンが不要になった場合は、バージョンを削除して元のドキュメントを維持できます。

>[!IMPORTANT]
>
>個別に削除したドキュメントのバージョンは復元できません。

ドキュメントのバージョンを削除する場合は、次の点に注意してください。

* 一度に削除できるバージョンは 1 つだけです。 If a version is deleted, this action appears in the Updates section on the document.
* バージョンを削除した後に新しいバージョンをアップロードすると、新しいバージョンには次の連番が振られます。 例えば、1 つのドキュメントに 3 つのバージョンがあり、バージョン 3 を削除した場合、次にアップロードされるドキュメントはバージョン 4 になります。
* バージョンに対して行われたシステム更新やコメントは、バージョンが削除された後も Workfront で保持されます。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

ドキュメントのバージョンを削除するには：

{{step1-to-documents}}

1. On the **Documents** page, select the document from the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. Scroll down to the **Versions** section to view all the document versions.
1. In the **Versions** section, click the click the **More** menu ![More menu](assets/more-icon.png) to the right of the version, then click **Delete** in the drop-down list that appears.

   >[!NOTE]
   >
   >* The **Delete** option is visible only if there are at least 2 versions.
   >* ドキュメントが外部のソースにリンクされている場合、そのリンクは削除され、Workfront を介してドキュメントにアクセスできなくなります。

   ![&#x200B; ドキュメントのバージョンを削除](assets/more-versions-350x143.png)
