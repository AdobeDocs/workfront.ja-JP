---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: システム更新の設定
description: Workfront は、オブジェクトの[!UICONTROL 更新]エリアで自動システム更新を生成し、ユーザーがオブジェクトに対して実行した変更を記録します。 [!DNL Workfront]  管理者は、 [!DNL Workfront]  がどのオブジェクトフィールドおよびアクションを追跡するかを設定して、システム更新を記録できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 96%

---

# システム更新の設定

[!DNL Adobe Workfront] は、オブジェクトの[!UICONTROL 更新]エリアで自動システム更新を生成し、次のイベントを記録します。

* オブジェクトフィールドでユーザーが行う変更
* オブジェクトに対してユーザーが実行するアクション

これらのシステム更新には、次の種類の情報が含まれます。

* 変更が加えられた
* 変更を加えたユーザーの名前
* 変更日時

システム更新について詳しくは、[システムで追跡される更新](../system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

[!DNL Workfront] 管理者は、[!DNL Workfront] がどのオブジェクトフィールドおよびアクションを追跡するかを設定して、システム更新を記録できます。

例えば、システム全体でユーザーがイシューの名前に対して行ったすべての変更を [!DNL Workfront] で追跡できます。イシュー名の変更は、イシューの[!UICONTROL 更新]エリアにシステム更新として表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!DNL Workfront] がオブジェクトタイプのどのフィールドを追跡するかを決定

ユーザーが [!DNL Workfront] インターフェイス全体で特定のオブジェクトタイプに関連付けられた情報を変更したときに、[!DNL Workfront] がどの情報を追跡するかを決定できます。これを行うには、[!DNL Workfront] が追跡するオブジェクトタイプのフィールドを追加または削除します。

>[!NOTE]
>
>* [!DNL Workfront] は、計算済みカスタムフィールドの更新を追跡して記録することはできません。
>* プロジェクト、タスク、イシュー、ポートフォリオ、プログラムおよびユーザーのシステム更新をカスタマイズできます。テンプレート、ドキュメントまたはタイムシートのシステムアップデートはカスタマイズできませんが、[!DNL Workfront] は、これらのオブジェクトのシステム更新を記録します。
>



