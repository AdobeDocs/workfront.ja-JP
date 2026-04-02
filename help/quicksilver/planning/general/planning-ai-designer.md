---
title: Adobe Workfront計画Designerの基本を学ぶ
description: AIを活用したAdobe Planning Designerを使用すると、ワークスペースとデータ構造を簡単に設定できます。 Planning Designerは、ワークスペースの作成と設定、フィールドと式の定義、レコードの管理、変更履歴の確認、カスタムビューの構築など、あらゆることをサポートしています。 直接またはAI アシスタントを通じて使用する場合でも、Planning Designerは、構造化され、連続性のある情報を構築および管理するための柔軟で強力な環境を提供します。
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 442ddab8c7b92d52e0de699bb7acf99a5ca0f215
workflow-type: tm+mt
source-wordcount: '1524'
ht-degree: 8%

---

# Adobe Workfront計画Designerの基本を学ぶ

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designerは、現在、クローズしたBeta プログラムに参加しているユーザーのみが使用できます。
>
>この記事の情報は、Adobe Workfront の追加機能である Adobe Workfront Planning に関するものです。
>
>Workfront Planning へのアクセス要件のリストについて詳しくは、[Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。
> 
>Workfront計画の一般的な詳細については、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。

AIを活用したAdobe Planning Designerを使用すると、ワークスペースとデータ構造を簡単に設定できます。 Planning Designerは、ワークスペースの作成と設定、フィールドと式の定義、レコードの管理、変更履歴の確認、カスタムビューの構築など、あらゆることをサポートしています。

直接またはAI アシスタントを通じて使用する場合でも、Planning Designerは、構造化され、連続性のある情報を構築および管理するための柔軟で強力な環境を提供します。

Workfront Planningについて詳しくは、次の記事を参照してください。

* [Adobe Workfront計画の一般的な情報と記事インデックス](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfront Planning の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)


## アクセス要件<!--edit theses??-->

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
<p>任意のWorkfrontおよびプランニングパッケージ</p>
<p>任意のワークフローとプランニングパッケージ</p>
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## プランニングDesignerのクローズ済みBeta プログラムへの登録

現在、Planning Designerのクローズ済みBeta プログラムへの参加をリクエストするには、sargism@adobe.comに電子メールを送信します。

メールを受け取った後、エンジニアリングチームはWorkfront インスタンスのPlanning Designerをオンにします。

>[!IMPORTANT]
>
>Planning Designerがシステムで使用可能になる前に、最初にAI Assistant契約書に同意する必要があります。

## Planning Designerに関するフィードバックの送信

ベータプログラム中に、Planning Designerに関するフィードバックを送信できます。

1. Workfrontにログインし、左上隅の&#x200B;**メインメニュー** アイコン ![行メインメニュー](assets/lines-main-menu.png)をクリックしてから、**計画**&#x200B;をクリックします。

   **計画**&#x200B;領域が開きます。

1. 「**AIを使用して作成**」をクリックします。<!--update this tag name when they change it-->

   **計画Designer** ウィンドウが開きます。

1. ページの下部にある&#x200B;**フィードバックを送信**&#x200B;をクリックします。
1. 提供されたスペースにフィードバックを追加し、**送信**&#x200B;をクリックします。
ご意見はエンジニアリングチームと製品チームに送信されます。

## Planning Designerに関する考慮事項

* Planning Designerを使用するには、まず組織のAI アシスタントをオンにする必要があります。 AI アシスタントを組織内のすべてのユーザーが利用できるようにするには、次の手順を実施する必要があります。

   * Workfrontでは、AI アシスタントを利用できる必要があります。

     詳しくは、[AI アシスタントの前提条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)を参照してください。
   * WorkfrontでAI アシスタントを組織で使用できるようにすると、Workfrontのメイン管理者がアクセスできるようになります。

     詳しくは、[システムの基本情報を設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。
   * Workfront管理者は、AI アシスタント契約書に同意し、他のすべてのユーザーに対してAI アシスタントをオンにする必要があります。

     詳しくは、[AI アシスタントの有効化または無効化](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)を参照してください。
* システム管理者が組織のAI アシスタントを有効にした後、組織で利用可能になった場合、デフォルトで、すべてのユーザーがPlanning Designerを使用できます。
* Planning Designerで実行するアクションは、Planning領域で使用する場合、AI Assistantでも実行できます。
* 計画領域でAI アシスタントによって実行されるアクションまたは計画Designerによって実行されるアクションは、Workfront計画の権限とWorkfront アクセスレベルのコンテキストにあります。

  詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* AI アシスタントまたはPlanning Designerがユーザーの代わりに行った変更は、レコードの履歴パネルで追跡されます。

* 計画Designerによって行われたアクションは永続的であり、元に戻せない可能性があります。 例えば、フィールドの削除を元に戻すことはできません。 Designerが提案したすべての措置を承認する前に再検討する。

  >[!IMPORTANT]
  >
  >Planning Designerを使用してオブジェクトを作成、更新または削除する場合、取り消せないアクションに対してのみ確認を求めるプロンプトが表示されます。 例えば、レコードタイプやワークスペースの削除は元に戻せません。 レコードの削除は行われません。 Planning Designerは、レコードタイプまたはワークスペースを削除する場合にのみ、確認を求めます。

* Planning Designerを使用してワークスペースとレコードタイプを作成すると、ビューとフィールドも自動的に作成されます。

## Planning Designerで現在使用できる機能

Planning DesignerまたはAI アシスタントを使用して、次のいずれかのアクションを実行できます。

* ワークスペースの作成と設定

<!--On March 2: * Edit workspaces-->

* グローバルなレコードタイプの定義やワークスペースへの追加など、レコードタイプを作成します

* フィールドまたは数式フィールドのデザイン

* レコードの作成、削除、複製、復元

* レコードのフィールドを編集、更新、追加する

* レコードを他のレコードにリンク

* アクセス レコードの変更履歴

* カスタムビューの構築

* ドキュメントを読み込んでレコードを作成する

  例えば、組織図の画像を社内にアップロードし、その画像をもとにPlanning Designerでワークスペースを作成できます。

  読み込んだドキュメントからオブジェクトを作成できるのは、Planning Designerのみで、AI アシスタントでは使用できません。

  >[!IMPORTANT]
  >
  >.XLSX ファイル形式はサポートしていますが、Planning Designerを使用した大規模なレコード読み込みには使用できません。
  >現時点でかなりの数のレコードをインポートする必要がある場合は、Planningで使用可能な手動機能を使用してインポートすることをお勧めします。
  >
  >詳しくは、[CSVまたはExcel ファイルから情報を読み込んでレコードを作成](/help/quicksilver/planning/records/import-file-to-create-records.md)を参照してください。
  >ファイルタイプの制限については、[AIによるフォーム入力を使用してプロンプトまたはドキュメントを使用してリクエストを入力する](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)の「 アップロードしたドキュメントに基づいて提案を取得する」セクションを参照してください。


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Planning Designerを使用したオブジェクトの作成または更新

特に指定がない限り、Workfront Planningでオブジェクトを作成または更新するには、Planning DesignerまたはAI アシスタントを使用します。

1. Workfrontにログインし、左上隅の&#x200B;**メインメニュー** アイコン ![行メインメニュー](assets/lines-main-menu.png)をクリックしてから、**計画**&#x200B;をクリックします。

   **計画**&#x200B;領域が開きます。<!--update screen shot when they change the name of the button-->

   ![&#x200B; ワークスペースページ上のAI ボタンを使用したデザイン &#x200B;](assets/design-with-ai-button-on-workspaces-page.png)

1. 「**AIを使用して作成**」または「**ワークスペースを作成**」をクリックし、上部のプロンプトウィンドウを使用して、作成するワークスペースの種類を指定します。<!--update this when they change it to Generate with AI-->

   **計画Designer** ウィンドウが開きます。<!--remove the Beta tag here when this removes from Beta-->

   ![Designer ウィンドウの計画](assets/planning-designer-window.png)

1. 提供されたスペースで、AI アシスタントのプロンプトを入力し始め、完了したら「Enter」をクリックします。

   <!--add screen shot-->

   例えば、次のようなプロンプトを入力できます。

   * 5つのレコードタイプを含むワークスペースを作成して設定し、キャンペーンを管理できます

   * 今年度の各月のマーケティング施策の作成

   * マーケティングデザインワークスペースのステータスのキャンペーンフィールドを追加します

   * ステータスが「古い」のすべてのレコードを削除

   * すべての計画キャンペーンをアクティブのステータスに更新します

   * マーケティングデザインワークスペースでキャンペーンをペルソナに接続すると

   * 「バレンタインデー」キャンペーンの変更履歴の表示

   * マーケティングデザインワークスペースでキャンペーンのタイムラインビューを構築する

   * ドキュメントを読み込んでレコードを作成します。 読み込んだドキュメントからレコードを作成できるのは、Planning Designerのみで、AI アシスタントでは使用できません。

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. 応答が成功したら、プロンプト領域に表示されるリンクに従って、リクエストのオブジェクトを作成、更新、レビューします。

   オブジェクトの作成に同意すると、変更内容がプロンプト領域の右側に表示されます。

   ワークスペース、レコードタイプ、フィールド、ビュー、レコードは、プロンプトの右側にあるプレビュー領域で表示できます。

   >[!TIP]
   >
   >確認を必要とせずに、すぐに作成されるオブジェクトもあります。

1. （オプション）追加のプロンプトを入力して、オブジェクトをさらに編集します。
1. （オプション）「**プレビュー画面を表示または非表示にする**」アイコン「![&#x200B; プレビュー画面を表示または非表示にする](assets/hide-show-preview-screen-in-planning-designer.png)」をクリックして、右側のプレビュー画面を開いたり閉じたりします。
1. **新しいタブでワークスペースを開くアイコン** ![新しいタブでワークスペースを開くアイコン &#x200B;](assets/open-workspace-on-new-tab-icon.png)をクリックして、新しいタブで更新しているワークスペースを開きます。
1. **閉じる** アイコン **X**&#x200B;をクリックして、プランニング Designerを閉じ、ワークスペース エリアを開きます。
1. （オプション）ワークスペースを編集するには、次のいずれかの操作を行います。

   * ワークスペースを開き、手動で変更します。 詳しくは、[ワークスペースの編集](/help/quicksilver/planning/architecture/edit-workspaces.md)を参照してください。
   * 「**AIで編集**」をクリックします。 これでPlanning Designerが開きます。 上記の手順を繰り返して、AIを使用し、ワークスペースをさらに変更します。

## 組織のプラン作成Designerをオフにします

Workfront管理者がAI アシスタント契約書に同意すると、デフォルトで、組織内のすべてのユーザーに対してPlanning Designerがオンになります。

オフにするには：

1. Workfront as a System Administratorにログインします。
1. 画面の左上隅にある&#x200B;**メインメニュー** ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-shell.png)をクリックし、**設定**&#x200B;をクリックします。
1. 左側のパネルで&#x200B;**システム**>をクリックし、**AI環境設定**&#x200B;領域に移動します。
1. 「**オンボーディング計画**」設定をオフにします。<!--add new screen shot with info icon and new name of the toggle; ensure you don't show the AI Reviewer if it is not in Prod yet-->

   ![&#x200B; システム環境設定でのDesigner設定の計画](assets/planning-designer-toggle-in-system-preferences.png)
1. 「**保存**」をクリックします。

   これにより、システム内のすべてのユーザーのPlanning Designerが削除されます。
