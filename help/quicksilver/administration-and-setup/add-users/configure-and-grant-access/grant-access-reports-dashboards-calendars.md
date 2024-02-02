---
title: レポート、ダッシュボード、カレンダーへのアクセスを許可
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront のレポート、ダッシュボードおよびカレンダーに対するユーザーのアクセス権を定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: ht
source-wordcount: '602'
ht-degree: 100%

---

# レポート、ダッシュボード、カレンダーへのアクセスを許可

Adobe Workfront 管理者は、アクセスレベルを使用して、レポート、ダッシュボードおよびカレンダーに対するユーザーのアクセス権を定義できます。詳しくは[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)を参照してください。

このアクセス権には、外部ページに対するアクセス権も含まれます。外部ページについて詳しくは、[財務データに対するアクセスを許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

>[!NOTE]
>
>* レポート、ダッシュボード、カレンダーへのアクセス権をユーザーに付与する場合は、そのユーザーにフィルター、ビュー、グループへのアクセス権も付与する必要があります。手順については、[フィルター、ビューおよびグループへのアクセスを許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)を参照してください。
>* あるユーザーが別のユーザーとレポート、ダッシュボードまたはカレンダーを共有する場合、受信者の権限は、レポート、ダッシュボードおよびカレンダーに対する受信者のアクセスレベル設定、_および_&#x200B;共有者がレポート、ダッシュボードまたはカレンダーに対して付与した権限の 2 つの組み合わせによって決まります。
>
>レポート、ダッシュボード、カレンダーの共有時に付与できる権限について詳しくは、[レポート、ダッシュボード、カレンダーを共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)を参照してください。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセスできない場合は、Workfront 管理者に問い合わせて、アクセスレベルに制限が追加されていないか確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムのアクセスレベルを使用して、レポート、ダッシュボード、およびカレンダーへのユーザーアクセスを設定する

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. または「レポート」の右側にある「**表示**」または「**編集**」ボタンの歯車アイコン ![](assets/gear-icon-settings.png) をクリックしてから、「**設定の微調整**」で許可する操作を選択します。

   ![reports_access.png](assets/reports-access.png)

   次のオプションは、デフォルトで有効になっています。

   * **作成**
   * **削除**
   * **組み込みレポートの表示**：Workfront が作成したレポートを表示するには、このオプションを選択する必要があります。
   * **共有**
   * **レポートをパブリックにして共有**：レポートへの公開リンクを Workfront アカウントを持たないユーザーと共有することで、レポートを公開できます。このレベルの共有を許可するには、このオプションを選択する必要があります。
   * **システム全体で共有**：レポートは、Workfront ライセンスを持つシステム内のすべてのユーザーと共有できます。このレベルの共有を許可するには、このオプションを選択する必要があります。

     レポート、ダッシュボード、カレンダーの共有について詳しくは、[レポート、ダッシュボード、カレンダーを共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)を参照してください。

1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら、「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ライセンスタイプ別のレポート、ダッシュボード、カレンダーへのアクセス

各アクセスレベルのユーザーがイシューに対してできる対応について詳しくは、[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事の[レポート](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports)の項を参照してください。

## 共有レポート、ダッシュボード、カレンダーへのアクセス

レポート、ダッシュボード、カレンダーの所有者または作成者として、他のユーザーに権限を付与することで、レポート、ダッシュボードまたはカレンダーを他のユーザーと共有できます。詳しくは、[レポート、ダッシュボード、カレンダーの共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つ項目の組み合わせによって決まります。

* オブジェクトについて受信者に付与する権限
* オブジェクトのタイプについての受信者のアクセスレベル設定
