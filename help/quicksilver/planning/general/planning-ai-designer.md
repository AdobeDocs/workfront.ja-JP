---
title: Adobe Workfront Planning Designerの基本を学ぶ
description: AI を活用したAdobe プランニング Designerを使用して、ワークスペースとデータ構造を簡単に設定できます。 Planning Designerは、ワークスペースの作成と構成から、フィールドと式の定義、レコードの管理、変更履歴の確認、およびカスタム ビューの作成まで、すべてをサポートします。 Planning Designerは、直接使用する場合も、AI アシスタントを通じて使用する場合も、構造化されたコネクテッド情報を構築および管理するための柔軟で強力な環境を提供します。
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
source-git-commit: b52c188d767ee37699ead71ed90642458d9889fa
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 4%

---


# Adobe Workfront Planning Designerの基本を学ぶ

>[!IMPORTANT]
>
>Planning Designerは現在、クローズドBetaプログラムに参加しているユーザーのみが利用できます。
>
>この記事では、Adobe Workfrontの追加機能であるAdobe Workfront Planning について説明します。
>
>Adobe Workfront Planning にアクセスするための要件の一覧については、[Workfront Planning アクセスの概要 &#x200B;](/help/quicksilver/planning/access/access-overview.md) を参照してください。
> 
>Adobe Workfront Planning の一般情報については、[Workfront Planning の基本を学ぶ &#x200B;](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

AI を活用したAdobe プランニング Designerを使用して、ワークスペースとデータ構造を簡単に設定できます。 Planning Designerは、ワークスペースの作成と構成から、フィールドと式の定義、レコードの管理、変更履歴の確認、およびカスタム ビューの作成まで、すべてをサポートします。

Planning Designerは、直接使用する場合も、AI アシスタントを通じて使用する場合も、構造化されたコネクテッド情報を構築および管理するための柔軟で強力な環境を提供します。

Workfrontの計画について詳しくは、次の記事を参照してください。

* [Adobe Workfrontの計画に関する一般情報](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfrontの計画の概要](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning のアクセスの概要](/help/quicksilver/planning/access/access-overview.md)


## アクセス要件 <!--edit theses??-->

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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 計画Designerのクローズド Beta プログラムへの登録

現在、sargism@adobe.comにメールを送信することで、Planning DesignerのクローズドBetaプログラムへの参加をリクエストできます。

メールが届いたら、エンジニアリングチームがWorkfront インスタンスで Planning Designerを有効にします。

>[!IMPORTANT]
>
>計画Designerをシステムで使用するには、まず会社が AI アシスタント契約に同意する必要があります。

## Planning Designerに関するフィードバックの送信

ベータ版プログラム中に、Planning Designerに関するフィードバックを送信できます。

1. Workfrontにログインし、左上隅の **メインメニュー** アイコン ![&#x200B; ラインメインメニュー &#x200B;](assets/lines-main-menu.png) をクリックして、「**計画**」をクリックします。

   **計画** エリアが開きます。

1. **AI で作成** をクリックします。<!--update this tag name when they change it-->

   **計画Workspace** ウィンドウの **Designer設定** エリアが開きます。<!--replace shot below when they rename the area to Planning Designer-->

1. ページ下部の **フィードバックを送信する** をクリックします。
1. 表示されたスペースにフィードバックを追加し、「**送信**」をクリックします。
フィードバックは、エンジニアリングチームと製品チームに送信されます。

## Designerの計画に関する考慮事項

* Planning Designerを使用するには、まず組織の AI アシスタントを有効にする必要があります。 AI アシスタントを組織内の全員が使用できるようにするには、次の設定が必要です。

   * Workfrontは、AI アシスタントを組織で使用できるようにする必要があります。

     詳しくは、[AI アシスタントの前提条件 &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) を参照してください。
   * Workfrontが AI アシスタントを組織で使用できるようになったら、Workfrontのメイン管理者がアクセスできます。

     詳しくは、[システムの基本情報を設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。
   * Workfront管理者は AI Assistant 契約に同意し、他のすべてのユーザーに対して AI Assistant を有効にする必要があります。

     詳しくは、[AI アシスタントを有効または無効にする &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。
* システム管理者が組織の AI アシスタントを有効にすると、Planning Designerが組織で使用可能になっている場合、デフォルトではすべてのユーザーが使用できます。
* 計画Designerで実行されるアクションは、計画エリアで AI アシスタントを使用して実行することもできます。
* 計画領域で AI アシスタントが実行するアクションや、計画Designerが実行するアクションは、Workfront計画権限とWorkfront アクセスレベルのコンテキストで行われます。

  詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* AI アシスタントや Planning Designerがユーザーに代わって行った変更は、レコードの履歴パネルで追跡されます。

* 計画Designerが実行したアクションは永続的であり、元に戻すことができない可能性があります。 例えば、フィールドを削除すると、元に戻すことはできません。 Designerによって提案されたすべてのアクションをレビューしてから承認します。

  >[!IMPORTANT]
  >
  >Planning Designerを使用してオブジェクトを作成、更新または削除する場合、プロンプトは元に戻せない処理に対してのみ確認を求めます。 例えば、レコードタイプやワークスペースを削除すると、元に戻せません。 レコードを削除することはできません。 レコードタイプまたはワークスペースを削除しようとすると、Planning Designerによって確認が求められます。

* 計画Designerを使用してワークスペースとレコードタイプを作成すると、ビューとフィールドも自動的に作成されます。

## 現在、PlanningDesignerで使用可能な機能

計画Designerまたは AI アシスタントを使用して、次のいずれかの操作を実行できます。

* ワークスペースの作成と設定

* グローバルレコードタイプの定義とワークスペースへの追加を含む、レコードタイプの作成

* デザイン フィールドまたは数式フィールド

* レコードの作成、削除、複製、復元

* レコードのフィールドの編集、更新、追加

* レコードを他のレコードにリンク

* レコードの変更履歴へのアクセス

* カスタムビューの作成

* ドキュメントを読み込んでレコードを作成

  例えば、会社の組織図の写真をアップロードし、それに基づいて Planning Designerでワークスペースを作成できます。

  読み込んだドキュメントからオブジェクトを作成する機能は、Planning Designerでのみ使用でき、AI アシスタントでは使用できません。

  >[!IMPORTANT]
  >
  >.XLSX および.CSV ファイルタイプはサポートされていますが、Planning Designerを使用した大規模なレコード読み込みには使用できません。
  >現時点で大量のレコードをインポートする必要がある場合は、Planning で使用できる手動機能を使用してインポートすることをお薦めします。
  >
  >詳しくは、[CSV または Excel ファイルから情報を読み込むことによるレコードの作成 &#x200B;](/help/quicksilver/planning/records/import-file-to-create-records.md) を参照してください。
  >ファイルタイプの制限については、[AI を利用したフォーム入力を使用してプロンプトやドキュメントを使用してリクエストを入力する &#x200B;](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md) の「アップロードするドキュメントに基づいて提案を取得する」の節を参照してください。


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## PlanningDesignerを使用したオブジェクトの作成または更新

特に指定がない限り、Workfront Planning Designerまたは AI アシスタントを使用して、Planning でオブジェクトを作成または更新できます。

1. Workfrontにログインし、左上隅の **メインメニュー** アイコン ![&#x200B; ラインメインメニュー &#x200B;](assets/lines-main-menu.png) をクリックして、「**計画**」をクリックします。

   **計画** エリアが開きます。<!--update screen shot when they change the name of the button-->

   ![&#x200B; ワークスペースページの「AI を使用したデザイン」ボタン &#x200B;](assets/design-with-ai-button-on-workspaces-page.png)

1. **AI で作成** をクリックします。<!--update this when they change it-->

   **計画Workspace** ウィンドウの **Designer設定** エリアが開きます。<!--replace shot below when they rename the area to Planning Designer-->

   ![&#x200B; 計画Designerウィンドウ &#x200B;](assets/planning-designer-window.png)

1. 指定されたスペースで、AI アシスタントのプロンプトの入力を開始し、完了したら [Enter] をクリックします。

   <!--add screen shot-->

   例えば、次のようなプロンプトを入力できます。

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

1. 応答が成功したら、プロンプトエリアに表示されるリンクに従って、リクエストのオブジェクトを作成、更新またはレビューします。

   オブジェクトの作成に同意すると、変更がプロンプト領域の右側に表示されます。

   プロンプトの右側のプレビュー領域で、ワークスペース、レコードタイプ、フィールド、ビュー、およびレコードを表示できます。

   >[!TIP]
   >
   >確認を行わなくても、すぐに作成されるオブジェクトもあります。

1. （オプション）オブジェクトをさらに編集するための追加プロンプトを入力します。
1. （オプション） **プレビュー画面の表示/非表示** アイコン ![&#x200B; プレビュー画面の表示/非表示アイコン &#x200B;](assets/hide-show-preview-screen-in-planning-designer.png) をクリックして、右側のプレビュー画面を開いたり閉じたりします。
1. **ワークスペースを新しいタブで開くアイコン**![&#x200B; ワークスペースを新しいタブで開くアイコン &#x200B;](assets/open-workspace-on-new-tab-icon.png) をクリックして、更新しているワークスペースを新しいタブで開きます。
1. **閉じる** アイコン **X** をクリックして、Planning Designerを閉じ、ワークスペースエリアを開きます。
1. PlanningDesignerを使用して編集したワークスペースを開き、そのオブジェクトにさらに変更を加えます。

## 組織の計画Designerをオフにする

Workfront管理者が AI アシスタント契約を承諾すると、デフォルトでは、組織内のすべてのユーザーに対してDesignerの計画が有効になります。

オフにするには：

1. システム管理者としてWorkfrontにログインします。
1. 画面の左上隅にある **メインメニュー**![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-shell.png) をクリックし、**設定** をクリックします。
1. 左側のパネルで **システム** /をクリックし、**AI 環境設定** 領域に移動します。
1. **オンボーディングの計画** 設定をオフにします。<!--add new screen shot with info icon and new name of the toggle; ensure you don't show the AI Reviewer if it is not in Prod yet-->

   ![&#x200B; システム環境設定でのDesigner設定の計画 &#x200B;](assets/planning-designer-toggle-in-system-preferences.png)
1. 「**保存**」をクリックします。

   これにより、システム内のすべてのユーザーの Planning Designerが削除されます。






