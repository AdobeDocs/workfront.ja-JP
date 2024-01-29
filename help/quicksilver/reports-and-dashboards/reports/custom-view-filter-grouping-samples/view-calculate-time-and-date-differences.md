---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：時間と日付の差異の計算'
description: 時間と日付の違いの計算について説明します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 4c12a692971f437a3b248e4a601d4145ce626553
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 表示：時間と日付の差を計算します

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>同じ種類の 2 つの異なるオブジェクト間のAdobe Workfrontで、時間と日付の差を計算することはできません。 たとえば、異なる 2 つのプロジェクト、タスク、またはタスクの 2 つの日付間の時間と日付の差を計算することはできません。

次の間の差を計算できます。

* 同じオブジェクト上の 2 つの日付フィールド間の時間と日付の差
* オブジェクト上のフィールドと親オブジェクト上の別のフィールドの間の時間と日付の差

>[!TIP]
>
>これらの計算では、2 つの日付の間の日数が表示されます。 結果は日数で表示されます。 日付フィールドのタイムスタンプも考慮され、タイムスタンプが一致しない場合は、日数の後に小数が続く場合があります。 タスクが遅れて完了した場合は、日数が負の値で表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> <p>新規： </p><ul><li><p>ビューを変更する寄稿者 </p></li><li>
   <p>レポートを変更するための標準</p></li></ul><p>または</p><p>現在：</p><ul><li><p>ビューの変更をリクエスト </p></li><li>
   <p>レポートを変更する計画</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートに対する権限の管理</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 同じオブジェクト上の 2 つの日付フィールド間の時間と日付の差を計算します

たとえば、タスクの計画完了日と実際の完了日の差を計算できます。

![](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. タスクのリストに移動します。
1. 次から： **表示** ドロップダウンメニューで、 **新しいビュー**.

1. クリック **列を追加** 」と入力し、 **この列に表示** フィールドを選択し、リストに表示されるタイミングで選択します。

1. クリック **列を追加** 」と入力し、 **この列に表示** フィールドを選択し、リストに表示されるタイミングで選択します。

1. クリック **列を追加**&#x200B;を選択し、次に **テキストモードに切り替え**.

1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 検索したテキストを削除します。 **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. クリック **保存**&#x200B;を、 **ビューを保存**.

## オブジェクト上のフィールドと親オブジェクト上の別のフィールドの時間と日付の差を計算します

オブジェクトとその親の一覧については、「相互依存関係とオブジェクトの階層について」の項を参照してください。 [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
たとえば、タスクの計画完了日と、その親タスクの計画完了日の差、またはタスクが存在するプロジェクトの差を計算できます。

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. タスクのリストに移動します。
1. 次から： **表示** ドロップダウンメニューで、 **新しいビュー**.

1. クリック **列を追加** 」と入力し、 **この列に表示** フィールドを選択し、リストに表示されるタイミングで選択します。

1. クリック **列を追加** 」と入力し、 **この列に表示** フィールドを選択し、リストに表示されるタイミングで選択します。

1. クリック **列を追加**&#x200B;を選択し、次に **テキストモードに切り替え**.

1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 検索したテキストを削除します。 **テキストモード** 」ボックスに置き換え、次のいずれかのコードに置き換えます。

   * プロジェクトの計画完了日とタスクの計画完了日の差を表示する手順は、次のとおりです。

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * 親タスクの「計画完了日」とタスクの「計画完了日」の差を表示する手順は、次のとおりです。

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. クリック **保存**&#x200B;を、 **ビューを保存**.
