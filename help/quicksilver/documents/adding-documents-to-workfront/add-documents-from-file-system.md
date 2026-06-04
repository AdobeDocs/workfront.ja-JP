---
product-area: documents
navigation-topic: add-documents-to-workfront
title: ファイルシステムから Adobe Workfront へのドキュメントの追加
description: Adobe Workfront の複数のエリアで、プロジェクト、タスクまたはイシューにドキュメントを追加できます。
author: Courtney, Alina
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/uM4y--i0xyZtRuB-PCZQLnLb8mNwc6YOW6jk4o6LAw0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1317
ht-degree: 43%

---

# ファイルシステムから Adobe Workfront へのドキュメントの追加

Adobe Workfrontには現在、次の2種類のドキュメントストレージがあります。

* 従来のWorkfront ストレージ
* Adobe クラウドストレージ

これらのストレージの種類について詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

>[!NOTE]
>
>一部のお客様は、両方の種類のドキュメントストレージを持っており、WorkfrontまたはAdobe ストレージのみを持っている場合もあります。

Workfrontへのドキュメントの追加は、組織が使用するドキュメント領域のバージョンによって異なります。

* [従来のドキュメント領域でファイルシステムからドキュメントを追加する](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [新しいドキュメント領域でWorkfrontにドキュメントを追加する](#add-documents-to-workfront-in-the-new-documents-area)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>従来のWorkfront ストレージを使用してドキュメントを管理するWorkfront パッケージ</p>
<p>Adobe クラウドストレージを使用してドキュメントを管理するワークフローパッケージ</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>コントリビューター以上</p> 
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>従来のWorkfront ストレージ：ドキュメントへのアクセスを編集する</p> 
   <p>Adobe クラウドストレージ：ドキュメントへの編集アクセスはデフォルトで有効になっており、変更できません</p>
   </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 従来のドキュメント領域でファイルシステムからドキュメントを追加する

組織で従来のWorkfront ストレージを使用している場合、Workfrontでドキュメントにアクセスすると、「従来のドキュメント」領域が表示されます。

Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

Workfrontの次の領域にドキュメントを追加できます。

* メインメニューの「ドキュメント」エリア
* Workfront オブジェクトの「ドキュメント」領域（プロジェクト、タスク、イシュー、テンプレート、テンプレートタスク、ポートフォリオ、プログラム）
* Workfront ボード上の接続されているカード

また、新しいバージョンのドキュメントをアップロードし、Google Drive、Dropbox、Microsoft OneDrive など、サードパーティのクラウドベンダーからのドキュメントへのリンクを追加することもできます。

新しいバージョンのドキュメントの追加について詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。

サードパーティのクラウドベンダーからのドキュメントの追加について詳しくは、[外部アプリケーションからのドキュメントのリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

Workfront にアップロードできるファイルの種類とサイズに制限はありません。 ただし、正常に完了するには、5 分以内にアップロードが完了し、十分なストレージ容量があることが必要です。

ドキュメントの新しいバージョンを Workfront にアップロードする方法について詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。


### 従来のドキュメント領域のWorkfrontへのドキュメントの追加

ワークステーションのファイルシステムから、新しいドキュメントを Workfront に追加できます。 また、Google Drive や SharePoint などのサードパーティアプリケーションからドキュメントをリンクすることもできます。

>[!IMPORTANT]
>
>* 一度に最大150件のドキュメントをアップロードできます。
>* ファイルサイズに制限はありません。
>* ドキュメントのダウンロードは4 GBに制限されています。

ドキュメントを追加するには：

1. 新しいドキュメントを追加するWorkfront オブジェクトに移動します。
1. 「**ドキュメント**」タブをクリックし、**新規を追加** ドロップダウンメニューをクリックします。

   ![新しいドキュメントを追加](assets/add-new-doc.png)

1. 追加するドキュメントの種類に応じて、次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ワークステーションのファイルシステムからのドキュメントのアップロード</td> 
      <td> 
       <ol> 
        <li value="1"><strong>新しい</strong>を追加ドロップダウンメニューから、<strong>文書を選択します。</strong></li> 
        <li value="2"> <p>ワークステーション上のファイルシステムから、追加するドキュメントを参照して選択します。<br></p> <p>Shift キーを押しながら追加のファイルを選択すると、複数のドキュメントを選択できます。</p> </li> 
        <li value="3">「<strong>開く</strong>」をクリックします。</li> 
       </ol> 
       <p><b>メモ</b>：ファイルマネージャーから直接ドキュメントリストにファイルをドラッグ＆ドロップすることもできます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Google Drive や SharePoint などのサードパーティアプリケーションからのドキュメントのアップロード</td> 
      <td> 
       <ol> 
        <li value="1"> <p>「<strong>新しい</strong>を追加」ドロップダウンメニューから、「<strong>&lt;name_of_third-party_application&gt;</strong>」を選択します。</p> <p>例えば、Google Drive からドキュメントをアップロードするには、<strong>From Google Drive</strong> をクリックします。</p> </li> 
        <li value="2"> <p>プロンプトに従って、サードパーティアプリケーションでドキュメントを選択します。<br></p> <p>リンクされたドキュメントについて詳しくは、<a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">外部アプリケーションからのドキュメントのリンク</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">別の Workfront ユーザーからのドキュメントのリクエスト</td> 
      <td> 
       <ol> 
        <li value="1"><strong>新しい</strong>を追加ドロップダウンメニューから、<strong> ドキュメントをリクエスト </strong>を選択します。</li> 
        <li value="2"><strong>誰からリクエストしますか</strong>ボックスに、ドキュメントをリクエストするユーザーの名前を入力します。</li> 
        <li value="3"><strong>リクエスト内容を伝える</strong>ボックスに、ドキュメントの名前を入力します。</li> 
        <li value="4"> <p><strong>リクエストを送信</strong>をクリックします。</p> <p>リクエストが「ドキュメント」タブに表示されます。</p> <p>ドキュメントのリクエストについて詳しくは、<a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">ドキュメントのリクエスト</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

   選択したオブジェクトの「文書」セクションに文書が追加されます。

## 新しいドキュメント領域でWorkfrontにドキュメントを追加する

Adobe クラウドストレージモデルを使用して、オブジェクトにドキュメントを追加できます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

新しいドキュメント領域で現在サポートされていない機能：

* メインメニューの「文書」領域への文書のアップロード
* Google Drive、Dropbox、Microsoft OneDriveなど、サードパーティのクラウドベンダーからのドキュメントへのリンクの追加。
* 文書の要求
* フォルダーへのリンクのコピー
* ドキュメントのチェックアウト
* クリップボードからの画像のペースト
* スマートフォルダーの追加

### 新しいドキュメント領域でWorkfrontにドキュメントを追加する

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

ドキュメントを追加するには：

1. 新しいドキュメントを追加するWorkfront オブジェクトに移動します。
1. 左側のパネルで「**ドキュメント**」セクションをクリックします。
1. ページの右側にある&#x200B;**新規**&#x200B;をクリックするか、表示されるドロップゾーンにファイルをドラッグ&amp;ドロップします。 一度に複数のドキュメントを追加できます。

   ![新しいドキュメントを追加](assets/add-new-doc-new-doc.png)

ドキュメントの新しいバージョンを Workfront にアップロードする方法について詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。

ドキュメントをアップロードするオブジェクトと同じ名前のフォルダーが「ドキュメント」セクションに自動的に作成され、ドキュメントがフォルダーに追加されます。

## Adobe クラウドストレージのドキュメントセキュリティ

Workfrontは、次の方法で、ウイルスやその他の悪意のあるコンテンツがドキュメントを介してサイトに入るのを防ぎます。

**Workfront が破損ファイルを検出する方法**

Adobe クラウドストレージモデルを使用すると、オブジェクトのドキュメントスキャンが自動的に有効になります。

500 MB未満のすべてのファイルは、アップロード時にスキャンされます。 500 MBを超えるファイルはスキャンされません。 Workfrontで破損したドキュメントが検出された場合、そのドキュメントは自動的に削除されます。

**ファイル名の制限**

この統合はAdobe クラウドストレージを使用して構築されているので、プロジェクトやドキュメントを管理する際に認識すべき構造や命名規則がいくつかあります。

* オブジェクト名は一意である必要があり、重複することはできません
* Adobe クラウドストレージでは、階層ツリー内に同じ親を持つピアオブジェクトに一意の名前が必要です
* ドキュメントが同じプロジェクトに属している場合、同じ名前を付けることはできません
* 文書名に次の特殊文字を含めることはできません：`\ / : * ? " | < >`
* ドキュメント名は最大255文字に制限されています

これらの制限を念頭に置いて、Workfrontでは、競合を防ぐために、必要に応じてオブジェクトまたはドキュメントの名前が自動的に変更されます。


## レガシーWorkfront ストレージのドキュメントセキュリティ

Workfrontは、次の方法で、ウイルスやその他の悪意のあるコンテンツがドキュメントを介してサイトに入るのを防ぎます。

**Workfront が破損ファイルを検出する方法**

ドキュメントスキャンは、リクエストに応じてのみ、組織に対して有効になっています。

ドキュメントスキャンが有効な場合、25 MB 未満のファイルはアップロード時にスキャンされます。 25 MB を超えるファイルはスキャンされません。

Workfrontが破損した文書を検出すると、ファイルが破損していることを示すメッセージが表示されます。 また、Workfront が悪質な可能性のあるコンテンツを検出し、ファイルの削除が予定されている場合にも、メール通知が送信されます。

破損したファイルは、手動で削除しない限り、検出から24時間以内に削除されます。 破損したファイルを削除すると、Workfront はこのアクションを更新として追跡します。 Workfront による削除を許可した場合、更新は記録されません。

**ファイル名の制限**

Workfront にアップロードされるファイルの名前には、特定の文字を含めることができません。 ファイル名に `! # % * \ | ' " / ? < > { } [ ]` のいずれかの文字が含まれている場合、その文字はファイルのアップロード時にファイル名から削除されます。
