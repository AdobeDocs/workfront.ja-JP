---
product-area: user-management
navigation-topic: configure-your-user-profile
title: カスタムセクションの作成
description: ' [!DNL Workfront]  web アプリケーションで確認できる情報は、多くの場合、デフォルトでは左側のパネルのセクションに表示されます。各セクションには、 [!DNL Workfront]  のエリアまたはオブジェクトに関する様々な情報が含まれています。'
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: ht
source-wordcount: '678'
ht-degree: 100%

---

# カスタムセクションの作成

## [!DNL Adobe Workfront] セクション

[!DNL Workfront] web アプリケーションで確認できる情報は、多くの場合、デフォルトでは左側のパネルのセクションに表示されます。各セクションには、[!DNL Workfront] のエリアまたはオブジェクトに関する様々な情報が含まれています。\
[!DNL Workfront] のデフォルトのエリアについて詳しくは、[デフォルトの  [!DNL Adobe Workfront]  レイアウトについて](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)の記事を参照してください。

[!DNL Workfront] にデフォルトで付属するセクションに加え、ワークフローに関連する情報を表示できるダッシュボードを追加できます。すべてのエリアやオブジェクトにダッシュボードを追加できるわけではありません。

次の表に、左側のパネルにセクションが含まれる [!DNL Workfront] のすべてのエリアとオブジェクトの一覧と、どのセクションがカスタマイズ可能かを示します。

| **[!DNL Workfront]のエリアまたはオブジェクト** | **デフォルトのシステムセクション** | **カスタムセクション** |
|---|---|---|
| [!UICONTROL プロジェクト]エリア | ✓ | ✓ |
| [!UICONTROL チーム] | ✓ |   |
| [!UICONTROL リクエスト]エリア | ✓ |   |
| [!UICONTROL タイムシート]エリア | ✓ |   |
| [!UICONTROL ポートフォリオ] | ✓ | ✓ |
| [!UICONTROL プログラム] | ✓ | ✓ |
| [!UICONTROL プロジェクト] | ✓ | ✓ |
| [!UICONTROL タスク] | ✓ |  ✓ |
| [!UICONTROL イシュー] |  ✓ |  ✓ |
| [!UICONTROL ユーザー] |  ✓ |  ✓ |
| [!UICONTROL ドキュメント] |  ✓ |  ✓ |

{style="table-layout:auto"}

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td>[!UICONTROL Reviewer] またはそれ以上の権限</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td>オブジェクトタイプへのアクセスの表示</td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスタイプを確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!DNL Workfront] オブジェクトまたはエリアの左側のパネルにダッシュボードを追加

ダッシュボードを追加する前に、表示するすべての情報を含むダッシュボードを作成する必要があります。外部ページを作成することもできます。\
ダッシュボードの作成について詳しくは、[ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)の記事を参照してください。\
外部ページの作成について詳しくは、[ダッシュボードへの外部 Web ページの埋め込み](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)の記事を参照してください。

ダッシュボードや外部ページを作成した後、左側のパネルに追加できます。

1. 左側のパネルのカスタムセクションに追加できる [!DNL Workfront] エリアまたはオブジェクトのいずれかに移動します。\
   または
1. 左側のパネルで[!UICONTROL ダッシュボード]を追加できるオブジェクトに移動します。\
   カスタムセクションを追加できるエリアとオブジェクトについて詳しくは、[[!DNL Adobe Workfront] セクション](#adobe-workfront-sections)を参照してください。
1. 左側のパネルで「**[!UICONTROL ダッシュボードを追加]**」をクリックします。
1. ダッシュボードの名前を「**[!UICONTROL クイックリンク名]**」フィールドに入力します。これは自分だけに表示されます。
1. 「**[!UICONTROL ダッシュボードを選択]**」フィールドに既存のダッシュボードまたは外部ページの名前を入力し、リストに表示されたらダッシュボードを選択します。
1. 「**[!UICONTROL 追加]**」をクリックします。
1. （オプション）セクションを表示する順序でドラッグ＆ドロップします。

   上部のセクションは、ページのデフォルトのセクションです。

   個々のオブジェクトに対して作成したセクションは、同じタイプのすべてのオブジェクトにアクセスすると表示され、自分だけが使用できます。

## オブジェクトの左側のパネルでのダッシュボードの表示

オブジェクトの下にダッシュボードを追加する方法について詳しくは、この記事の [[!UICONTROL Workfront オブジェクトまたはエリアの左側のパネルへのダッシュボード ] の追加](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area)の節を参照してください。

オブジェクトの下のカスタムセクションにダッシュボードを追加する場合、そのオブジェクトはダッシュボードのフィルターとして機能します。例えば、タスクレポートをダッシュボードに追加し、そのダッシュボードをプロジェクトに追加する場合、プロジェクト上のダッシュボードを含むカスタムセクションには、表示中のプロジェクトのタスクのみが表示されます。

次のオブジェクトは、表示されるオブジェクトに対してフィルタリングされます（そのオブジェクトの階層がオブジェクトよりも高い場合）。

* プロジェクト
* タスク
* イシュー
* 承認プロセス
* メモ
* ドキュメント

オブジェクトの階層と相互依存関係について詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の記事の[オブジェクトの相互依存性と階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)の節を参照してください。

## レイアウトテンプレートを使用した左側のパネルのカスタマイズ

ダッシュボードを [!DNL Workfront] インスタンスに追加すると、自分だけに表示されます。

[!DNL Workfront] のセクションをカスタマイズして、レイアウトテンプレート内の複数のユーザーと新規レイアウトを共有できます。レイアウトテンプレート内の他のユーザーと共有できるのは、システム管理者またはグループ管理者だけです。レイアウトテンプレートを使用して左側のパネルをカスタマイズする方法について詳しくは、[レイアウトテンプレートを使用した左側のパネルのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)を参照してください。
