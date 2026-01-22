---
title: Adobe Workfront Planning Designerの基本を学ぶ
description: Adobe Planning Designerを使用すると、新しい作業領域を生成したり、Workfront Planning のレコード・タイプおよびフィールドを使用して新規作業領域を作成したり、作業領域にオブジェクトを追加したり、レコードの変更履歴を表示したりできます。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 8%

---


# Adobe Workfront Planning Designerの基本を学ぶ

{{planning-important-intro}}

Adobe Planning Designerを使用すると、新しい作業領域を生成したり、Workfront Planning のレコード・タイプおよびフィールドを使用して新規作業領域を作成したり、作業領域にオブジェクトを追加したり、レコードの変更履歴を表示したりできます。

>[!IMPORTANT]
>
>Planning Designerは現在、クローズドベータ版のステージに参加しているユーザーのみが利用できます。

## アクセス要件 <!--edit theses-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよび Planning パッケージ</p>
<p>任意のワークフローおよび計画パッケージ</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 計画Designerのクローズ済Betaプログラムへの登録

<!--edit this Or create a new article under Beta programs?? -->

現在、Planning DesignerのクローズドBetaプログラムへの参加をリクエストできます。

## Designerの計画に関する考慮事項

<!--these are from the AI Assistant - edit these-->

* Planning Designerを使用するには、まず組織の AI アシスタントを有効にする必要があります。 AI アシスタントを組織内の全員が使用できるようにするには、次の機能を有効にする必要があります。

   * 会社のユーザーが AI アシスタントを使用できるようにするには、組織で AI アシスタントを有効にする必要があります。 詳しくは、[AI アシスタントの概要 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) を参照してください。
   * Workfrontで組織の AI アシスタントが有効になると、メインのWorkfront管理者が使用できるようになります。 詳しくは、[システムの基本情報を設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。

   * Workfront管理者は、他のすべてのユーザーに対して AI アシスタントを有効にする必要があります。 詳しくは、[AI アシスタントを有効または無効にする ](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

   * AI アシスタントは、各ページのコンテキストで機能します。 AI アシスタントに対して送信するリクエストでは、開いているページで使用できる機能を参照する必要があります。

* Planning Designerを使用するには、システム管理者が設定の「システム環境設定」領域で有効にする必要があります。

* 計画領域で AI アシスタントが実行するアクションは、Workfront Planning の権限とWorkfrontのアクセスレベルのコンテキストにあります。 詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* ユーザーに代わって AI アシスタントが行った変更は、レコードの履歴パネルで追跡されます。

* コマンドを使用してアクションを取り消すことができます。 例えば、「最後の変更を取り消す」と入力して、変更を元に戻すことができます。

* AI Assistant を使用してオブジェクトを作成、更新、または削除する場合、AI Assistant は意図したアクションを表示し、確認を求めます。 その後、アクションを確認またはキャンセルできます。

—>

## 現在、PlanningDesignerで使用可能な機能

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

計画Designerまたは AI アシスタントを使用して、次のいずれかの操作を実行できます。

* ワークスペースの作成と設定

* レコードタイプの作成

* デザイン フィールドまたは数式フィールド

* レコードの作成、削除、複製、復元

* レコードのフィールドの編集、更新、追加

* レコードを他のレコードにリンク

* レコードの変更履歴へのアクセス

* カスタムビューの作成

* ドキュメントを読み込んでレコードを作成します。 読み込んだドキュメントからレコードを作成する機能は、Planning Designerでのみ使用でき、AI アシスタントでは使用できません。<!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Workfront Planning で PlanningDesignerを見つけます。

Planning Designerには、Workfront Planning のメイン・ページからアクセスできます。

<!--add screen shot-->

また、AI アシスタントを使用して、Planning Designerと同じ機能を利用することもできます。

## 組織の計画Designerを有効にする

Workfront管理者は、最初に組織の Planning Designerを有効にする必要があります。

<!--add steps here-->

## PlanningDesignerを使用したオブジェクトの作成または更新

特に指定がない限り、Workfront Planning Designerまたは AI アシスタントを使用して、Planning でオブジェクトを作成または更新できます。

1. Workfrontにログインし、画面の右上隅にある **メインメニュー** アイコン ![ ドットメインメニュー ](assets/dots-main-menu.png) をクリックするか、左上隅にある **メインメニュー** アイコン ![ ラインメインメニュー ](assets/lines-main-menu.png) をクリックします。

1. **計画** をクリックします。 計画エリアが開きます。

1. **AI でデザイン** をクリックします。

1. 指定されたスペースで、AI アシスタントのコマンドの入力を開始し、完了したら [Enter] をクリックします。

   <!--add screen shot-->

   例えば、次のようなリクエストを入力できます。

   * キャンペーンを管理するための 5 つのレコードタイプを含むワークスペースの作成と設定

   * 今年の各月のマーケティングキャンペーンを作成

   * マーケティングデザイン ワークスペースのステータス用のキャンペーンフィールドを追加

   * 古いステータスのすべてのレコードを削除

   * すべての計画キャンペーンをアクティブのステータスに更新

   * マーケティングデザインワークスペースでのペルソナに対するキャンペーンの接続

   * 「バレンタインデー」キャンペーンの変更履歴を表示

   * マーケティングデザインワークスペースでのキャンペーンのタイムラインビューの作成

   * ドキュメントを読み込んでレコードを作成します。 読み込んだドキュメントからレコードを作成する機能は、Planning Designerでのみ使用でき、AI アシスタントでは使用できません。

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   アシスタントが作成できるサンプルが表示されます。

1. 応答が成功したら、コマンドラインに表示されるリンクに従って、リクエストのオブジェクトを作成、更新またはレビューします。




