---
title: Adobe Workfront計画CX Coworkerの概要
description: Workfront PlanningのCX Coworkerを使用すると、通常インターフェイスで実行するPlanningのレコードや他のオブジェクトと同様のアクションを実行できます。 ユーザーのコマンドとAIによるコマンドの実行が連携して、AIによる変更が環境に正確に反映されるようにします。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: d5f36e0c8dbd9749503de25b75e70bf18b1d187b
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 11%
---

# Adobe Workfront計画CX Coworkerの概要


<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 リリースからプレビューの後、高速リリースを有効にしたお客様は、同じ機能を毎月実稼動環境でも使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

CX Coworkerは、目標を平易な言葉で説明し、Adobeと接続されたシステムをまたいで作業を計画、実行、検証し、承認のために返す会話型のインターフェイスです。

CX Coworkerは、現在のAI アシスタントの機能をすべて保持しながら、新しいフルスクリーン体験とWorkfrontの右側のパネルの両方に、より強力なエンドツーエンドの機能を追加しています。

組織の既存の製品レベルのアクセス制御内で動作するため、ユーザーはWorkfrontで既に許可されているアクションのみを実行でき、デフォルトでは読み取り専用アクセスが使用され、Workfront管理者は書き込みアクセスを制御できます。

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
<p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p>
または
<p>スタンドアロン製品として購入された場合の任意のプランニング・パッケージ</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td>  
   <p>PlanningでCX Coworkerへのアクセスを許可するには、管理者が次の操作を行う必要があります。</p>
   <ul>
   <li><p>ワークフローとプランニングパッケージの両方を持っている場合は、ワークフローとプランニングライセンスタイプの両方をアクセスレベルに追加します</p></li>
   <li><p>アクセスレベルの「WorkfrontでCX Coworker パネルを無効にする」設定の選択を解除します。 デフォルトで選択されています。</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>システム設定</p></td> 
   <td>   <p>Workfront管理者は、設定の「システム環境設定」セクションで「読み取り専用」および「書き込み専用」のMCP ツールを選択する必要があります。 デフォルトでは、「読み取り専用」 MCP ツールが選択されています。</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++


## CX Coworkerの考慮事項

* CX Coworkerは、社内のユーザーが利用できるようにする前に、自社に対して有効にする必要があります。

  詳しくは、[CX Coworkerの概要](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)を参照してください。

* Workfrontが組織のエージェントを有効にした後、メインのWorkfront管理者が使用できるようになります。 詳しくは、[システムの基本情報を設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。

* Workfront管理者は、他のすべてのユーザーに対してAI アシスタントを有効にする必要があります。 詳しくは、[AI アシスタントの有効化または無効化](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)を参照してください。

* AI アシスタントは、各ページのコンテキストで動作します。 AI アシスタントに対して送信するリクエストは、開いているページで使用可能な機能を参照する必要があります。

* 計画領域でAI アシスタントによって実行されるアクションは、Workfront計画の権限とWorkfront アクセスレベルのコンテキストにあります。 詳しくは、次の記事を参照してください。

  * [Adobe Workfront プランニングでの共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Adobe Workfront プランニング使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* ユーザーに代わってAI アシスタントが行った変更は、レコードの履歴パネルで追跡されます。

* AI アシスタントによるアクションは永続的であり、元に戻せない可能性があります。 例えば、フィールドの削除を元に戻すことはできません。 AI アシスタントが提案したすべてのアクションを承認する前に確認します。

* AI アシスタントを通じてオブジェクトを作成、更新、削除する場合、AI アシスタントは意図されたアクションを表示し、確認を求めます。 その後、アクションを確認またはキャンセルできます。

## AI アシスタントで現在利用可能な機能

現在、AI アシスタントはWorkfrontの計画領域で次のページで利用できます。

* Workspace page
* レコードタイプページ
* レコードページ

現時点では、AI アシスタントを使用して次のアクションを実行できます。

* レコードの検索： 任意のレコードフィールドに含まれる情報で検索できます。
* レコードを作成します。 新しいレコードへのリンクを含むIDは、レコードの作成後に表示されます。 日付や説明など、作成プロセス中に更新するフィールドを指定できます。
* アップロードしたドキュメントに基づいてレコードを作成します。 Workfrontは、AI アシスタントで次のドキュメントフォーマットをサポートしています。

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT、およびほとんどの画像フォーマット
* 画面に表示されるレコードのフィールドを更新する
* レコードの削除
* 削除したレコードを復元


## Workfront PlanningのAI アシスタントを探す

AI アシスタントは、Workfront Planningの次の領域で見つけることができます。

* 画面の右上隅にあるメインナビゲーションバー。
* レコードの詳細領域内で、プレビューでレコードを開いた後、またはレコードのページを開いた後。

## 計画領域のAI アシスタントにアクセスします

1. Workfrontにログインし、左上隅の&#x200B;**メインメニュー** アイコン ![行メインメニュー](assets/lines-main-menu.png)をクリックしてから、**計画**&#x200B;をクリックします。

   計画領域が開きます。

1. **ワークスペースカード**&#x200B;をクリックします。

1. （オプション） **レコードタイプカード**&#x200B;をクリックします。

1. （オプション） **レコード**&#x200B;をクリックして、レコードの&#x200B;**詳細** ページを開きます。

1. グローバルナビゲーションバーの画面の右上隅、またはレコードのプレビューまたはページの右上隅にある&#x200B;**AI アシスタントアイコン**&#x200B;をクリックします。

   ![AI アシスタント アイコン &#x200B;](assets/ai-assistant-icon-highlighted.png)

1. 提供されたスペースで、AI アシスタントのコマンドを入力し始め、完了したら「Enter」をクリックします。

   ![空のコマンドボックスを含むAI アシスタントパネル &#x200B;](assets/ai-assistant-panel-with-empty-command-box.png)

   例えば、次のいずれかを入力します。

   * 開始日が7月4日で終了日が7月30日のキャンペーンを作成します
   * 日付が決定されるサマーキャンペーンレコードの「説明」フィールドを更新します
   * 最後のレコードを削除
   * レコードの復元

   AI アシスタントがコマンドを処理する間、視覚的なインジケーターが表示され、応答時間に対する期待値が設定されます。

   応答が成功した後、提供されたリンクに従うか、左側の変更に注意してください。



