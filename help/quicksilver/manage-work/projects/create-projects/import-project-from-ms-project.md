---
product-area: projects
navigation-topic: create-projects
title: Microsoft Project からプロジェクトを読み込む
description: Microsoft Project からAdobe Workfrontにプロジェクトを読み込み、1 つのアプリケーションですべてのプロジェクトを管理できます。 Microsoft Project からプロジェクトを読み込むたびに、Workfrontに新しいプロジェクトが作成されます。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# Microsoft Project からプロジェクトを読み込む

Microsoft Project からAdobe Workfrontにプロジェクトを読み込み、1 つのアプリケーションですべてのプロジェクトを管理できます。 Microsoft Project からプロジェクトを読み込むたびに、Workfrontに新しいプロジェクトが作成されます。

>[!IMPORTANT]
>
>すべてのMicrosoftプロジェクトフィールドがWorkfrontに転送されるわけではありません。
>
>WorkfrontとMicrosoft Project 間でのフィールドの互換性について詳しくは、 [Microsoft Project フィールドのAdobe Workfrontプロジェクトへのマッピング](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## アクセス要件

P&amp;P 用に下書き：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のライセンス：標準 </p> 
   または
   <p>レガシーライセンス：プラン </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 プロジェクトへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトを作成すると、自動的にプロジェクトに対する管理権限が付与されます </p> <p> プロジェクト権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 プロジェクトへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトを作成すると、自動的にプロジェクトに対する管理権限が付与されます </p> <p> プロジェクト権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## MS プロジェクトからプロジェクトを作成する

プロジェクトは、メインメニューの「プロジェクト」領域、またはポートフォリオやプログラムの「プロジェクト」領域から作成できます。

1. Microsoft Project に移動し、Workfrontで読み込むプロジェクトを開きます。
1. クリック **ファイル**&#x200B;を、 **名前を付けて保存** プロジェクトを.xml ファイルとして保存します。

1. Workfrontにログインします。
1. 次のいずれかの操作を行います。

   * 次をクリック： **メインメニュー** ![](assets/main-menu-icon.png)をクリックし、 **プロジェクト**&#x200B;を展開し、 **新規プロジェクト**.
   * ポートフォリオに移動し、を展開します。 **新規プロジェクト**.
   * プログラムに移動し、を展開します。 **新規プロジェクト**.
   * グループ管理者は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。 詳しくは、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. を選択します。 **MS プロジェクトを読み込み** オプション。

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. クリック **ファイルを選択**&#x200B;次に、Microsoft Project から書き出したコンピューター上の.xml ファイルを参照します。
1. 選択したファイルをインポートします。

   Workfrontは読み込み処理を開始し、Microsoftプロジェクトから書き出されたファイルに基づいて新しいプロジェクトを作成します。

   読み込み処理が完了したら、新しいプロジェクトページが開き、読み込みが正常に完了したことを示す確認メッセージが表示されます。

   >[!NOTE]
   >
   >Workfrontでは、ファイルのアップロードに 15 分の時間制限があります。 ファイルのアップロードに時間がかかる場合は、プロジェクトを小さなプロジェクトに分割し、それらを個別に読み込むことをお勧めします。 タスクをWorkfrontに読み込んだら、タスクを 1 つのプロジェクトから別のプロジェクトに移動して、1 つのプロジェクトに組み合わせます。 タスクの移動について詳しくは、 [タスクを移動](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. （オプション） Workfrontでプロジェクトの編集を続行します。 プロジェクトの編集について詳しくは、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

   テンプレートから作成された新しいプロジェクトのステータスは、「プロジェクトの環境設定」領域のWorkfront管理者、または「グループプロジェクトの環境設定」領域のグループ管理者が定義したステータスに対応します。 プロジェクトの環境設定の詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
