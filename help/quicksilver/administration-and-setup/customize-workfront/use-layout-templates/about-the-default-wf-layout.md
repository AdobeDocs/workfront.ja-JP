---
title: デフォルトのAdobe Workfrontのレイアウトについて
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: デフォルトのレイアウトでは、Adobe Workfront 管理者がレイアウトテンプレートを使用して変更を行う前に、メインメニュー、左側のパネル、表示、グループ化およびフィルターが配置されています。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 78%

---

# デフォルトの Adobe Workfront レイアウトについて

デフォルトのレイアウトは、Adobe Workfront管理者がレイアウトテンプレートを使用して変更を加える前に、メインメニュー ![](assets/main-menu-icon.png) またはメインメニュー ![](assets/lines-main-menu.png) （使用可能な場合）の左側のパネル、ビュー、グループ化およびフィルターを配置することです。

Workfront 管理者がユーザーにレイアウトテンプレートを割り当ててユーザーのデフォルトレイアウトを変更する方法について詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

>[!NOTE]
>
>ユーザーは、ユーザープロファイルの環境設定を編集することで、自分のレイアウトを変更できます。詳しくは、[個人設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)の[環境設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences)の節を参照してください。

## 各アクセスレベルのデフォルトレイアウト

各ユーザーのデフォルトのレイアウトは、アクセスレベルに応じて異なります。割り当てられているアクセスレベルによっては、メインメニューまたは特定の左側のパネル項目に特定の領域が表示されない場合があります。

次の表に、デフォルトのランディング領域と、各アクセスレベルに表示される左側のパネル項目を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>エリア</th> 
   <th> 左側のパネル項目 </th> 
   <th> システム管理者</th> 
   <th> プランナー </th> 
   <th>作業者</th> 
   <th>レビュアー</th> 
   <th>依頼者</th> 
   <th>外部ユーザー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>プロジェクト</strong> </td> 
   <td><strong>プロジェクト</strong> </td> 
   <td>✔<br>（デフォルトのランディング領域）</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br> （デフォルトのランディングエリア）</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>ポートフォリオ</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>レポート</strong> </td> 
   <td><strong>レポート</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ダッシュボード</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>カレンダー</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>ユーザー</strong>（ワークライセンスを持つユーザーの場合は<strong>チーム</strong>に名前を変更）</td> 
   <td><strong>チーム</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>ユーザー</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> <!--
   <tr> 
    <td><strong>Legacy Resource Planning</strong> </td> 
    <td>✔ </td> 
    <td>✔ </td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
   </tr>
  --> 
  <tr> 
   <td><strong>計画</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>スケジュール</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>要求</strong> </td> 
   <td>新しいリクエスト </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>送信済みの要求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>（デフォルトのランディングエリア）</td> 
   <td>✔ <br>（デフォルトのランディングエリア）</td> 
  </tr> 
  <tr> 
   <td><strong>すべての要求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>タイムシート</strong> </td> 
   <td><strong>マイタイムシート</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>承認するタイムシート</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>すべてのタイムシート</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>ドキュメント</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>設定</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>機能制限付き</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
