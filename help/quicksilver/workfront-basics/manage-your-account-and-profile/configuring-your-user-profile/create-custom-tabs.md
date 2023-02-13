---
product-area: user-management
navigation-topic: configure-your-user-profile
title: カスタムセクションの作成
description: に表示される情報 [!DNL Workfront] Web アプリケーションは、多くの場合、デフォルトでは左側のパネルのセクションに表示されます。 各セクションには、 [!DNL Workfront] 領域またはオブジェクト。
author: Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 3%

---

# カスタムセクションの作成

## [!DNL Adobe Workfront] セクション

に表示される情報 [!DNL Workfront] web アプリケーションは、多くの場合、デフォルトで左のパネルセクションに表示されます。 各セクションには、 [!DNL Workfront] 領域またはオブジェクト。\
のデフォルト領域の詳細 [!DNL Workfront]（記事を参照） [デフォルトについて [!DNL Adobe Workfront] レイアウト](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

に加えて、 [!DNL Workfront] デフォルトでは、ワークフローに関連する情報を表示できるダッシュボードを追加できます。 すべての領域とオブジェクトにダッシュボードを追加することはできません。

次の表に、 [!DNL Workfront] 左側のパネルにセクションが含まれ、それらのセクションをカスタマイズできる領域とオブジェクト：

| **[!DNL Workfront]領域またはオブジェクト** | **デフォルトのシステムセクション** | **カスタムセクション** |
|---|---|---|
| [!UICONTROL プロジェクト] 領域 | ✓ | ✓ |
| [!UICONTROL チーム] | ✓ |   |
| [!UICONTROL リクエスト] 領域 | ✓ |   |
| [!UICONTROL タイムシート] 領域 | ✓ |   |
| [!UICONTROL ポートフォリオ] | ✓ | ✓ |
| [!UICONTROL プログラム] | ✓ | ✓ |
| [!UICONTROL プロジェクト] | ✓ | ✓ |
| [!UICONTROL タスク] | ✓ |  ✓ |
| [!UICONTROL 問題] |  ✓ |  ✓ |
| [!UICONTROL ユーザー] |  ✓ |  ✓ |
| [!UICONTROL ドキュメント] |  ✓ |  ✓ |

{style=&quot;table-layout:auto&quot;}

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td>[!UICONTROL レビュー担当者 ] 以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td>オブジェクトタイプへのアクセスの表示</td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、 [!DNL Workfront] 管理者。

## の左側のパネルにダッシュボードを追加する [!DNL Workfront] オブジェクトまたは領域

ダッシュボードを追加する前に、表示するすべての情報を含むダッシュボードを作成する必要があります。 外部ページを作成することもできます。\
ダッシュボードの構築について詳しくは、「 [ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
外部ページの作成について詳しくは、 [外部 Web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

ダッシュボードや外部ページを作成した後、それらを左のパネルに追加できます。

1. 次のいずれかに移動します。 [!DNL Workfront] カスタムセクションを左側のパネルに追加できる領域またはオブジェクト。\
   または
1. オブジェクトに移動し、そこで [!UICONTROL dashboard] をクリックします。\
   カスタムセクションを追加できる領域とオブジェクトの詳細については、「 [[!DNL Adobe Workfront] セクション](#adobe-workfront-sections).
1. クリック **[!UICONTROL ダッシュボードを追加]** をクリックします。
1. ダッシュボードの名前を **[!UICONTROL クイックリンク名]** フィールドに入力します。 これはあなただけに表示されます。
1. 既存のダッシュボードまたは外部ページの名前を **[!UICONTROL ダッシュボードを選択]** 「 」フィールドを選択し、リストに表示されたらダッシュボードを選択します。
1. クリック **[!UICONTROL 追加]**.
1. （オプション）セクションを表示する順序でドラッグ&amp;ドロップします。

   上部のセクションは、ページのデフォルトのセクションです。

   個々のオブジェクトに対して作成したセクションは、同じタイプのすべてのオブジェクトにアクセスすると表示され、自分だけが使用できます。

## オブジェクトの左側のパネルにダッシュボードを表示

オブジェクトの下にダッシュボードを追加する方法について詳しくは、「 [[!UICONTROL ダッシュボードを追加する] Workfrontオブジェクトまたは領域の左パネル](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) 」を参照してください。

オブジェクトの下のカスタムセクションにダッシュボードを追加する場合、そのオブジェクトはダッシュボードのフィルタとして機能します。 例えば、タスクレポートをダッシュボードに追加し、そのダッシュボードをプロジェクトに追加した場合、プロジェクト上のダッシュボードを含むカスタムセクションには、表示中のプロジェクト上のタスクのみが表示されます。

次のオブジェクトは、表示されるオブジェクトに対してフィルタリングされます（そのオブジェクトの階層がオブジェクトよりも高い場合）。

* プロジェクト
* タスク
* 問題
* 承認プロセス
* メモ
* ドキュメント

オブジェクトの階層と相互依存関係の詳細については、 [オブジェクトの相互依存性と階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 記事内 [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## レイアウトテンプレートの左側のパネルをカスタマイズする

ダッシュボードを [!DNL Workfront] 例えば、ユーザーに対してのみ表示されます。

セクションは、 [!DNL Workfront] およびは、レイアウトテンプレート内の複数のユーザーと新しいレイアウトを共有します。 レイアウトテンプレート内の他のユーザーと共有できるのは、システム管理者またはグループ管理者だけです。 レイアウトテンプレートを使用して左側のパネルをカスタマイズする方法について詳しくは、 [レイアウトテンプレートを使用して左のパネルをカスタマイズする](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
