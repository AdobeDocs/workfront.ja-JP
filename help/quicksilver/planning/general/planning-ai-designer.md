---
title: Adobe Workfront Planning Designerの基本を学ぶ
description: Adobe Planning Designerを使用すると、新しい作業領域を作成したり、Workfront Planning のレコード・タイプとフィールドを使用して新規作業領域を作成したり、作業領域にオブジェクトを追加したり、レコードの変更履歴を表示したりできます。
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 6%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Adobe Workfront Planning Designerの基本を学ぶ

{{planning-important-intro}}

AI を活用したAdobe計画Designerを使用して、新しいワークスペースを生成したり、ワークスペースにオブジェクト（レコードタイプ、レコード、ビュー、フィールド）を追加したり、レコードの変更履歴を表示したりできます。

>[!IMPORTANT]
>
>Planning Designerは現在、クローズドBetaプログラムに参加しているユーザーのみが利用できます。

Workfrontの計画について詳しくは、次の記事を参照してください。

* [Adobe Workfrontの計画に関する一般情報](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfrontの計画の概要](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning のアクセスの概要](/help/quicksilver/planning/access/access-overview.md)


## アクセス要件

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

* Planning Designerを使用するには、Workfront AI アシスタントを使用するための要件を満たす必要があります。

  詳しくは、[AI アシスタントの前提条件 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) を参照してください。

* Planning Designerを使用するには、システム管理者が設定の「システム環境設定」領域で有効にする必要があります。

* プロンプトを使用して、計画領域からWorkfront AI アシスタントを使用するか、または計画Designerを使用して、計画オブジェクトを作成できます。

* 計画領域で AI アシスタントが実行するアクションや、計画Designerが実行するアクションは、Workfront計画権限とWorkfront アクセスレベルのコンテキストで行われます。

  詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* ユーザーに代わって Planning Designerが行った変更は、レコードの履歴パネルで追跡されます。

* コマンドを使用してアクションを取り消すことができます。 例えば、「最後の変更を取り消す」と入力して、変更を元に戻すことができます。

* Planning Designerを使用してオブジェクトを作成、更新または削除する際に、意図したアクションが表示され、確認を求められます。 その後、アクションを確認またはキャンセルできます。

* 計画Designerを使用してワークスペースとレコードタイプを作成すると、ビューとフィールドも自動的に作成されます。

## 現在、PlanningDesignerで使用可能な機能

計画Designerまたは AI アシスタントを使用して、次のいずれかの操作を実行できます。

* ワークスペースの作成と設定

* レコードタイプの作成

* デザイン フィールドまたは数式フィールド

* レコードの作成、削除、複製、復元

* レコードのフィールドの編集、更新、追加

* レコードを他のレコードにリンク

* レコードの変更履歴へのアクセス

* カスタムビューの作成

* ドキュメントを読み込んでレコードを作成します。

  読み込んだドキュメントからレコードを作成する機能は、Planning Designerでのみ使用でき、AI アシスタントでは使用できません。

  使用できるファイルのタイプとサイズについては、記事 [AI を使用したフォーム入力を使用して、プロンプトやドキュメントを使用してリクエストを入力 ](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md) の「ドキュメントガードレール」の節を参照してください。

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 組織の計画Designerを有効にする

Workfront管理者は、最初に組織の Planning Designerを有効にする必要があります。

<!--add steps here-->

1. システム管理者としてWorkfrontにログインします。
1. 画面の左上隅にある **メインメニュー**![ メインメニューアイコン ](assets/main-menu-shell.png) をクリックし、**設定** をクリックします。
1. 左側のパネルで **システム** /をクリックし、**AI 環境設定** 領域に移動します。
1. 次の設定をオンにします。
   * **AI を有効にする**
   * **AI ベータ版のオプトイン**
   * **Designerの計画**

   ![ システム環境設定でのDesigner設定の計画 ](assets/planning-designer-toggle-in-system-preferences.png)
1. 「**保存**」をクリックします。

   システム内で Standard ライセンスを持つすべてのユーザーは、計画領域のワークスペース メインページの **AI を使用したデザイン** ボタンを表示できるようになりました。<!--check screen shot-->

   ![ ワークスペースページの「AI を使用したデザイン」ボタン ](assets/design-with-ai-button-on-workspaces-page.png)

   これで、すべてのユーザーが Planning Designerを開始および使用して、Workfront Planning オブジェクトを作成および更新できます。

## PlanningDesignerを使用したオブジェクトの作成または更新

特に指定がない限り、Workfront Planning Designerまたは AI アシスタントを使用して、Planning でオブジェクトを作成または更新できます。

1. Workfrontにログインし、左上隅の **メインメニュー** アイコン ![ ラインメインメニュー ](assets/lines-main-menu.png) をクリックします。

1. **計画** をクリックします。 計画エリアが開きます。

1. **AI でデザイン** をクリックします。

   **計画Designer** ウィンドウが開きます。

   ![ 計画Designerウィンドウ ](assets/planning-designer-window.png)

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

1. 応答が成功したら、プロンプトエリアに表示されるリンクに従って、リクエストのオブジェクトを作成、更新またはレビューします。

   オブジェクトの作成に同意すると、変更がプロンプト領域の右側に表示されます。

   プロンプトの右側のプレビュー領域で、ワークスペース、レコードタイプ、フィールド、ビュー、およびレコードを確認できます。
1. （オプション）オブジェクトをさらに編集するための追加プロンプトを入力します。
1. （オプション） **AI Workspace プレビュー画面を切り替える** アイコン ![ プレビュー画面を非表示または表示アイコン ](assets/hide-show-preview-screen-in-planning-designer.png) をクリックして、右側のプレビュー画面を開いたり閉じたりします。
1. **ワークスペースを新しいタブで開くアイコン**![ ワークスペースを新しいタブで開くアイコン ](assets/open-workspace-on-new-tab-icon.png) をクリックして、更新しているワークスペースを新しいタブで開きます。
1. **閉じる** アイコン **X** をクリックして、Planning Designerを閉じ、ワークスペースエリアを開きます。
1. PlanningDesignerを使用して編集したワークスペースを開き、そのオブジェクトにさらに変更を加えます。




