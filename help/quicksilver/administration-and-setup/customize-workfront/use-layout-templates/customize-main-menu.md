---
title: レイアウトテンプレートを使用したメインメニューのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfrontの管理者またはグループ管理者は、レイアウトテンプレートを使用して、Workfrontでメインメニューを開いたときに表示されるオプションを設定できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# レイアウトテンプレートを使用したメインメニューのカスタマイズ

Adobe Workfront管理者またはグループ管理者は、レイアウトテンプレートを使用して、Workfrontでメインメニューを開く際にユーザーに表示されるオプションを設定できます。

![メインメニューオプション](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>ユーザーに表示されるメインメニューオプションは、ライセンスの種類と、アクセスレベルで設定されている設定によって異なります。 このレイアウトテンプレートを使用する一部のユーザーは、ここで選択するすべてのオプションが表示されない場合があります。 詳しくは、 [アクセスレベルと権限の連携](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) および [各オブジェクトタイプの機能への設定可能なアクセス](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

グループのレイアウトテンプレートについて詳しくは、 [グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfrontプラン</strong></td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfrontライセンス</strong></td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## メインメニューのカスタマイズ

1. レイアウトテンプレートの使用を開始する ( [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. クリック **メインメニューの設定** 右上隅付近にある

   表示される「メインメニュー」(Main Menu) ボックスで、テンプレートのメインメニューで現在アクティブな項目と、追加可能な項目を確認できます。 次に、追加できるすべての項目を示します。

   * ホーム

      >[!TIP]
      >
      >既定では、メインメニューの [ 更新 ] 領域を含むレイアウトテンプレートがプロファイルに関連付けられている場合を除き、[ ホーム ] には [ レビューライセンスユーザの更新 ] と表示されます。

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
      >シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用でき、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md).

   * チーム
   * ユーザー

      >[!NOTE]
      >
      >プランライセンスを持つユーザーのみがユーザーを表示できます ![](assets/users-icon-in-main-menu.png) をクリックします。

   * リクエスト
   * タイムシート
   * ドキュメント
   * テンプレート
   * 分析
   * 校正
   * 目標

      >[!NOTE]
      >
      >追加のライセンスが必要です。 Workfront目標について詳しくは、 [Adobe Workfront目標の概要](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * マイ更新
   * ボード
   * ブループリント

1. 次のいずれかの操作を行います。

   * を隠す ![](assets/remove-icon---x-in-circle.png) **アクティブな項目** 表示したくない
   * 表示 ![](assets/add-icon-plus-in-circle.png) **利用可能な項目** を選択します。
   * ドラッグ ![](assets/move-icon---dots.png) **アクティブな項目** をクリックして、メインメニューの表示順を変更します。

1. クリック **完了**.

   また、 **キャンセル** 変更を破棄する場合は、いつでも変更を破棄できます。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、 **保存**.

   >[!TIP]
   >
   >「保存」はいつでもクリックして進行状況を保存でき、後でテンプレートの変更を続行できます。

レイアウトテンプレートについて詳しくは、 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
