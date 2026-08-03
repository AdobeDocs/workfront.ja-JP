---
user-type: administrator
product-area: system-administration;setup
title: 変更履歴の表示と管理
description: 変更履歴を使用すると、Workfront オブジェクトとフィールドに対する変更のログを表示できます。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 100b900bd7419d78a3135358026ec5e27755fdeb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 6%

---

# 変更履歴の表示と管理

{{preview-fast-release-general}}

変更履歴を使用すると、Adobe Workfrontのオブジェクトと特定のフィールドに対する変更を設定および追跡できます。 柔軟な設定により、追跡するオブジェクトとフィールドを正確に設定できます。

変更履歴では、定義した次の種類のデータを追跡できます。

* アクセスレベルや担当業務の作成や削除など、設定領域でのアクティビティ
* プロジェクトの説明の編集やユーザーのレイアウトテンプレートの変更など、フィールドレベルの更新
* プロジェクトのステータスの更新や、タスクへのカスタムフォームの添付など、オブジェクトの更新
* <span class="preview">参加者と決定を含む、統一されたレビューと承認のワークフローアクティビティ </span>

追跡するオブジェクトとフィールドの定義について詳しくは、[変更履歴で追跡するフィールドの設定](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md)を参照してください。

変更履歴リストでは、次のような属性を含むWorkfront オブジェクトに対する変更履歴のログを確認できます。

* オブジェクト名
* オブジェクトタイプ
* 変更のタイプ（操作）
* 変更の日時
* Sourceのアーキテクチャを活用します。例えば、特定のユーザー、API、Workfront Fusion、AI LLM、Workfrontシステムなどです

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><span class="preview">変更履歴への管理アクセス</span></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.
-->


## 変更履歴リストの表示

設定領域で変更履歴ログを表示できます。

変更履歴リストは強化されたリストで、フィルター、列、行の高さ、日付選択、検索バーが備わっています。

{{step-1-to-setup}}

1. 左側のパネルで、**トラッキングの変更/履歴リストの変更**&#x200B;をクリックします。

   変更履歴リストが開きます。

1. 変更が表示される日付を調整するには、日付選択ツールをクリックし、新しい日付を選択します。

   過去90日間の変更が利用可能です。

1. 特定の用語を検索するには、検索ボックス内をクリックして、用語を入力します。 入力時に結果がリスト内でハイライト表示されます。
1. （オプション）列でフィルタリングするには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の拡張リスト ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)の[項目のフィルタリングを参照してください。
1. （オプション）列を非表示、表示、または並べ替えるには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の[列をカスタマイズ ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)を参照してください。
1. （オプション）列を追加または削除するには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の「[列マネージャー](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)」を参照してください。
1. （オプション）行の高さを調整するには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の「[ ビュー内の行の高さを変更](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)」を参照してください。

## 変更履歴を書き出し

{{step-1-to-setup}}

1. 左側のパネルで、**トラッキングの変更/履歴リストの変更**&#x200B;をクリックします。
1. 書き出す項目を表示するには、リストをフィルター処理します。
1. **書き出し** アイコン ![書き出しアイコン ](assets/export-icon.png)をクリックし、XLSX形式とCSV形式のどちらに保存するかを選択します。

   ファイルを保存ボックスが開き、書き出したファイルをコンピューターに保存できます。
   書き出したファイルの保存を完了します。パソコンで見つけて、他の人と共有できます。



