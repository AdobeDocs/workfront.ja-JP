---
title: ドキュメントに対するアクセス権の付与
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront でユーザーのドキュメントへのアクセスを定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '595'
ht-degree: 100%

---

# ドキュメントに対するアクセス権の付与

Adobe Workfront 管理者は、アクセスレベルを使用して、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)の説明に従って、ドキュメントに対するユーザーのアクセスを定義できます。

このアクセスは、ドキュメントフォルダーにも適用されます。

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
   <td> <p>Workfront 管理者である必要があります。&gt;.</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムアクセスレベルを使用したドキュメントへのユーザーアクセスの設定

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. ドキュメントの右の「**表示**」または「**編集**」ボタンの歯車アイコン ![](assets/gear-icon-settings.png) をクリックして、次に「**設定を微調整**」で付与する権限を選択します。

   ![document_access.png](assets/document-access.png)

   ユーザーがアクセス権のあるプロジェクト、タスクおよびイシューに関する次の作業を許可できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">作成</td> 
      <td>ドキュメントをアップロード</td> 
     </tr> 
     <tr> 
      <td role="rowheader">削除</td> 
      <td> <p>アップロードしたドキュメントを削除。</p> <p>このオプションが有効な場合、「<b>作成</b>」オプションは自動的に有効になります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共有</td> 
      <td>特定のユーザー、担当業務、チームとドキュメントを共有します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメントを公開して共有</td> 
      <td>ドキュメントを（Workfront ライセンスを持たない）外部ユーザーと共有します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">システム全体で共有</td> 
      <td> <p>ドキュメントを Workfront インスタンス内のすべてのユーザーが使用できるようにします。</p> <p>次の場合に、システム内の誰でもこの方法で共有されたドキュメントを表示できます。</p> 
       <ul> 
        <li> <p>アップロード先のドキュメントページへのリンクを送信。</p> </li> 
        <li> <p>Workfront で検索。</p> </li> 
       </ul> <p>このオプションが有効な場合、「<b>共有</b>」オプションは自動的に有効になります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >特定の種類のオブジェクトに対してアクセスレベルの設定を行う場合、その設定は、低いランクのオブジェクトに対するユーザーのアクセスには影響しません。例えば、ユーザーのアクセスレベルでプロジェクトの削除を制限できますが、プロジェクトよりも下位のドキュメントの削除は制限されません。オブジェクトの階層について詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の記事の[オブジェクトの相互依存性と階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)の節を参照してください。

1. （オプション）ドキュメントの継承された権限を上位のオブジェクトから制限するには、「**追加制限の設定**」を選択し、「**ドキュメントのアクセス権をプロジェクト、タスク、イシューなどから継承しない**」を選択します。
1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら、「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ライセンスタイプ別のドキュメントへのアクセス

各アクセスレベルのユーザーがドキュメントで実行できる操作について詳しくは、[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事の[ドキュメント](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document)の節を参照してください。

## 共有ドキュメントへのアクセス

ドキュメントを Workfront にアップロードした後、[ドキュメントの共有](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)の説明に従って、他のユーザーと共有するには、そのユーザーに権限を付与します。

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つ項目の組み合わせによって決まります。

* オブジェクトについて受信者に付与する権限
* オブジェクトのタイプについての受信者のアクセスレベル設定
