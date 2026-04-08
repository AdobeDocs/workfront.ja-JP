---
title: グループへのアクセス権の付与
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront のチームへのユーザーのアクセス権を定義できます
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: 627d59c8c8296e5b6c8b6da53705a1c3d7633751
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 93%

---

# チームに対するアクセスの許可

Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront のチームへのユーザーのアクセス権を定義できます。詳しくは、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)を参照してください。

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

## カスタムアクセスレベルを使用して、チームを編集するためのユーザーのアクセス権を設定します

1. アクセスレベルの作成または編集を行います。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
1. 「チーム」の右側にある&#x200B;**表示**&#x200B;ボタンまたは&#x200B;**編集**&#x200B;ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) をクリックし、付与する権限を&#x200B;**設定を微調整する**&#x200B;で選択します。

   ![ チームを微調整](assets/fine-tune-teams.png)

   * **表示**：任意のライセンスを持つユーザーがチームを表示する方法を設定する場合は、次のオプションを変更します。

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">自分のグループと関連付けられたチームを確認する</td>
         <td>
          <p><b>有効</b>：ユーザーが「チーム」先行入力フィールドでチームを探すと、自分がチームメンバーであるかどうかに関係なく、グループに関連付けられたチームが表示されます。 </p>
          <p><b>無効</b>：ユーザーが「チーム」先行入力フィールドでチームを探すと、自分がチームメンバーである場合にのみ、グループに関連付けられたチームが表示されます。</p><p>このオプションは、デフォルトで有効になっています。</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">すべてのチームを表示</td>
         <td><p>このオプションを有効にし、ユーザーが「チーム」先行入力フィールドでチームを探すと、ユーザーは任意のチームを表示して選択できます。</p><p>このオプションは、デフォルトで有効になっています。 </p></td>
        </tr>
       </tbody>
      </table>

   * **編集**：Plan ライセンスおよび Work ライセンスを持つユーザーがチームを管理する方法を設定する場合は、次のオプションを変更します。

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">作成</td>
         <td><p>Plan ライセンスまたは Work ライセンスを持つユーザーがチームを作成できます。</p><p>このオプションは、デフォルトで有効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">削除</td>
         <td><p> Plan ライセンスを持つユーザーが、編集するアクセス権のあるチームを削除できます（Work ライセンスを持つユーザーは使用できません）。</p><p>このオプションは、デフォルトで有効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">自分が管理するグループのチームを編集する（グループ管理者のみ）</td>
         <td><p>グループ管理者として指定された Plan ライセンスユーザーが、管理するグループに関連付けられたチームを編集できます。</p><p>このオプションは、デフォルトで有効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">自分の所属するチームを編集</td>
         <td><p>Plan ライセンスまたは Work ライセンスを持つユーザーは、自分がメンバーであるチームを編集できます。</p><p>このオプションはデフォルトでは無効になっています。</p></td>
        </tr>
        <tr>
         <td role="rowheader">自分のグループと関連付けられたチームを確認する</td>
         <td>
         <p><b>有効</b>：ユーザーが「チーム」先行入力フィールドでチームを探すと、自分がチームメンバーであるかどうかに関係なく、グループに関連付けられたチームが表示されます。 </p>
         <p><b>無効</b>：ユーザーが「チーム」先行入力フィールドでチームを探すと、自分がチームメンバーである場合にのみ、グループに関連付けられたチームが表示されます。</p><p>このオプションは、デフォルトで有効になっています。</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">すべてのチームを表示</td>
         <td><p>このオプションを有効にし、ユーザーが「チーム」先行入力フィールドでチームを探すと、ユーザーは任意のチームを表示して選択できます。</p><p>このオプションは、デフォルトで有効になっています。 </p></td>
        </tr>
       </tbody>
      </table>



1. 「X」をクリックして「**設定を微調整する**」ボックスを閉じます。
1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら、「**保存**」をクリックします。

>[!NOTE]
>
>* アクセスレベルの設定に関係なく、次のことが当てはまります。
>
>   * チームの所有者は、常に自分のチームを表示および編集できます
>   * ユーザーは、常に自分のチームを表示できます
>
>* 表示と編集の両方で使用できるオプション（「自分のグループに関連付けられたチームの表示」など）の設定は、アクセスレベルで「表示」ではなく「編集」（または「編集」ではなく「表示」）を選択した場合も保持されます。
>

## ライセンスタイプ別のチームへのアクセス権

各アクセスレベルのユーザーがチームで実行できる処理について詳しくは、記事[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams)のTeams[の節を参照してください。](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)
