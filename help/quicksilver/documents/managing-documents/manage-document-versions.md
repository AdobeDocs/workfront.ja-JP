---
product-area: documents
navigation-topic: manage-documents
title: ドキュメントバージョンの管理
description: Workfrontでは、複数のバージョンのドキュメントを管理できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# ドキュメントバージョンの管理

Workfrontでは、複数のバージョンのドキュメントを管理できます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントへのアクセスを表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

* この記事では、ドキュメントに複数のバージョンが含まれていることを前提としています。

   ドキュメントの新しいバージョンをWorkfrontにアップロードする方法について詳しくは、 [新しいバージョンのドキュメントをアップロード](../../documents/managing-documents/upload-new-document-version.md).

## ドキュメントのすべてのバージョンのリストを表示

1. 「概要」で、「 **すべてのバージョン** 」セクションに入力します。 ここで、ドキュメントのすべてのバージョンを表示できます。

## 以前のバージョンのドキュメントの詳細を表示および管理します

1. ドキュメントの詳細ページの上部付近で、名前の横にあるドロップダウンメニューをクリックし、表示および管理するバージョンの名前をクリックします。

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   バージョンの詳細の表示に加えて、バージョンの名前、メタデータ、校正設定（ドキュメント配達確認の場合）などのバージョンを変更できます。

## 単一のドキュメントバージョンのダウンロード

1. 概要で、 **バージョン**、その他メニューをクリックします。 ![](assets/more-icon.png) をクリックし、 **ダウンロード** 」と入力します。

   ![](assets/more-versions-350x143.png)

## ドキュメントのすべてのバージョンをダウンロード

1. クリック **ドキュメントの詳細**&#x200B;を選択し、「 **すべてのバージョン** をクリックします。

1. クリック **すべてダウンロード** をクリックします。

## ドキュメントバージョンの削除

誤ってドキュメントのバージョンをアップロードした場合や、バージョンが不要になった場合は、バージョンを削除して元のドキュメントを維持できます。

>[!IMPORTANT]
>
>個別に削除したドキュメントバージョンは復元できません。

ドキュメントのバージョンを削除する場合は、次の点に注意してください。

* 一度に削除できるバージョンは 1 つだけです。 バージョンが削除された場合、このアクションは **更新** 」と入力します。
* バージョンを削除した後に新しいバージョンをアップロードすると、新しいバージョンは次の連番を受け取ります。 例えば、1 つのドキュメントに 3 つのバージョンがあり、バージョン 3 を削除した場合、次にアップロードされるドキュメントはバージョン 4 になります。
* バージョンに対しておこなわれたシステム更新やコメントは、バージョンが削除された後もWorkfrontで保持されます。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

ドキュメントのバージョンを削除するには：

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「 」を選択します。 **ドキュメント**&#x200B;必要なドキュメントを検索します。
1. 内 **バージョン** 「概要」領域で、バージョンをクリックし、 **削除** 」と入力します。 この **削除** オプションは、少なくとも 2 つのバージョンがある場合にのみ表示されます。

   ドキュメントが外部のソースにリンクされている場合、そのリンクは削除され、Workfrontからドキュメントにアクセスできなくなります。

   ![](assets/more-versions-350x143.png)
