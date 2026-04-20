---
title: Workfront の AI アシスタント
content-type: reference
description: Adobe Workfront の AI アシスタントについて
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 97%

---

# Workfront の AI アシスタント

Workfront の AI アシスタントは、アプリ内の情報やおすすめを自然言語で提供し、作業の遂行を支援します。AI アシスタントを使用すると、次の操作をよりスムーズに行うことができます。

* 作業アイテムまたはドキュメントの要約
* 作業プロセスの指示または参考資料の検索
* 計算フィールドの数式の生成や確認

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>Select以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## AI アシスタントの前提条件

組織の AI アシスタントを有効にするには、次の&#x200B;**すべて**&#x200B;の条件を満たす必要があります。

<!--Remove me October 2026-->

* 組織が Adobe IMS（ID 管理システム）に移行している必要があります。
* Adobe Unified Experience を有効にする必要があります。
* 組織が Select、Prime、または Ultimate の Workfront プランを導入している必要があります。
* アドビが署名済みの Adobe 生成 AI 契約を保存している必要があります。

  契約の署名について詳しくは、この記事の [Adobe 生成 AI 契約への署名](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)を参照してください。

## AI アシスタントに関する考慮事項

* AI アシスタントは、開いているページに応じてコンテキストを認識します。例えば、プロジェクトページで AI アシスタントに「このプロジェクトを要約する」と入力すると、その特定のプロジェクトの概要が返されます。
* Workfront 管理者は、組織内のユーザーに対して AI アシスタントを有効にする必要があります。AI アシスタントはアクセスレベルで有効になります。

  詳しくは、[AI アシスタントの有効化または無効化](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)を参照してください。

* Workfront Planning の AI アシスタントには、Workfront の AI アシスタントとは異なる機能があります。

  Workfront Planning の AI アシスタントについて詳しくは、[Adobe Workfront Planning の AI アシスタントの概要](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)を参照してください。

* AI アシスタントは現在、英語でのみ利用できます。


## AI アシスタントで利用可能な機能

現在、AI アシスタントでは次の機能が提供されています。

* プロジェクト、タスク、イシューまたはドキュメントを要約する。

  詳細については、[AI アシスタントを使用した要約](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)を参照してください。

* Adobe Experience League に関する Workfront ドキュメントから取得した手順や参照情報を提供する。

  詳しくは、[AI アシスタントの利用](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)を参照してください。

* Workfront 内の特定のアイテムを検索する。

  詳しくは、[AI アシスタントを使用した、プロジェクト、タスクおよびイシューの作業](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md)を参照してください。

* 計算カスタムフィールドの数式を生成または調整する。

  >[!NOTE]
  >
  >この機能は、Workfront プランの Prime または Ultimate を利用している組織のみが使用できます。

  詳しくは、[AI アシスタントを使用した計算フィールド数式の生成または修正](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md)を参照してください。

* プロジェクトに関する更新、アップロードされたドキュメント、その他の注目すべき変更を優先度別に 24 時間、3 日、7 日間の期間でまとめます。

詳しくは、[優先度での作業の遅れの取り戻し](/help/quicksilver/workfront-basics/priorities/catch-me-up.md)を参照してください。


## AI アシスタントで利用可能なオブジェクトタイプ

ユーザーが Workfront で有効な権限を持っている場合、AI アシスタントは次のオブジェクトタイプに関連付けられたデータをクエリできます。

* ポートフォリオ
* プログラム
* プロジェクト
* タスク
* イシュー
* カスタムフォーム
* ユーザー
* Adobe Workfront Planning のレコード


## AI アシスタントへのアクセス

1. Workfront ページの上部で、AI アシスタントアイコン ![AI アシスタントアイコン](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) をクリックします。
1. 質問を入力するか、画面の右側にあるパネルにプロンプトを表示します。

   このパネルに入力できない場合は、組織が Adobe 生成 AI 契約に署名していないことを示します。

1. AI アシスタントから必要な回答が提供されない場合は、プロンプトを調整して再試行してください。

## Adobe 生成 AI 契約への署名

組織が Adobe 生成 AI 契約に署名していない場合、組織に対して AI アシスタントを有効にすることはできません。

Adobe 生成 AI 契約が署名されていない場合、ユーザーが AI アシスタントを使用しようとすると、次のメッセージが表示されます。

* ユーザー：ユーザーは、AI アシスタントが組織で有効になっていないこと、および Workfront 管理者に連絡し、AI アシスタントをリクエストできることが通知されます。
* 管理者：Adobe 生成 AI 契約に署名していないこと、および署名する契約書のコピーを送信するようリクエストできることが通知されます。

Adobe 生成 AI 契約をリクエストするには：

1. Workfront 管理者は、AI アシスタントアイコン ![AI アシスタントアイコン](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) をクリックします。
1. AI アシスタントパネルで入力を開始します。
1. Adobe 生成 AI 契約メッセージが表示されたら、「**契約をレビュー**」をクリックします。
1. Adobe 生成 AI 契約に署名する組織の担当者の名前とメールアドレスを入力します。

   署名する契約書が担当者に送信されます。署名済み契約書を返送後、アドビが内容を確認すると、組織に対して AI アシスタントが有効になります。

   >[!NOTE]
   >
   >* 署名済み契約書を返送後、アドビが内容を確認し、AI アシスタントを有効にするまで 1～3 営業日かかります。
   >* 有効にした後、組織のインスタンスで利用可能なAI アシスタントのオプションが表示されない場合は、Workfront カスタマーサポートにお問い合わせください。

## AI アシスタントでプロンプトを作成する際のヒント

プロンプトに次のキーワードを使用して、コンテキストを提供し、AI アシスタントが正しい情報を見つけられるようにします。キーワードは大文字と小文字を区別しません。

プロンプトを入力する場合は、`using (keyword)` というフレーズを含めます。

| キーワード | エフェクト |
| --- | --- |
| `workfront` | Workfront とやり取りしてください。 |
| `planning` | Workfront Planning とやり取りしてください。 |
| `help` | Experience League ドキュメントからの情報を返してください。 |
| `formula` | Planning、設定、またはカスタムフォームで使用する数式をチェックして返してください。 |
| `health` | プロジェクトのヘルスアドバイザーでプロジェクトの正常性を確認してください。 |
| `summarize` | ファイルをアップロードしたり、プロジェクトを要約したりするときなど、アイテムを要約してください。 |

>[!NOTE]
>
> すべてのエリアですべてのキーワードを使用できるわけではありません。
>
>* `formula` キーワードは、Planning、設定およびカスタムフォームビルダーでのみ使用できます。
>* `planning` キーワードは、Workfront Planning からのみ使用できます。





