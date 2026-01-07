---
title: Workfrontの AI アシスタント
content-type: reference
description: Adobe Workfront の AI アシスタントについて
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 7%

---

# Workfrontの AI アシスタント

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

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## AI アシスタントの前提条件

組織の AI アシスタントを有効にするには、次の **すべて** を適用する必要があります。

* 組織がAdobe IMS（Identity Management System）に移行している必要があります
* Adobe統合エクスペリエンスを有効にする必要があります
* 組織には Select、Prime、UltimateのいずれかのWorkfront プランが必要です
* Adobeは、ファイルにAdobe生成 AI 契約を署名済みにする必要があります

  契約の署名について詳しくは、この記事の [Adobe生成 AI 契約への署名 &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) を参照してください。

## AI アシスタントに関する考慮事項

* AI アシスタントは、開いているページのコンテキストに依存します。 例えば、プロジェクトページで「このプロジェクトを要約」を AI アシスタントに入力すると、その特定のプロジェクトの概要が返されます。
* Workfront管理者は、組織内のユーザーに対して AI アシスタントを有効にする必要があります。 AI アシスタントはアクセスレベルで有効になります。

  詳しくは、[AI アシスタントを有効または無効にする &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

* Workfront Planning AI Assistant には、Workfront AI Assistant とは異なる機能があります。

  Adobe Workfront計画の AI アシスタントについて詳しくは、[Workfront計画 AI アシスタントの概要 &#x200B;](/help/quicksilver/planning/general/planning-ai-assistant-overview.md) を参照してください。

* AI アシスタントは現在、英語でのみ利用できます。


## AI アシスタントで使用可能な機能

現在、AI アシスタントは次の機能を提供しています。

* プロジェクト、タスク、イシューまたはドキュメントの要約。

  詳細については、[AI アシスタントを使用して要約する &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md) を参照してください。

* Adobe Experience League に関するWorkfront ドキュメントから取得した手順や参照情報を提供する。

  詳細については、「[AI アシスタントからヘルプを表示する &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)」を参照してください。

* Workfront内の特定の項目を検索する。

  詳しくは、[AI アシスタントを使用して、プロジェクト、タスク、問題を操作する &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md) を参照してください。

* 計算されたカスタム フィールドの数式を生成または調整しています。

  >[!NOTE]
  >
  >この機能は、PrimeまたはUltimate Workfront プランを利用している組織のみが使用できます。

  詳細については、[AI アシスタントを使用して計算フィールドの数式を生成または変更する &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md) を参照してください。

* プロジェクトに関する更新、アップロードされたドキュメント、その他の注目すべき変更を優先度の 24 時間、3 日、7 日間の期間内にまとめます。

詳しくは、[&#x200B; 優先度の作業のキャッチアップ &#x200B;](/help/quicksilver/workfront-basics/priorities/catch-me-up.md) を参照してください。


## AI アシスタントで使用可能なオブジェクトタイプ

ユーザーがWorkfrontで有効な権限を持っている場合、AI アシスタントは次のオブジェクトタイプに関連付けられたデータをクエリできます。

* ポートフォリオ
* プログラム
* プロジェクト
* タスク
* イシュー
* カスタムフォーム
* ユーザー
* Workfront計画レコード


## AI アシスタントへのアクセス

1. Workfront ページの上部で、「AI アシスタント」アイコン ![AI アシスタントのアイコン &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) をクリックします。
1. 質問を入力するか、画面の右側にあるパネルにプロンプトを表示します。

   このパネルに入力できない場合は、署名済みのAdobe Gen AI 契約がファイルにありません。

1. AI アシスタントが必要な回答を提供しない場合は、プロンプトを調整して再試行してください。

## Adobe Gen AI 契約に署名

組織が署名済みのAdobe Gen AI 契約をファイルで持っていない場合、組織に対して AI アシスタントを有効にすることはできません。

Adobe生成 AI 契約に署名されていないときに、ユーザーが AI アシスタントを使用しようとすると、次のメッセージが表示されます。

* ユーザー：ユーザーは、AI アシスタントが組織で有効になっていないことと、Workfront管理者に連絡して組織で AI アシスタントをリクエストできることを知らされます。
* 管理者：署名済みのAdobe Gen AI 契約がないことを知らされ、契約のコピーを署名用に送信するようリクエストできます。

Adobe生成 AI 契約をリクエストするには：

1. Workfrontの管理者は、「AI アシスタント」アイコン ![AI アシスタントのアイコン &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) をクリックします。
1. AI アシスタント パネルで入力を開始します。
1. Adobe生成 AI 契約メッセージが表示されたら、「**契約を確認**」をクリックします。
1. Adobe Gen AI 契約に署名する組織内の個人の名前とメールアドレスを入力します。

   契約書はこのユーザーに送信され、署名が行われます。 署名して返された後、Adobeが契約書を確認し、組織に対して AI アシスタントが有効になります。

   >[!NOTE]
   >
   >Adobeが AI アシスタントを確認して有効にするには、契約書に署名して返してから 1 ～ 3 営業日かかります。

## AI アシスタントでプロンプトを作成するためのヒント

プロンプトで次のキーワードを使用して、コンテキストを提供し、正しい情報を見つけるのに役立てます。 キーワードでは大文字と小文字が区別されません。

プロンプトを入力する場合は、`using (keyword)` というフレーズを含めます。

| キーワード | 効果 |
|---|---|
| `workfront` | Workfrontとやり取りする。 |
| `planning` | Workfrontの計画とやり取りする。 |
| `help` | Experience League ドキュメントからの情報を返します。 |
| `formula` | Planning、設定またはカスタム・フォームで使用する式をチェックして戻します。 |
| `health` | プロジェクト正常性アドバイザーでプロジェクトの正常性を確認します。 |
| `summarize` | ファイルのアップロード時やプロジェクトの要約時などに、項目の概要が表示されます。 |

>[!NOTE]
>
> すべてのエリアですべてのキーワードを使用できるわけではありません。
>
>* `formula` キーワードは、Planning、設定およびカスタム フォーム ビルダーでのみ使用できます。
>* `planning` キーワードは、Workfront Planning からのみ使用できます。





