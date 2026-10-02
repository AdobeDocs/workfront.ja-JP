---
user-type: administrator
product-area: system-administration;setup
title: カスタムローカライズの設定
description: カスタムローカライゼーションを使用すると、様々な言語でカスタム用語やフレーズを定義できます。 次に、Workfrontでは、これらの用語がブラウザー設定で設定された言語で表示されます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 18%
---
# カスタムローカライゼーションの設定

{{highlighted-preview}}

カスタムローカライゼーションを使用すると、<span class="preview">はAI</span>を使用して、様々な言語でカスタム用語とフレーズを定義できます。 次に、Workfrontでは、ユーザーのAdobe Identity Management（IMS）設定で設定された言語でこれらの用語が表示されます。

例えば、「Target Audience」というラベルは、ドイツ語の「Zielgruppe」にローカライズできます。 ブラウザーの主要言語としてドイツ語を選択したユーザーは、「Zielgruppe」という単語を英語の「Target Audience」というラベルが付いたフィールドのラベルとして見ることができます。

複数の言語への翻訳を設定できます。 現在利用可能な言語は次のとおりです。

* 中国語（繁体字）
* 中国語（簡体字）
* フランス語
* ドイツ語
* イタリア語
* 日本語
* 韓国語
* ポルトガル語 （ブラジル）
* スペイン語

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>Workflow Prime以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>翻訳を設定するには、Workfront管理者である必要があります。</p>  </td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ローカライゼーションの設定時の考慮事項

ローカライゼーションを設定する際には、次の点を考慮してください。

* 複数の言語に翻訳する用語を設定できます。
* ローカライズは、カスタムフィールドラベル（列ヘッダーとして使用する場合を含む）とツールヒントに適用されます。
* カスタムローカライズは、ビジネスルールから生成されたメッセージに適用できますが、ビジネスルールで有効にする必要があります。

  手順については、「[&#x200B; ビジネスルールでローカライゼーションを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules)」を参照してください。

## 翻訳の設定

翻訳は設定領域で設定されます。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. セットアップ領域で、左側のナビゲーションパネルの&#x200B;**ローカライゼーション**&#x200B;をクリックします。
1. 新しい翻訳を追加するには、**新しい行**&#x200B;をクリックします。
1. **英語**&#x200B;列に、翻訳する英語用語を入力します。
1. 用語を翻訳する言語の列で、ターゲット言語に用語を入力します。
1. （オプション）単語を追加の言語に翻訳するには、翻訳を適切な言語列に追加します。
1. （オプション）言語列を並べ替えるには、移動する列のヘッダーをクリックし、目的の場所にドラッグします。
1. （オプション）用語の翻訳を削除するには、用語の横にあるチェックボックスをクリックし、ページ下部の青いバーの&#x200B;**削除**&#x200B;をクリックします。

<div class="preview">

## AIによる翻訳を使用して未翻訳のカスタムテキストをローカライズ

AIを活用してカスタムテキストをローカライズすることもできます。 用語と言語を選択し、翻訳を適用する前に承認することができます。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. セットアップ領域で、左側のナビゲーションパネルの&#x200B;**ローカライゼーション**&#x200B;をクリックします。
1. ローカライゼーション領域で、「**未翻訳のカスタムテキスト**」タブを選択します。

   未翻訳のカスタムテキストのリストが表示されます。 これには、フィールドラベルやカスタムルールメッセージなどのテキストが含まれます。

1. ローカライズする用語を1つ以上選択します。
1. 画面下部の青いバーで、**AIを使用した翻訳**&#x200B;を選択します。

   翻訳を生成ウィンドウが開きます。

1. 用語または用語を翻訳する言語をクリックします。 すべての言語をすばやく選択するには、**すべて選択**&#x200B;をクリックします。
1. （オプション）翻訳の具体的なガイダンスを提供するには、「AIの手順」フィールドに指示を入力します。
1. 「**生成**」をクリックします。

   AIが翻訳を生成し始めます。

   翻訳を確認ウィンドウが開きます。

1. （オプション）翻訳を調整したり、独自の翻訳を追加したりするには、テーブルの適切な正方形をクリックして、目的の翻訳を入力します。
1. 「**保存**」をクリックします。

## ローカライズされた用語の追加言語への翻訳

AIを活用してローカライズした用語を新しい言語に翻訳したり、独自の翻訳を提供したりすることができます。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. セットアップ領域で、左側のナビゲーションパネルの&#x200B;**ローカライゼーション**&#x200B;をクリックします。
1. ローカライゼーション領域で、「**翻訳**」タブを選択します。

   以前に翻訳された用語とその翻訳のリストが表示されます。

1. （オプション）翻訳を編集または直接入力するには、表内の適切なボックスをクリックし、目的の翻訳を入力します。
1. これらの用語の横にあるチェックボックスをクリックして、追加の翻訳を生成する用語を選択します。
1. ページ下部の青いバーで、**AIで入力**&#x200B;をクリックします。


   翻訳を生成ウィンドウが開きます。

1. 用語または用語を翻訳する言語をクリックします。 すべての言語をすばやく選択するには、**すべて選択**&#x200B;をクリックします。
1. （オプション）翻訳の具体的なガイダンスを提供するには、「AIの手順」フィールドに指示を入力します。
1. 「**生成**」をクリックします。

   AIが翻訳を生成し始めます。

   翻訳を確認ウィンドウが開きます。

1. （オプション）翻訳を調整したり、独自の翻訳を追加したりするには、テーブルの適切な正方形をクリックして、目的の翻訳を入力します。
1. 「**保存**」をクリックします。
1. （オプション）用語のすべての翻訳を削除するには、用語の横にあるチェックボックスをクリックし、ページ下部の青いバーの&#x200B;**削除**&#x200B;をクリックします。


</div>
