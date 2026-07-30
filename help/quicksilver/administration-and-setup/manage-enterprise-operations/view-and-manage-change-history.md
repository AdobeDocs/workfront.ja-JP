---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 変更履歴
description: 変更履歴を使用すると、Workfront オブジェクトに対する変更のログを表示できます
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: ba1843cf6be446a809f9526608a3ae3bef69c494
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 7%

---

# 変更履歴の表示と管理

監査ログを含む変更履歴は、「設定」の「変更履歴」エリアで確認できます。

* **監査ログ**&#x200B;は、ユーザーによってトリガーされた変更です。
監査ログと監査ログ領域について詳しくは、[監査ログの概要](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)を参照してください
* **設定**&#x200B;には、変更履歴リストで追跡されているフィールドが表示されます。
設定は現在、情報としてのみ利用でき、変更できません。追跡するフィールドを変更する機能は、近日中に利用できるようになります。
* **変更履歴リスト**&#x200B;を使用すると、次のような属性を含む、Workfront オブジェクトに対する変更のログを表示できます。

  * オブジェクト
  * オブジェクトタイプ
  * 変更のタイプ（操作）
  * Sourceのアーキテクチャを活用します。例えば、特定のユーザー、API、Workfront Fusion、AI LLM、Workfrontシステムなどです

  <span class="preview">統一されたレビューと承認のワークフローアクティビティは、参加者と決定を含む変更履歴で追跡されます。</span>

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
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 監査ログの表示と管理

監査ログを表示および管理するには、[監査ログの表示と書き出し](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)を参照してください。

## 変更を追跡するための設定領域を表示します

>[!NOTE]
>
>設定は現在、情報としてのみ利用でき、変更できません。 追跡するフィールドを変更する機能は、近日中に利用できるようになります。

追跡される変更のタイプを表示するには、次の手順に従います。

{{step-1-to-setup}}

1. 左側のパネルで、**変更履歴** ![変更履歴アイコン &#x200B;](assets/change-history-icon.png)をクリックします。
1. 「**設定**」をクリックします。

   フィールドは、オブジェクトタイプ別にグループ化されて表示されます。

1. 特定のオブジェクトの下にフィールドを表示するには、オブジェクトタイプの横にあるドロップダウン矢印をクリックします。

## 変更履歴リストの表示

Workfront管理者は、設定領域で変更履歴を表示できます。

変更履歴リストは強化されたリストで、フィルター、列、行の高さ、日付選択、検索バーが備わっています。

{{step-1-to-setup}}

1. 左側のパネルで、**変更履歴** ![変更履歴アイコン &#x200B;](assets/change-history-icon.png)をクリックします。
1. 「**履歴リストを変更**」をクリックします。

   変更履歴リストが開きます。

1. 変更が表示される日付を調整するには、日付選択ツールをクリックし、新しい日付を選択します。

   過去90日間の変更が利用可能です。

1. 特定の用語を検索するには、検索バーをクリックして用語を入力します。 入力時に結果がリスト内でハイライト表示されます。
1. （オプション）列でフィルタリングするには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の拡張リスト [&#128279;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)の項目のフィルタリングを参照してください。
1. （オプション）列を非表示、表示、または並べ替えるには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の[列をカスタマイズ &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)を参照してください。
1. （オプション）列を追加または削除するには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の「[列マネージャー](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)」を参照してください。
1. （オプション）行の高さを調整するには、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の「[&#x200B; ビュー内の行の高さを変更](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)」を参照してください。

## 変更履歴を書き出し

{{step-1-to-setup}}

1. 左側のパネルで、**トラッキングの変更/履歴リストの変更**&#x200B;をクリックします。
1. 書き出す項目を表示するには、リストをフィルター処理します。
1. **書き出し** アイコン ![書き出しアイコン &#x200B;](assets/export-icon.png)をクリックし、XLSX形式とCSV形式のどちらに保存するかを選択します。

   ファイルを保存ボックスが開き、書き出したファイルをコンピューターに保存できます。
   書き出したファイルの保存を完了します。パソコンで見つけて、他の人と共有できます。