* [ [!DNL Workfront]  が追跡するフィールドの追加](#add-fields-you-want-workfront-to-track)
* [追跡しないフィールドの削除](#remove-fields-that-you-don-t-want-tracked)

### [!DNL Workfront] が追跡するフィールドの追加 {#add-fields-you-want-workfront-to-track}

[!DNL Workfront] インターフェイス全体に渡り、特定のタイプのオブジェクトについて [!DNL Workfront] が追跡するフィールドを追加できます。ユーザーがそのフィールドの情報を変更した場合、[!DNL Workfront] は、変更に関する情報をシステム更新として、オブジェクトの[!UICONTROL 更新]エリアに記録します。

>[!NOTE]
>
>更新フィードでは、最大 300 個の組み込みフィールドとカスタムフィールドを追跡できます。フィールドの最大数を追跡し、さらに「[!UICONTROL すべてのフィールド]」サブタブに表示されていない追加フィールドを追跡する場合、新しいフィールドを追跡するには、まず追跡済みフィールドの一部を削除する必要があります。更新フィールドからフィールドを削除する方法について詳しくは、[追跡しないフィールドの削除](#remove-fields-that-you-don-t-want-tracked)を参照してください。

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**[!UICONTROL 設定]**」![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、**[!UICONTROL インターフェイス]**／**[!UICONTROL フィードを更新]**&#x200B;をクリックします。

1. 「**[!UICONTROL フィールドを追加]**」をクリックし、次に追跡するオブジェクトをクリックします。

1. 「**[!UICONTROL フィードを更新]**」ボックスが表示されたら、オブジェクトの組み込み（標準）フィールドまたはカスタムフィールドを入力し、リストに表示されたらクリックして選択します。

   [!DNL Workfront] が既にフィールドを追跡している場合、リストから再度追加することはできません。

1. [!DNL Workfront] が追跡するすべてのフィールドを追加したら、「**[!UICONTROL フィールドを追加]**」をクリックします。

   追加した組み込みフィールドが「**[!UICONTROL 組み込みフィールド]**」サブタブの下に表示されます。

   追加したカスタムフィールドは、「**[!UICONTROL カスタムフィールド]**」サブタブの下に表示されます。

   「**[!UICONTROL すべてのフィールド]**」サブタブには、追跡されている組み込みフィールドおよびカスタムフィールドの両方が表示されます。

### 追跡しないフィールドの削除 {#remove-fields-that-you-don-t-want-tracked}

[!DNL Workfront] インターフェイス全体で、特定のタイプのオブジェクトについてシステムで追跡しないフィールドを削除できます。

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**[!UICONTROL 設定]**」![](assets/gear-icon-settings.png) をクリックします。

1. **[!UICONTROL インターフェイス]**／**[!UICONTROL フィードを更新]**&#x200B;をクリックします。

1. 「**[!UICONTROL 追跡済みフィールド]**」タブで、「**[!UICONTROL すべてのフィールド]**」サブタブを選択します。

   これには、現在追跡されている組み込みフィールドおよびカスタムフィールドの両方が表示されます。

1. 追跡を停止するフィールドを選択し、「**[!UICONTROL 削除]**」をクリックします。

1. 表示される「**[!UICONTROL フィールドを削除]**」ボックスで、「**[!UICONTROL はい、削除します]**」をクリックして確定します。

以前に追跡されたフィールドに関する更新は、記録された[!UICONTROL 更新]エリアに保存されます。

## [!DNL Workfront] がオブジェクトタイプのどのアクションを追跡するかを決定

ユーザーが [!DNL Workfront] インターフェイス全体でオブジェクトに対して実行できる次のアクションは [!DNL Workfront] で追跡できます。

例えば、ユーザーがタスクまたはイシューへの割り当てを更新するたびに、[!DNL Workfront] に更新を記録できます。変更は、タスクまたはイシューの[!UICONTROL 更新]エリアに、システム更新として表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>アクション</strong> </th> 
   <th><strong>オブジェクト</strong> </th> 
   <th><strong>デフォルトのステータス</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>割り当ての変更</td> 
   <td>タスク、イシュー</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>ベースラインの削除</td> 
   <td>プロジェクト</td> 
   <td> <p>無効</p> </td> 
  </tr> 
  <tr> 
   <td>請求記録の作成または削除</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>ドキュメントの作成または削除</td> 
   <td>プロジェクト、タスク、イシュー、ポートフォリオ、プログラム</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>費用の作成または削除</td> 
   <td>プロジェクト、タスク</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>時間の記録または削除</td> 
   <td>プロジェクト、タスク、イシュー</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>イシューを削除</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>タスクの削除</td> 
   <td>プロジェクト</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>誰かのアクセス権限の変更</td> 
   <td>プロジェクト、タスク、イシュー、ドキュメント、ポートフォリオ、プログラム</td> 
   <td> <p>有効</p> </td> 
  </tr> 
  <tr> 
   <td>コメントオブジェクトの登録</td> 
   <td>プロジェクト、タスク、イシュー</td> 
   <td> <p>有効</p> </td> 
  </tr> 
 </tbody> 
</table>

[!DNL Workfront] で追跡するアクションを設定するには、次の操作を行います。

1. [!DNL Adobe Workfront]の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. **[!UICONTROL インターフェイス]**／**[!UICONTROL フィードの更新]**&#x200B;をクリックします。

1. 「**[!UICONTROL アクション]**」タブをクリックします。

1. アクションを選択して有効にするか、アクションの選択を解除して無効にします。
1. 「**[!UICONTROL 保存]**」をクリックします。

アクションを無効にすると、そのアクションに関して以前に記録された更新は、記録が行われた[!UICONTROL 更新]エリアに保存されます。
