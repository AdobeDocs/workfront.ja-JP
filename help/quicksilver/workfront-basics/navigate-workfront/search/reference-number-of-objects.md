---
content-type: reference
navigation-topic: search
title: オブジェクトの参照番号を使用
description: ' [!DNL Adobe Workfront] の場合、項目はオブジェクトとして識別されます。オブジェクトはデータベースに対応し、データと項目の関連付けに使用されます。参照番号は、2 つの類似したオブジェクト（同じ名前のタスクなど）を区別するのに役立ちます。参照番号を検索し、レポートに含めることができます。'
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: ht
source-wordcount: '443'
ht-degree: 100%

---

# オブジェクトの参照番号を使用

[!DNL Adobe Workfront] の場合、項目はオブジェクトとして識別されます。オブジェクトはデータベースに対応し、データと項目の関連付けに使用されます。

Workfront は、オブジェクトの作成時に、次の各オブジェクトに一意の参照番号を自動的に割り当てます。

* プロジェクト
* タスク
* イシュー
* ドキュメント

参照番号は、2 つの類似したオブジェクト（同じ名前のタスクなど）を区別するのに役立ちます。参照番号を検索し、レポートに含めることができます。

>[!IMPORTANT]
>
>* [!DNL Workfront] では、すべての顧客とすべてのオブジェクトに対して、参照番号を連続して割り当てます。例えば、タスクを作成すると、[!DNL Workfront] は参照番号 00005 を割り当てる場合があります。別の顧客が次にプロジェクトを作成すると、そのプロジェクトは、次に利用可能な参照番号（00006 など）を受け取る場合があります。次にイシューを作成すると、そのイシューは参照番号 00007 などを受け取る場合があります。
>* [!DNL Workfront] 内のオブジェクトの参照番号のシーケンスは制御できません。シーケンスは、常にデータベースによって制御されます。
>



## オブジェクトの参照番号を表示する

タスクとイシューに関する参照番号は、デフォルトで表示されます。[!DNL Workfront] を簡単に設定して、他のタイプのオブジェクトの参照番号を表示することもできます。

* [タスクとイシューの参照番号を表示する](#view-reference-numbers-for-tasks-and-issues)
* [他のオブジェクトの参照番号を表示する](#view-reference-numbers-for-other-objects)
* [レポートの参照番号を表示する](#view-reference-numbers-in-reports)

### タスクとイシューの参照番号を表示する

タスクまたはイシューを表示する場合は、参照番号がデフォルトで表示されます。参照番号を確認するには、左側のパネルで「**[!UICONTROL タスクの詳細]**」または「**[!UICONTROL イシューの詳細]**」をクリックし、概要で「**[!UICONTROL 基本情報]**」セクションを見つけます。

![](assets/reference-number-nwe-350x184.png)

### 他のオブジェクトの参照番号を表示する

オブジェクトの参照番号を表示するには、カスタムビューを作成するか、既存のビューを修正して、「[!UICONTROL 参照番号]」フィールドをビューの列に追加します。例えば、[!UICONTROL プロジェクト]ビューを変更して、すべてのプロジェクトの参照番号を表示できます。

ビューを作成または変更する方法について詳しくは、[ [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) のビューの概要を参照してください。

### レポートの参照番号を表示する

[!UICONTROL 参照番号]列をレポートに追加すると、レポート内のオブジェクトの参照番号を表示できます。

レポートに列を追加する方法について詳しくは、[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

## 参照番号でオブジェクトを検索する

[!DNL Workfront] を使用すると、参照番号でオブジェクトを検索できます。

「**[!UICONTROL 検索]**」フィールドにオブジェクトの参照番号を入力し、**[!UICONTROL Enter]** を押します。

Workfront での検索について詳しくは、[検索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)を参照してください。
