---
title: 'AI アシスタントの概要'
content-type: reference
description: AI アシスタントの概要
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 1517f7480bbe481bc918876441d1b70b09963a97
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 6%

---

# AI アシスタントの概要

>[!IMPORTANT]
>
>Workfront AI アシスタントは一時的に削除されており、後日利用できるようになります。

Workfrontの AI アシスタントを使用すると、アプリ内の情報やおすすめを自然言語で提供できるので、作業を遂行できます。 AI アシスタントを使用すると、次の操作をよりスムーズに行うことができます

* 作業項目またはドキュメントの要約
* 作業プロセスの指示または参照資料の検索
* 計算フィールドの数式を生成または確認する

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

* 組織がAdobe IMS（Identity Management System）に移行している必要があります
* Adobe統合エクスペリエンスを有効にする必要があります
* 組織には Select、Prime または Ultimate Workfront プランが必要です
* Adobeは、ファイルに署名済みのAdobe生成 AI 契約が必要

  契約の署名について詳しくは、この記事の [Adobe生成 AI 契約への署名 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) を参照してください。

## AI アシスタントに関する考慮事項

* AI アシスタントは、開いているページのコンテキストに依存します。 例えば、プロジェクトページで「このプロジェクトを要約」を AI アシスタントに入力すると、その特定のプロジェクトの概要が返されます。
* Workfront管理者は、組織内のユーザーに対して AI アシスタントを有効にする必要があります。 AI アシスタントはアクセスレベルで有効になります。

  詳しくは、[AI アシスタントを有効または無効にする ](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

* Workfront Planning AI Assistant には、Workfront AI Assistant とは異なる機能があります。

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

1. Workfrontページの上部にある AI アシスタント アイコン ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) をクリックします。
1. 質問を入力するか、画面の右側にあるパネルにプロンプトを表示します。

   このパネルに入力できない場合は、署名済みのAdobe生成 AI 契約がファイルにありません。

1. AI アシスタントが必要な回答を提供しない場合は、プロンプトを調整して再試行してください。

## Adobe生成 AI 契約に署名

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

