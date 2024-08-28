---
title: 「AI アシスタントの概要」
content-type: reference
description: AI アシスタントの概要
author: Becky
feature: Get Started with Workfront
source-git-commit: d261fd9eb9b8b649ebe413e35161543db1db8412
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 6%

---

# AI アシスタントの概要

>[!IMPORTANT]
>
>ワークフロントAIアシスタントは一時的に削除されましたが、後日利用できるようになります。

WorkfrontのAIアシスタントは、アプリ内の情報や提案を自然言語の会話で提供することで、作業の達成を支援します。 AIアシスタントは、次の方法でよりスムーズな作業エクスペリエンスを提供できます

* 作業項目またはドキュメントの概要
* 作業プロセスの指示または参照品目の検索
* 計算フィールドの数式の生成または確認

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在：使用できません</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：使用できません</p></td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。## AI アシスタントの前提条件

組織の AI アシスタントを有効にするには、次の **すべて** を適用する必要があります。

* 組織が Adobe Systems IMS(Identity Management System)に移行している必要があります。
* Adobe Systems Unified Experience を有効にする必要があります
* 組織には、Select、Prime、またはUltimate ワークフロントプランが必要です
* Adobe Systems署名済みのAdobe Systems Gen AI契約をファイルに提出する必要があります

  契約への署名の詳細については、この記事の [Adobe Systems Gen AI 契約に署名する](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) を参照してください。

## AI アシスタントに関する考慮事項

* AI アシスタントは、開いているページ状況依存です。 たとえば、プロジェクトの AI アシスタントに「このプロジェクトを要約」と入力すると、その特定のプロジェクトの概要ページ返されます。
* Workfront 管理者は、組織内のユーザーに対して AI Assistant を有効にする必要があります。 AI アシスタントは、アクセス レベルで有効になります。

  詳しくは、 [AI Assistant を有効または無効にする](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)を参照してください。

* ワークフロント計画 AI アシスタントには、ワークフロント AI アシスタントとは異なる機能があります。

  Adobe Workfront計画の AI アシスタントについて詳しくは、[Workfront計画 AI アシスタントの概要 ](/help/quicksilver/planning/general/planning-ai-assistant-overview.md) を参照してください。


## AI アシスタントで使用可能な機能

現在、AI アシスタントは次の機能を提供しています。

* プロジェクト、タスク、イシューまたはドキュメントの要約。

  詳細については、[AI アシスタントを使用して要約する ](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md) を参照してください。

* Adobe Experience LeagueのWorkfront ドキュメントから取得した手順や参照情報を提供する。

  詳細については、「[AI アシスタントからヘルプを表示する ](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)」を参照してください。

* 計算されたカスタム フィールドの数式を生成または調整します。

  >[!NOTE]
  >
  >この機能は、Prime または Ultimate Workfront プランを利用している組織のみが利用できます。

  詳細については、[AI アシスタントを使用して計算フィールドの数式を生成または変更する ](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md) を参照してください。

## AI アシスタントにアクセス

1. ワークフロント ページの上部にある AI アシスタント アイコン ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)をクリックします。
1. 画面の右側のパネルに質問またはプロンプト書式 ＜例外＞Photoshop のみ「テキスト」します。

   このパネルに入力できない場合、組織は署名済みの Adobe Systems Gen AI 契約を登録していません。

1. AI アシスタントが必要な～に回答を提供しない場合は、プロンプトを調整して再試行してください。

## Adobe Systems 世代 AI 契約に署名する

組織が署名済みのAdobe生成 AI 契約をファイルで持っていない場合、組織に対して AI アシスタントを有効にすることはできません。

Adobe生成 AI 契約に署名されていないときに、ユーザーが AI アシスタントを使用しようとすると、次のメッセージが表示されます。

* ユーザー：ユーザーは、AI アシスタントが組織で有効になっていないことと、Workfront管理者に連絡して組織で AI アシスタントをリクエストできることを知らされます。
* 管理者：署名済みのAdobe生成 AI 契約がないことを知らされ、契約のコピーを署名用に送信するようリクエストできます。

Adobe生成 AI 契約をリクエストするには：

1. Workfront管理者は、「AI アシスタント」アイコンをクリック ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) ます。
1. AI アシスタント パネルで入力を開始します。
1. Adobe生成 AI 契約メッセージが表示されたら、「**契約を確認**」をクリックします。
1. Adobe生成 AI 契約に署名する組織内の個人の名前とメールアドレスを入力します。

   契約書はこのユーザーに送信され、署名が行われます。 署名して返されると、組織で AI アシスタントが有効になります。

