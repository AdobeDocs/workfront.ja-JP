---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 特定のステータスを使用した、承認保留中プロセスのオブジェクトのリスト
description: ステータスを削除しようとすると、システム内のオブジェクトの承認待ちプロセスで使用されているため削除できないことを示すエラーメッセージが表示される場合があります。これらのオブジェクトを検索して確認し、必要な作業を決定する場合は、それらのオブジェクトを一覧表示するレポートを実行できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 87%

---

# 特定のステータスを使用して、承認待ちのプロセスを持つオブジェクトをリストします

ステータスを削除しようとすると、システム内の少なくとも 1 つの保留中の承認プロセスにあるので、削除できないことを示すエラーメッセージが表示される場合があります。レポートを実行して、承認待ちプロセスのオブジェクトのリストを表示し、各オブジェクトに対して何を実行する必要があるかを決定できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
     <p>新規：標準</p>
     <p>または</p>
     <p>現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p><p>フィルター、ビュー、グループへのアクセスを編集</p></td>
  </tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>作成したレポートに対する管理権限を取得します。</td>
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 標準モード

{{step1-to-reports}}

1. 「**新規レポート**」をクリックして、「**プロジェクトレポート**」、「**タスクレポート**」、または「**イシューレポート**」を選択します。
1. 「**フィルター**」タブを開きます。
1. 「**フィルター規則の追加**」をクリックし、次の手順を実行してルールを設定します。
   1. `status` の入力を開始し、表示されたら「**ステータス**」を選択します。
   1. 2 番目のフィールドは「**等しい**」のままにします。
   1. 3 番目のフィールドで、ステータスの名前を選択します。
1. 「**フィルター規則の追加**」を再度クリックし、次の手順を実行してルールを設定します。
   1. `pending status` の入力を開始し、確認しているオブジェクトタイプ（**プロジェクト**、**タスク**、または&#x200B;**イシュー**）の下に項目が表示されたら、その項目を選択します。
   1. 2 番目のフィールドは「**等しい**」のままにします。
   1. 3 番目のフィールドで、`in` を入力します。
1. 「**フィルター規則の追加**」を再度クリックし、次の手順を実行してルールを設定します。
   1. 承認プロセスの入力を開始し、**承認プロセス**&#x200B;の下に表示されたら&#x200B;**グループ ID** を選択します。
   1. 2 番目のフィールドで「**が空白**」を選択します。
1. 「**保存して閉じる**」をクリックしてレポートを実行し、指定したステータスに基づいて承認プロセスが待ち状態になっている、指定したタイプのオブジェクトを一覧表示します（**プロジェクト**、**タスク**、または&#x200B;**イシュー**）。
1. これらの手順を繰り返して、他の 2 つのオブジェクトタイプに関して同じ情報を見つけます。


## テキストモード

{{step1-to-reports}}

1. 「**新規レポート**」をクリックして、「**プロジェクトレポート**」、「**タスクレポート**」、または「**イシューレポート**」を選択します。
1. 「**フィルター**」タブを開きます。
1. 「**テキストモードに切り替える**」をクリックします。
1. 次の内容をコピーして編集ウィンドウに貼り付け、XXX をステータスの 3 文字のキーに置き換えます。

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   次の記事に示すように、ステータスのリストでキーを表示できます。
   * [システムプロジェクトステータスのリストへのアクセス](project-statuses.md)
   * [システムタスクステータスのリストへのアクセス](task-statuses.md)
   * [システムのイシューステータスのリストへのアクセス](issue-statuses.md)

1. 「**保存して閉じる**」をクリックしてレポートを実行し、指定したステータスに基づいて承認プロセスが待ち状態になっている、指定したタイプのオブジェクトを一覧表示します（**プロジェクト**、**タスク**、または&#x200B;**イシュー**）。
1. これらの手順を繰り返して、他の 2 つのオブジェクトタイプに関して同じ情報を見つけます。
