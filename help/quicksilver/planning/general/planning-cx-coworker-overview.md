---
title: Adobe Workfront計画CX Enterprise Coworkerの概要
description: Workfront PlanningでCX Enterprise Coworkerを使用すると、通常インターフェイスで実行するPlanningのレコードや他のオブジェクトと同様のアクションを実行できます。 ユーザーのコマンドとAIによるコマンドの実行が連携して、AIによる変更が環境に正確に反映されるようにします。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 2b2e58c17bdcb7c28b11bf460bad24bc1e1eb642
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 9%
---

# Adobe Workfront計画CX Enterprise Coworkerの概要

<!--replaced information from the AI Assistant for Planning article with CX Enterprise Coworker-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 リリースからプレビューの後、高速リリースを有効にしたお客様は、同じ機能を毎月実稼動環境でも使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

CX Enterprise Coworkerは対話型のインターフェイスです。目的を平易な言葉で説明し、Workfront計画やその他の接続されたAdobeシステムをまたいで作業を計画、実行、検証してから、承認用に戻します。

Adobe Workfrontは、AI アシスタントのあらゆる機能を保持しながら、新しいフルスクリーン体験とWorkfrontの右側のパネルの両方に、より強力なエンドツーエンドの機能を追加しています。

組織の既存の製品レベルのアクセス制御内で動作するため、ユーザーはWorkfrontで既に許可されているアクションのみを実行でき、デフォルトでは読み取り専用アクセスが使用され、Workfront管理者は書き込みアクセスを制御できます。

>[!IMPORTANT]
>
>Coworkerは現在、ヘルスケア、金融、その他の機密データを扱う業界の組織には利用できません。 AI アシスタントは、これらの組織で利用できます。
>
>詳しくは、[AI アシスタントの概要](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)を参照してください。


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
  <p>管理者は、Planningの同僚へのアクセスを許可するために、次の操作を行う必要があります。</p>
   <ul>
   <li><p>ワークフローとプランニングパッケージの両方を持っている場合は、ワークフローとプランニングライセンスタイプの両方をアクセスレベルに追加します</p></li>
  <li><p>アクセスレベルの「Workfrontで同僚パネルを無効にする」設定の選択を解除します。 デフォルトで選択されています。</p></li></ul>
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## 共同作業者に関する考慮事項

* 会社のユーザーが利用できるようにするには、組織で共同作業者を有効にする必要があります。

  詳しくは、[CX Enterprise Coworkerの概要](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)を参照してください。

* WorkfrontでWorkfront インスタンスのエージェントを有効にすると、メインのWorkfront管理者がエージェントを有効にでき、組織に対してエージェントを有効にすることができます。 詳しくは、[ システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

* Workfront管理者は、アクセスレベルでCoworkerを有効にする必要があります。 詳しくは、[ アクセスレベルの作成と変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* 共同作業者は、WorkfrontまたはWorkfront Planningにあり、アクセス権を持つ情報とオブジェクトを操作します。 プランニングの右側パネルで、共同作業者パネルは、開いているワークスペース、レコードタイプ、またはレコードページのコンテキストで動作します。

* プランニング領域で共同作業者が実行するアクションは、Workfrontプランニング権限とWorkfrontアクセスレベルのコンテキストにあります。 詳しくは、次の記事を参照してください。

  * [Adobe Workfront プランニングでの共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Adobe Workfront プランニング使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* ユーザーに代わって同僚が行った変更は、レコードの履歴パネルで追跡されます。

* 同僚が行ったアクションは永続的であり、元に戻せない可能性があります。 例えば、フィールドの削除を元に戻すことはできません。 承認する前に、同僚が提案したすべてのアクションを確認してください。

* Coworkerを通じてオブジェクトを作成、更新、または削除する場合、Coworkerは意図されたアクションを表示し、確認を求めます。 その後、アクションを確認またはキャンセルできます。

## Coworkerで現在利用可能な機能

現在、CoworkerはWorkfrontのプランニング エリアで利用でき、プランニング オブジェクトの情報にアクセスして操作するための一連のスキルを使用します。 詳しくは、[CX Enterprise Coworker スキル ](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md)を参照してください。

Coworkerを使用して、次のアクションを実行できます。

* レコードの検索： 任意のレコードフィールドに含まれる情報で検索できます。
* レコードを作成します。 新しいレコードへのリンクを含むIDは、レコードの作成後に表示されます。 日付や説明など、作成プロセス中に更新するフィールドを指定できます。
* アップロードしたドキュメントに基づいてレコードを作成します。 Workfrontでは、次のドキュメントフォーマットをサポートしています。

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT、およびほとんどの画像フォーマット
* 画面に表示されるレコードのフィールドを更新する
* レコードの削除、複製、復元
* レコードを他のレコードにリンク
* レコードの変更履歴の表示


## Workfront Planningで「同僚」を探す

Coworkerは、Workfront Planningの次の領域で見つけることができます。

* 画面の右上隅にあるメインナビゲーションバー。
* 新しいタブでレコードを開いたときに、レコードの詳細エリア内に表示されます。

## プランニング エリアの同僚へのアクセス

1. Workfrontにログインし、左上隅の&#x200B;**メインメニュー** アイコン ![行メインメニュー](assets/lines-main-menu.png)をクリックしてから、**計画**&#x200B;をクリックします。

   計画領域が開きます。

   ページの右上隅にある&#x200B;**Coworker** アイコン ![Coworker アイコン ](assets/coworker-icon.png)を見つけるか、以下の手順に進みます。

1. **ワークスペースカード**&#x200B;をクリックします。

1. **レコードタイプカード**&#x200B;をクリックします。

1. **レコード**&#x200B;をクリックしてレコードの&#x200B;**詳細** ページを開き、**新しいタブで開く** アイコン ![新しいタブで開く](assets/open-workspace-on-new-tab-icon.png)をクリックします。

1. 画面の右上隅にある&#x200B;**同僚アイコン** ![同僚アイコン ](assets/coworker-icon.png)をクリックします。

1. 提供されたスペースで、Coworkerのコマンドを入力し始め、完了したら「Enter」をクリックします。

   空のコマンドボックスを持つ![同僚パネル ](assets/cx-coworker-right-rail.png)

   例えば、次のいずれかを入力します。

   * 「Summer Sale 2026」という新しいキャンペーンレコードを作成します
   * サマーキャンペーンのレコードの予算フィールドを$75,000に更新します
   * Old Promoという名前のキャンペーンレコードを削除します
   * 誤って削除したキャンペーンを復元する

   >[!TIP]
   >
   >Coworkerにオブジェクトに対する編集アクションの実行を依頼する前に、システム環境設定でWorkfront管理者が書き込み専用のMCP ツールを有効にしていることを確認してください。

   Coworkerがコマンドを処理する際に、応答時間の期待値を設定する視覚的なインジケーターが表示されます。

   応答が成功した後、提供されたリンクに従うか、左側の変更に注意してください。


1. （オプション）「**フルスクリーンを展開**」アイコン「![ フルスクリーンアイコン「](assets/expand-full-screen-icon.png)」をクリックすると、フルブラウザータブで同僚のチャットボックスが開きます。


