---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードへのリクエストキューの埋め込み
description: 新しいリクエストキューをダッシュボードに埋め込むと、リクエストエリアに移動せずに、ユーザがリクエストキューに直接アクセスできるようになります。
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 2894161b61a00dab04c17ef642ace4a45179eb17
workflow-type: ht
source-wordcount: '1178'
ht-degree: 100%

---

# ダッシュボードへのリクエストキューの埋め込み

新しいリクエストキューをダッシュボードに埋め込むと、リクエストエリアに移動せずに、ユーザがリクエストキューに直接アクセスできるようになります。 

例えば、ヘルプデスクキューや、全員が定期的にアクセスする必要がある PTO リクエストキューなど、組織全体に公開されているリクエストキューがある場合、リクエストキューをダッシュボードの 1 つに直接挿入して、素早く簡単にアクセスできるようにすると便利な場合があります。この設定手順は、ダッシュボードで外部ページを作成する手順と似ています。

まず、リクエストキューへの URL を取得する必要があります。次に、外部ページを追加して、URL をダッシュボードに埋め込むことができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

ダッシュボードにリクエストキューを埋め込む前に、以下の両方を作成する必要があります。

* **ダッシュボード**：ダッシュボードの作成について詳しくは、[ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)を参照してください。
* **リクエストキュー**：リクエストキューの作成について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

## リクエストキューの URL を取得 {#obtain-the-url-of-the-request-queue}

リクエストキューの URL は、ユーザーがダッシュボードからアクセスしたときに、リクエストキューのどの部分をユーザーに公開したいかにより、複数の方法で取得できます。

* [リクエストタイプを変更できる特定のキュートピックへのリンクを取得](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [リクエストキューへのリンクとリクエストタイプを変更できる機能を取得](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [リクエストタイプを変更できないリクエストキューへのリンクを取得](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### リクエストタイプを変更できる特定のキュートピックへのリンクを取得 {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

特定のキュートピックへのリンクを他のユーザーと共有すると、リクエストフォームは、リクエストの送信に使用する必要がある正確なキュートピックで開きます。これは、特定のリクエストキューのリクエストをログに記録するときに、ユーザーがどのキュートピックを選択すればよいかわからない場合に役立ちます。

ユーザーは、リクエストのタイプを変更したり、必要に応じて別のトピックを選択したりすることができます。リクエストエリアのナビゲーションも表示されます。

1. **メインメニュー**／**リクエスト**／**新規リクエスト**&#x200B;をクリックします。
1. 特定のキューを共有する場合は、ダッシュボードで共有するキューに到達するまで、トピックグループとキュートピックの選択を続けます。リクエストの送信について詳しくは、[Adobe Workfront のリクエストの作成および送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

   >[!TIP]
   >
   >トピックグループとキュートピックの選択はオプションです。

1. 新規リクエストエリアの右上隅にある「**パスを共有**」をクリックします。

   これにより、リクエストキューまたはキュートピックへのリンクが、画面に表示された状態でコピーされます。ユーザーは、リクエストタイプ、または利用可能なトピックグループおよびキュートピックを更新できます。

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### リクエストキューへのリンクとリクエストタイプを変更できる機能を取得 {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

リクエストタイプへのリンクを共有する場合、そのユーザーに対してリクエストタイプが選択されます。これは、ユーザーが同じリクエストタイプに対して複数のトピックグループまたはキュートピックから選択する必要がある場合に役立ちます。ユーザーはリクエストタイプを変更し、別のリクエストタイプを選択できます。リクエストエリアのナビゲーションも表示されます。

1. リクエストキューとして指定されたプロジェクトに移動します。

   プロジェクトからのリクエストキューの作成について詳しくは、[リクエストキューを作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)に移動してください。

1. **キューの詳細**&#x200B;に移動します。
1. 「**ダイレクトアクセス URL**」フィールドで見つけたコードをコピーします。

   コードは次のようになります。

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   これは、選択したプロジェクトに関連付けられたリクエストキューへのリンクです。リクエストタイプは事前に選択されています。

   ユーザーは、必要なトピックグループやキュートピックを選択したり、別のリクエストタイプを選択したりすることができます。

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### リクエストタイプを変更できないリクエストキューへのリンクを取得 {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

事前に選択されたリクエストタイプへのリンクを共有した場合、そのリクエストタイプはユーザーに対して選択され、変更できません（グレー表示になります）。ユーザーは、必要なトピックグループやキュートピックを選択できます。これは、ユーザーに他のリクエストタイプを表示および選択させたくない場合に役立ちます。リクエストエリアのナビゲーションは表示されません。

1. リクエストキューとして指定されたプロジェクトに移動します。

   プロジェクトからのリクエストキューの作成について詳しくは、[リクエストキューを作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)に移動してください。

1. **キューの詳細**&#x200B;に移動します。
1. 「**埋め込みコード**」フィールドに見つけたコードをコピーします。

   コードは次のようになります。

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. コードを編集して、以下の情報のみを保持します。

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >`<samp>iframe </samp>` タグを追加して、Workfront 以外のアプリケーションにコードを埋め込むこともできます。

   これは、選択したプロジェクトに関連付けられたリクエストキューへのリンクです。リクエストタイプは事前に選択されており、変更できません。

   ユーザーは、選択したリクエストタイプに必要な任意のトピックグループまたはキューのトピックを選択できます。別のリクエストタイプは選択できません。

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## ダッシュボードへのリクエストキューの埋め込み

リクエストキューへのリンク、またはリクエストキューの下にネストされたキュートピックへのリンクをダッシュボードに埋め込むと、ユーザーはリクエストの入力に直接アクセスできます。

1. この記事の[リクエストキューの URL の取得](#obtain-the-url-of-the-request-queue)の節で説明されている方法のいずれかを使用して、リクエストキュー URL を取得します。
1. **メインメニュー**／**ダッシュボード**／**新規ダッシュボード**&#x200B;をクリックします。
1. ダッシュボードの&#x200B;**名前**&#x200B;を入力します。必須フィールドです。
1. 「**外部ページを追加**」をクリックします。

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. 「**外部ページを追加**」ボックスで、次のフィールドを編集します。

   * **名前**：ダッシュボードに表示するリクエストキューの名前を入力します。必須フィールドです。

   * **説明**：この外部ページに表示される説明を入力します。これは必須フィールドではなく、レポート目的でのみ重要です。ダッシュボードには表示されません。
   * **URL**：手順 1 で取得した URL を以下の方法のいずれかでペーストします。

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **高さ**：外部ページの高さを入力します。これは、リクエストキューを含む外部ページがダッシュボード上で占めるスペースを定義するものです。これは必須フィールドで、デフォルト値は 500 です。

1. 「**保存**」をクリックします。
1. 「**保存して閉じる**」をクリックします。

   リクエストキューは、ダッシュボードに別個のダッシュボードコンポーネントとして表示されます。

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. （オプション）「**ダッシュボードのアクション**」をクリックして、「**編集**」をクリックして、同じダッシュボードにレポート、カレンダーまたはさらに外部ページを追加します。\
   ダッシュボードへのコンポーネントの追加について詳しくは、[ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)を参照してください。

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
