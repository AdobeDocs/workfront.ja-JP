---
title: ユーザーへのアクセス権の付与
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront の他のユーザーに対するユーザーのアクセス権を定義できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: a22bff203680d2b59e14a9d705c963f2a1d3a80b
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 61%

---


# ユーザーへのアクセスを許可

Adobe Workfront 管理者は、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)の説明に従って、アクセスレベルを使用して、Workfront の他のユーザーに対するユーザーのアクセス権を定義できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーへのアクセスの設定

他のユーザーに関してユーザーが表示および編集できる情報は、デフォルトのアクセスレベルまたは作成したカスタムアクセスレベルを使用して管理できます。デフォルトの標準、プラン、および作業ライセンスを持つユーザーは、他のユーザーの連絡先情報を表示できます。 次のユーザーは誰でも、他のユーザーを作成および編集できます。

* Workfront 管理者。

  詳しくは、[ユーザーに完全な管理アクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)を参照してください。

* この記事で説明されているように、デフォルトの標準またはプランのライセンスを持つユーザー。ユーザーにもアクセスできます。

  自社またはプライマリ会社のユーザーのみの表示に制限されているユーザーは、表示できるユーザーのみを編集するアクセス権を持っています。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* デフォルトの標準ライセンスまたはプランライセンスを持つユーザー。別のユーザーのマネージャーとしても指定されます。

  自分のアクセスレベルのユーザーに対して編集アクセス権を付与されたユーザーは、直属の部下であるユーザーを管理できます。ユーザーの管理について詳しくは、[組織図を表示する](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)を参照してください。

* ユーザーを作成したデフォルトの標準またはプランのライセンスを持つユーザーは、作成したユーザーを非アクティブ化、削除、または編集できます。 新しいユーザーの作成について詳しくは、[ユーザーの追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

## カスタムのアクセスレベルを使用して、ユーザーを編集するユーザーのアクセス権を設定

1. アクセスレベルの作成または編集を行います。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
1. 標準、プラン、または作業ライセンスを持つユーザーの機能を変更して、他のユーザーの情報を表示するには、![ ユーザー](assets/gear-icon-settings.png)の右側にある&#x200B;**表示** ボタンの歯車アイコン **をクリックし、**&#x200B;設定を微調整&#x200B;**ボックスで付与する表示オプションを選択します。**

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>請求率を表示</strong> </td> 
      <td> ユーザーがユーザープロファイルの請求レートを表示できるようにします。</td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>連絡先情報を表示</strong> </td> 
      <td> 他のユーザーのユーザー詳細ページを表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> コスト率を表示</strong> </td> 
      <td> ユーザーがユーザープロファイルのコスト率を表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>財務の表示</strong> </td> 
      <td> ユーザーがユーザープロファイルの一般的な財務フィールド（請求またはコスト率に関連しない）を表示できるようにします。</td>
     </tr> 
    </tbody> 
   </table>

   ![ ユーザー設定の表示を微調整](assets/fine-tune-view-users.png)

1. 標準またはプランのライセンスを持つユーザーの権限を変更して他のユーザーを編集するには、![ ユーザー](assets/gear-icon-settings.png)の右側にある&#x200B;**編集** ボタンの歯車アイコン **歯車アイコン**&#x200B;をクリックし、**設定を微調整** ボックスで付与する編集オプションを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>作成</strong> </td> 
      <td> <p>ユーザーがユーザーを作成できるようにします。<br>このオプションは、デフォルトで有効になっています。</p> 
     <p><b>メモ</b>：組織が Adobe Admin Console にオンボーディングされている場合は、これは使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。<!--Check this October 2026--></p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>削除</strong> </td> 
      <td> <p> ユーザーが自分で作成したユーザーを削除できるようにします。<br>このオプションは、デフォルトで有効になっています。</p> <p><b>メモ</b>：組織が Adobe Admin Console にオンボーディングされている場合は、これは使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。<!--Check this October 2026--></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>請求率の編集</strong> </td> 
      <td> ユーザーがユーザープロファイルの請求レートを編集できるようにします。</td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong> コストレートを編集</strong> </td> 
      <td> ユーザーがユーザープロファイルのコスト率を編集できるようにします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>財務の編集</strong> </td> 
      <td> ユーザーがユーザープロファイルの一般的な財務フィールド（請求またはコスト率に関連しない）を編集できるようにします。</td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザー管理者（すべてのユーザー）</strong> </td> 
      <td> <p>Workfront の任意のユーザーに対して、次の操作を実行できます。</p> 
       <ul> 
        <li>ユーザーを編集、削除、または非アクティブ化</li> 
        <li>ユーザーとしてログイン<p><b> メモ </b>: システム管理者であるユーザーはログインできません。</p></li> 
        <li>ユーザーのパスワードをリセット</li> 
       </ul> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザー管理者（グループユーザー）</strong> </td> 
      <td> <p>ユーザーは、管理するグループ内のすべてのユーザーに対して、次の操作を実行できます。 
        <ul>
         <li><p>ユーザーを編集、削除、または非アクティブ化</p></li>
         <li>ユーザーとしてログイン</li>
         <li><p>ユーザーのパスワードをリセット</p><p><b>メモ</b>：グループ管理者は、Workfront 管理者としてログインしたり、パスワードをリセットしたりすることはできません。</p></li>
        </ul><p>このオプションはデフォルトでは無効になっています。</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>請求率を表示</strong> </td> 
      <td> ユーザーがユーザープロファイルの請求レートを表示できるようにします。</td>  
     </tr>
     <tr> 
      <td role="rowheader"><strong> コスト率を表示</strong> </td> 
      <td> ユーザーがユーザープロファイルのコスト率を表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>財務の表示</strong> </td> 
      <td> ユーザーがユーザープロファイルの一般的な財務フィールド（請求またはコスト率に関連しない）を表示できるようにします。</td>
     </tr>
    </tbody> 
   </table>

   >[!TIP]
   >
   >グループ管理者に、管理するグループのすべてのメンバーへのアクセス権を付与しない場合は、上記の「ユーザー管理者」オプションの両方を無効にします。グループ管理者は、引き続き、Workfront に追加したグループメンバーや、Workfront でレポートするグループメンバーにアクセスできます。

1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら、「**保存**」をクリックします。

## ライセンスタイプ別のユーザーへのアクセス

各アクセスレベルのユーザーがユーザーに対して実行できる操作について詳しくは、[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)記事内「[ユーザー](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users)」の節を参照してください。
