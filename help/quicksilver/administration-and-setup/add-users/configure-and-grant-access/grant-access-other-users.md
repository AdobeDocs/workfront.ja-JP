---
title: ユーザーへのアクセス権の付与
description: Adobe Workfront管理者は、アクセスレベルを使用して、Workfrontで他のユーザーに対するユーザーのアクセスを定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d1fe7165932fb6f2aff3c8488bdb8e1dfae3b6d3
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# ユーザーへのアクセス権の付与

Adobe Workfront管理者は、Workfrontでユーザーの他のユーザーへのアクセスを定義するために、アクセスレベルを使用できます。詳しくは、 [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーへのアクセスの設定

ユーザーが表示および編集できる情報は、作成したデフォルトのアクセスレベルまたはカスタムアクセスレベルを使用して、他のユーザーに対して管理できます。 デフォルトのプランおよび作業用ライセンスを持つユーザーは、他のユーザーの連絡先情報を表示できます。 次のユーザーは、他のユーザーを作成および編集できます。

* Workfront管理者。

   詳しくは、 [ユーザーに完全な管理アクセス権を付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* デフォルトのプランライセンスを持つユーザーで、この記事で説明するユーザーにもアクセスできます。

   会社または主な会社のユーザーのみを表示するように制限されているユーザーは、表示できるユーザーのみを編集する権限を持っています。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 別のユーザーの管理者として指定された、既定のプランライセンスを持つユーザー。

   アクセスレベルでユーザーに対して「編集」アクセス権を付与されたユーザーは、自分に対してレポートを作成するユーザーを管理できます。 ユーザーの管理について詳しくは、 [組織図を表示](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* ユーザを作成した既定のプランライセンスを持つユーザは、作成したユーザを非アクティブ化、削除、または編集できます。 新しいユーザーの作成について詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## カスタムアクセスレベルを使用してユーザーのアクセスを設定し、ユーザーを編集します

1. アクセスレベルの作成または編集を開始します ( [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. プランまたは作業用ライセンスを持つユーザーの能力を変更して、他のユーザーのプロファイルを表示するには、次の手順に従います。

   1. 歯車アイコンをクリックします。 ![](assets/gear-icon-settings.png) の **表示** 右のボタン **ユーザー**.

   1. 無効にする **連絡先情報の表示**」、「 X 」の順にクリックして、 **設定を微調整する** ボックス

1. プランライセンスのアクセス権を持つユーザーの能力を変更して他のユーザーを編集するには、歯車アイコンをクリックします ![](assets/gear-icon-settings.png) の **編集** 右のボタン **ユーザー**&#x200B;を選択し、許可するアビリティを次の中から選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>作成</strong> </td> 
      <td> <p>ユーザーがユーザーを作成できるようにします。<br>このオプションは、デフォルトで有効になっています。</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">この変更が行われていることを確認してから、これらの 2 つの注記の下書きを解除してください。 3/29では、req doc は、これが調査結果に依存すると述べています。</p>

       &lt;p>&lt;b>注意&lt;/b>:組織がAdobe Admin Consoleにオンボーディングされている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>削除</strong> </td> 
      <td> <p> ユーザーが自分で作成したユーザーを削除できるようにします。<br>このオプションは、デフォルトで有効になっています。</p> <p><b>注意</b>:組織がAdobe Admin Consoleにオンボーディングされている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザー管理者 (すべてのユーザー)</strong> </td> 
      <td> <p>Workfrontの任意のユーザーに対して、次の操作を実行できます。</p> 
       <ul> 
        <li>ユーザーを編集、削除、または非アクティブ化する</li> 
        <li>ユーザーとしてログイン</li> 
        <li>ユーザーのパスワードをリセット</li> 
       </ul> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザー管理者 (グループ ユーザー)</strong> </td> 
      <td> <p>管理するグループ内のすべてのユーザーに対して、次の操作を実行できます。 
        <ul>
         <li><p>ユーザーを編集、削除、または非アクティブ化する</p></li>
         <li>ユーザーとしてログイン</li>
         <li><p>ユーザーのパスワードをリセット</p><p><b>注意</b>:グループ管理者は、Workfront管理者のパスワードとしてログインしたり、リセットしたりすることはできません。</p></li>
        </ul><p>このオプションはデフォルトでは無効になっています。</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >グループ管理者に、管理するグループのすべてのメンバーへのアクセス権を付与しない場合は、上記の「ユーザー管理者」オプションを両方とも無効にします。 グループ管理者は、引き続き、Workfrontに追加したグループメンバーや、Workfrontでレポートするグループメンバーにアクセスできます。

1. （オプション）作業中のアクセスレベルの他のオブジェクトや領域のアクセス設定を構成するには、 [Adobe Workfrontへのアクセスの設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)例： [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) および [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完了したら、「 **保存**.

## ライセンスタイプ別のユーザーへのアクセス

各アクセスレベルのユーザーがユーザーに対して実行できる操作について詳しくは、「 [ユーザー](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) 記事内 [各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
