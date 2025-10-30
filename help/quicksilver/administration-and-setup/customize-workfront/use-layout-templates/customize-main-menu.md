---
title: レイアウトテンプレートを使用したメインメニューのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront の管理者またはグループ管理者は、レイアウトテンプレートを使用して、Workfront でメインメニューを開いた際に表示されるオプションを設定できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 61%

---

# レイアウトテンプレートを使用したメインメニューのカスタマイズ

{{preview-fast-release-general}}

<!--Audited: 01/2024-->

Adobe Workfront の管理者またはグループ管理者は、レイアウトテンプレートを使用して、Workfront でメインメニューを開いた際に表示されるオプションを設定できます。

>[!NOTE]
>
>ユーザーに表示されるメインメニューオプションは、ライセンスタイプおよびアクセスレベルで指定されている設定によって異なります。このレイアウトテンプレートを使用する一部のユーザーには、ここで選択するすべてのオプションが表示されない場合があります。詳しくは、[アクセスレベルと権限の連携](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)および[各オブジェクトタイプの機能への設定可能なアクセス](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)を参照してください。
>
>Adobe Workfront統合エクスペリエンスでオンボーディングされた組織の場合は、メインメニューに異なるオプションが表示されることがあります。 詳しくは、[WorkfrontのAdobe統合エクスペリエンス &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p>
       <p>メインメニューへのカスタムアプリケーションの追加は、Adobe App Builderでライセンスを取得している組織のみが使用できます。</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
     >現在のライセンスモデルのプランライセンスを持つユーザー、または新しいライセンスモデルの標準ライセンスを持つユーザーのみが、メインメニューのユーザー ![&#x200B; ユーザーアイコン &#x200B;](assets/users-icon-in-main-menu.png) を表示できます。

   * リクエスト
   * タイムシート
   * ドキュメント
   * テンプレート
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
     >計画には追加ライセンスが必要です。 Workfront計画について詳しくは、[Adobe Workfront計画の概要 &#x200B;](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

   * カスタムアプリケーション

     >[!NOTE]
     >
     > カスタムアプリケーションは、メインメニューオプションとして使用する前に、個別に作成する必要があります。 詳しくは、[Adobe App Builderを使用したWorkfrontのカスタムアプリケーションの作成 &#x200B;](/help/quicksilver/app-builder/app-builder.md) を参照してください。

1. 次のいずれかの操作を行います。

   * 表示しない ![&#x200B; 非表示アイコン &#x200B;](assets/remove-icon---x-in-circle.png)**アクティブな項目** を非表示にする
   * メインメニューに表示する ![&#x200B; アイコンを表示 &#x200B;](assets/add-icon-plus-in-circle.png)**利用可能な項目** を表示します。
   * ドラッグ ![&#x200B; ドラッグアイコン &#x200B;](assets/move-icon---dots.png)**アクティブなアイテム** を使用して、メインメニューの表示順序を変更できます。

1. 「**完了**」をクリックします。

   また、変更を破棄する場合は、いつでも「**キャンセル**」をクリックして変更を破棄できます。

1. <span class="preview"> プレビュー環境の場合：レイアウトテンプレートのカスタマイズを続行します。 「**適用**」をクリックすると、いつでも進捗を保存できます。</span>

   <span class="preview">または</span>

   <span class="preview"> カスタマイズが終了したら、「**保存して閉じる** をクリックします。</span>

1. 実稼動環境の場合：レイアウトテンプレートのカスタマイズを続行します。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「**保存**」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。

レイアウトテンプレートに関して詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。
