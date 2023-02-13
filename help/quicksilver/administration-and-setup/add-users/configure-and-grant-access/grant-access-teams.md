---
title: チームへのアクセス権の付与
description: Adobe Workfront管理者は、アクセスレベルを使用して、Workfrontでユーザーのチームへのアクセスを定義できます
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 4%

---

# チームへのアクセス権の付与

Adobe Workfront管理者は、アクセスレベルを使用して、Workfrontでユーザーのチームへのアクセスを定義できます。詳しくは、 [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## カスタムアクセスレベルを使用してユーザーのアクセスを設定し、ユーザーを編集します

1. アクセスレベルの作成または編集を開始します ( [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 歯車アイコンをクリックします。 ![](assets/gear-icon-settings.png) の **表示** または **編集** 「チーム」の右側のボタンをクリックし、 **設定を微調整する**.

   * **表示**:ライセンスを持つユーザーがチームを表示する方法を設定する場合は、次のオプションを変更します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">自分のグループと関連付けられたチームを確認する</td>
         <td>
          <p><b>有効</b>:[ チームの先行入力 ] フィールドでチームを探すと、チームメンバーかどうかに関係なく、グループに関連付けられたチームを確認できます。 </p>
          <p><b>無効</b>:[ チームの先行入力 ] フィールドでチームを探すと、グループに関連付けられたチームは、チームメンバーの場所でのみ表示されます</p><p>このオプションは、デフォルトで有効になっています。</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">すべてのチームを表示</td>
         <td><p>このオプションを有効にし、ユーザーがチーム先行入力フィールドでチームを探す場合、ユーザーは任意のチームを表示して選択できます。</p><p>このオプションは、デフォルトで有効になっています。 </p></td>
        </tr>
       </tbody>
      </table>

   * **編集**:プランライセンスとワークライセンスを持つユーザがチームを管理する方法を設定する場合は、次のオプションを変更します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">作成</td>
         <td><p>プランライセンスまたは作業用ライセンスを持つユーザーがチームを作成することを許可します。</p><p>このオプションは、デフォルトで有効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">削除</td>
         <td><p> プランライセンスを持つユーザーが、編集するアクセス権のあるチームを削除できるようにします（作業ライセンスを持つユーザーは使用できません）。</p><p>このオプションは、デフォルトで有効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">自分が管理するグループのチームを編集する (グループ管理者のみ)</td>
         <td><p>グループ管理者として指定された Plan ライセンスユーザが、管理するグループに関連付けられたチームを編集できるようにします。</p><p>このオプションは、デフォルトで有効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">自分の所属するチームを編集</td>
         <td><p>ユーザーがライセンスまたは作業ライセンスを計画して、自分がメンバーとなっているチームを編集することを許可します。</p><p>このオプションはデフォルトでは無効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">自分のグループと関連付けられたチームを確認する</td>
         <td>
         <p><b>有効</b> [ チームの先行入力 ] フィールドでチームを探すと、チームメンバーかどうかに関係なく、グループに関連付けられたチームを確認できます。 </p>
         <p><b>無効</b>:[ チームの先行入力 ] フィールドでチームを探すと、グループに関連付けられたチームは、チームメンバーの場所でのみ表示されます</p><p>このオプションは、デフォルトで有効になっています。</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">すべてのチームを表示</td>
         <td><p>このオプションを有効にし、ユーザーがチーム先行入力フィールドでチームを探す場合、ユーザーは任意のチームを表示して選択できます。</p><p>このオプションは、デフォルトで有効になっています。 </p></td>
        </tr>
       </tbody>
      </table>

1. 「 X 」をクリックして「 」を閉じます。 **設定を微調整する** ボックス
1. （オプション）作業中のアクセスレベルの他のオブジェクトや領域のアクセス設定を構成するには、 [Adobe Workfrontへのアクセスの設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)例： [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) および [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完了したら、「 **保存**.

>[!NOTE]
>
>* アクセスレベルの設定に関係なく、次のことが当てはまります。
   >
   >   * チームの所有者は、常にチームを表示および編集できます
   >   * ユーザーは常に自分のチームを表示するアクセス権を持っています
>
* 表示と編集の両方で使用可能なオプション（「自分のグループに関連付けられたチームの表示」など）の設定は、アクセスレベルで「表示」の代わりに「編集」または「編集」を選択した場合も保持されます。
>


## ライセンスタイプ別のチームへのアクセス

各アクセスレベルのユーザーが問題に対してどのような処理を行うかについては、「 [チーム](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) 記事内 [各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
