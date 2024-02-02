---
title: プログラムへのアクセス権の付与
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront でユーザーのプログラムへのアクセス権を定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '475'
ht-degree: 100%

---

# プログラムへのアクセス権の付与

Adobe Workfront 管理者は、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)で説明されるように、プロジェクトに対するユーザーのアクセス権を定義するために、アクセスレベルを使用できます。

カスタムアクセスレベルを使用して、Workfront の他のオブジェクトタイプへのユーザーのアクセスを管理する方法について詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

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
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムアクセスレベルを使用してプログラムへのユーザーのアクセス権を設定する

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. プログラムの右側にある「**表示**」ボタンまたは「**編集**」ボタンの歯車アイコン![](assets/gear-icon-settings.png) をクリックし、「**設定の微調整**」で許可する機能を選択します。

   各アクセスレベルのユーザーがプログラムに対して実行できる内容について詳しくは、[各オブジェクトタイプで利用可能な機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事の[プログラム](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs)の節を参照してください。

   >[!NOTE]
   >
   >特定の種類のオブジェクトに対してアクセスレベルの設定を行う場合、その設定は、低いランクのオブジェクトに対するユーザーのアクセスには影響しません。例えば、ユーザーのアクセスレベルでプログラムの削除を制限できますが、プログラムよりも下位のプロジェクトの削除は制限されません。オブジェクトの階層について詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の記事の[オブジェクトの相互依存性と階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)の節を参照してください。

1. （オプション）作業中のアクセスレベルの他のオブジェクトやエリアのアクセス設定を指定するには、[Adobe Workfront へのアクセスを設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)にある記事のうちの 1 つ（[タスクへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)、[財務データへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)など）に従って、作業を続けます。
1. 完了したら、「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザープロファイルを編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ライセンスタイプ別のプログラムへのアクセス権

各アクセスレベルのユーザーがプログラムに対して実行できる内容について詳しくは、[各オブジェクトタイプで利用可能な機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事の[プログラム](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs)の節を参照してください。

## 共有プログラムへのアクセス権

プログラムの所有者または作成者として、プログラムに対する権限を付与することで、[タスクを共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md)の説明に従って、他のユーザーと共有できます。

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
