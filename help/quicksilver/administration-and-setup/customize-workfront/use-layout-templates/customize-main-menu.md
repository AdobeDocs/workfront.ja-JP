---
title: レイアウトテンプレートを使用したメインメニューのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront の管理者またはグループ管理者は、レイアウトテンプレートを使用して、Workfront でメインメニューを開いた際に表示されるオプションを設定できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 71%

---

# レイアウトテンプレートを使用したメインメニューのカスタマイズ

<!--Audited: 01/2024-->

Adobe Workfront の管理者またはグループ管理者は、レイアウトテンプレートを使用して、Workfront でメインメニューを開いた際に表示されるオプションを設定できます。

![メインメニューオプション](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>ユーザーに表示されるメインメニューオプションは、ライセンスタイプおよびアクセスレベルで指定されている設定によって異なります。このレイアウトテンプレートを使用する一部のユーザーには、ここで選択するすべてのオプションが表示されない場合があります。詳しくは、[アクセスレベルと権限の連携](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)および[各オブジェクトタイプの機能への設定可能なアクセス](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)を参照してください。
>
>Adobe Workfront統合エクスペリエンスでオンボーディングされた組織の場合は、メインメニューに異なるオプションが表示されることがあります。 詳しくは、[WorkfrontのAdobe統合エクスペリエンス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td><p>現在：プラン</p>
   または
   <p>新規：標準</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
    <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*アクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## メインメニューをカスタマイズ

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. テンプレートの右上隅の「**メインメニューをセット**」をクリックします。

   「メインメニュー」ボックスが開き、テンプレートのメインメニューで現在表示されているエリアと、追加できる項目を確認できます。次に、追加できるすべての項目を示します。
   * ホーム

     >[!TIP]
     >
     >既定では、メイン メニューの [ ホーム ] アイコンには、（現在のライセンス プラン内の）レビューライセンス ユーザに対する [ マイ アップデート ] 領域が表示されます。ただし、[ ホーム ] 領域に加えて、メイン メニューの [ マイ アップデート ] 領域を含むレイアウト テンプレートがプロファイルに関連付けられている場合は除きます。

   * ポートフォリオ
   * プログラム
   * プロジェクト
   * レポート
   * ダッシュボード
   * カレンダー
   * リソース
   * シナリオ

     >[!NOTE]
     >
     >シナリオプランナには、追加のライセンスが必要です。Workfront シナリオプランナについては、[シナリオプランナの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。

   * チーム
   * ユーザー

     >[!NOTE]
     >
     >現在のライセンスモデルのプランライセンスを持つユーザー、または新しいライセンスモデルの標準ライセンスを持つユーザーのみが、メインメニューのユーザー ![ ユーザーアイコン ](assets/users-icon-in-main-menu.png) を表示できます。

   * リクエスト
   * タイムシート
   * ドキュメント
   * テンプレート
   * 分析
   * プルーフ
   * Goals

     >[!NOTE]
     >
     >Goals では追加のライセンスが必要です。Workfront Goals について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。

   * マイ更新
   * ボード
   * ブループリント
   * プラン

     >[!NOTE]
     >
     >計画には追加ライセンスが必要です。 Workfront計画について詳しくは、[Adobe Workfront計画の概要を参照してください ](/help/quicksilver/planning/general/planning-overview.md)

1. 次のいずれかの操作を行います。

   * 表示しない ![ 非表示アイコン ](assets/remove-icon---x-in-circle.png)**アクティブな項目** を非表示にする
   * メインメニューに表示する ![ アイコンを表示 ](assets/add-icon-plus-in-circle.png)**利用可能な項目** を表示します。
   * ドラッグ ![ ドラッグアイコン ](assets/move-icon---dots.png)**アクティブなアイテム** を使用して、メインメニューの表示順序を変更できます。

1. 「**完了**」をクリックします。

   また、変更を破棄する場合は、いつでも「**キャンセル**」をクリックして変更を破棄できます。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが完了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「保存」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。
