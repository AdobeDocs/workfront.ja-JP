---
title: ユーザーへのアクセスを許可
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront の他のユーザーに対するユーザーのアクセス権を定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: ht
source-wordcount: '768'
ht-degree: 100%

---


# ユーザーへのアクセスを許可

Adobe Workfront 管理者は、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)の説明に従って、アクセスレベルを使用して、Workfront の他のユーザーに対するユーザーのアクセス権を定義できます。

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
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーへのアクセスの設定

他のユーザーに関してユーザーが表示および編集できる情報は、デフォルトのアクセスレベルまたは作成したカスタムアクセスレベルを使用して管理できます。デフォルトのプランライセンスおよびワークライセンスを持つユーザーは、他のユーザーの連絡先情報を表示できます。次のユーザーは誰でも、他のユーザーを作成および編集できます。

* Workfront 管理者。

  詳しくは、[ユーザーに完全な管理アクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)を参照してください。

* デフォルトのプランライセンスを持ち、この記事で説明するユーザーに対するアクセス権も持つユーザー。

  自社またはプライマリ会社のユーザーのみの表示に制限されているユーザーは、表示できるユーザーのみを編集するアクセス権を持っています。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* デフォルトのプランライセンスを持ち、別のユーザーの管理者としても指定されているユーザー。

  自分のアクセスレベルのユーザーに対して編集アクセス権を付与されたユーザーは、直属の部下であるユーザーを管理できます。ユーザーの管理について詳しくは、[組織図を表示する](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)を参照してください。

* ユーザーを作成した、デフォルトのプランライセンスを持つユーザーは、作成したユーザーを非アクティブ化、削除または編集できます。新しいユーザーの作成について詳しくは、[ユーザーの追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

## カスタムのアクセスレベルを使用して、ユーザーを編集するユーザーのアクセス権を設定

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. プランライセンスまたはワークライセンスを持つユーザーの権限を、他のユーザーのプロファイルを表示できるように変更するには：

   1. 歯車アイコンをクリックします。「**ユーザー**」の右側にある&#x200B;**表示**&#x200B;ボタンで歯車アイコン ![](assets/gear-icon-settings.png) をクリックします。

   1. 「**連絡情報の表示**」を無効にし、「X」をクリックして、「**設定の微調整**」ボックスを閉じます。

1. 他のユーザーを編集するプランライセンスのアクセス権を持つユーザーの権限を変更するには、「**ユーザー**」の右側にある&#x200B;**編集**&#x200B;ボタン上の歯車アイコン ![](assets/gear-icon-settings.png) をクリックし、付与する権限を次の中から選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>作成</strong> </td> 
      <td> <p>ユーザーがユーザーを作成できるようにします。<br>このオプションは、デフォルトで有効になっています。</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">この変更が行われていることを確認してから、これら 2 つの注釈のドラフト指定を解除してください。3/29 では、req doc は、これが調査結果に依存すると述べています。</p>

       &lt;p>&lt;b>メモ&lt;/b>：組織が Adobe Admin Console にオンボーディングされている場合は、これは使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>削除</strong> </td> 
      <td> <p> ユーザーが自分で作成したユーザーを削除できるようにします。<br>このオプションは、デフォルトで有効になっています。</p> <p><b>メモ</b>：組織が Adobe Admin Console にオンボーディングされている場合は、これは使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザー管理者（すべてのユーザー）</strong> </td> 
      <td> <p>Workfront の任意のユーザーに対して、次の操作を実行できます。</p> 
       <ul> 
        <li>ユーザーを編集、削除、または非アクティブ化</li> 
        <li>ユーザーとしてログイン</li> 
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
    </tbody> 
   </table>

   >[!TIP]
   >
   >グループ管理者に、管理するグループのすべてのメンバーへのアクセス権を付与しない場合は、上記の「ユーザー管理者」オプションの両方を無効にします。グループ管理者は、引き続き、Workfront に追加したグループメンバーや、Workfront でレポートするグループメンバーにアクセスできます。

1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら、「**保存**」をクリックします。

## ライセンスタイプ別のユーザーへのアクセス

各アクセスレベルのユーザーがユーザーに対して実行できる操作について詳しくは、[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)記事内「[ユーザー](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users)」の節を参照してください。
