---
title: デフォルトのAdobe Workfrontレイアウトについて
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: デフォルトのレイアウトは、Adobe Workfront管理者がレイアウトテンプレートを使用して変更をおこなう前に、メインメニュー、左側のパネル、ビュー、グループ化およびフィルターが配置されたものです。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 14%

---

# デフォルトのAdobe Workfrontレイアウトについて

デフォルトのレイアウトは、メインメニューの配置です ![](assets/main-menu-icon.png)、 Adobe Workfront管理者がレイアウトテンプレートを使用して変更をおこなう前に、左側のパネルと、ビュー、グループ化、フィルターを使用しておこないます。

Workfront管理者がユーザーにレイアウトテンプレートを割り当ててユーザーのデフォルトレイアウトを変更する方法について詳しくは、 [レイアウトテンプレートにユーザーを割り当てる](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>ユーザーは、ユーザープロファイルの環境設定を編集することで、自分のレイアウトを変更できます。 詳しくは、 [環境設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences) セクション [設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## 各アクセスレベルのデフォルトレイアウト

各ユーザーのデフォルトのレイアウトは、アクセスレベルに応じて異なります。 割り当てられているアクセスレベルによっては、メインメニューまたは特定の左側のパネル項目に特定の領域が表示されない場合があります。

次の表に、デフォルトで各アクセスレベルに対して左側のパネル項目が表示される内容を示します。 各アクセスレベルのデフォルトのランディング領域も示されます。

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
   <th> 左のパネル項目 </th> 
   <th> <p>システム管理者</p> </th> 
   <th> <p>計画担当者</p> </th> 
   <th>作業者</th> 
   <th>レビュアー</th> 
   <th>要求者</th> 
   <th>外部ユーザー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>プロジェクト</strong> </td> 
   <td><strong>プロジェクト</strong> </td> 
   <td>✔ <br>（デフォルトのランディング領域）</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>（デフォルトのランディング領域）</td> 
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
   <td rowspan="3"><strong>報告書</strong> </td> 
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
   <td rowspan="5"><strong>人</strong> ( に名前を変更 <strong>チーム</strong> （作業ライセンスを持つユーザー向け）</td> 
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
   <td rowspan="3"><strong>リクエスト</strong> </td> 
   <td><strong>新しい要求</strong> </td> 
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
   <td>✔ <br>（デフォルトのランディング領域）</td> 
   <td>✔ <br>（デフォルトのランディング領域）</td> 
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
   <td>限られた機能</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
