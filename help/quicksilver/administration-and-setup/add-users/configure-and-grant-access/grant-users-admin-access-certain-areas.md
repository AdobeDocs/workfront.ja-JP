---
title: 特定の領域に対する管理者アクセス権をユーザーに付与する
description: Adobe Workfront管理者は、アクセスレベルを使用して、プランライセンスを持つユーザーに、システムの特定の領域への管理アクセス権を付与できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# 特定の領域に対する管理者アクセス権をユーザーに付与する

<!--Linked in several places, do not rename or change URL.-->

Adobe Workfront管理者は、アクセスレベルを使用して、プランライセンスを持つユーザーに、システムの特定の領域への管理アクセス権を付与できます。

>[!NOTE]
>
>これは、ユーザーにWorkfrontへの完全な管理アクセス権を付与するのとは異なります。詳しくは、 [ユーザーに完全な管理アクセス権を付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md). &#x200B;

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

## Workfrontの特定の領域に管理者アクセス権を付与するプラン

>[!IMPORTANT]
>
>ユーザーを設定した後で参照できるように、組み込みのアクセスレベルを変更しないことを強くお勧めします。 アクセスレベルをカスタマイズするには、デフォルトのアクセスレベルをコピーし、コピーを変更します。 （システム管理者と外部ユーザーを除くすべてのアクセスレベルに対してこれを実行できます）。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **アクセスレベル**.
1. Workfrontの特定の領域に対する管理者アクセス権をユーザーに付与するために使用するアクセスレベルの名前をクリックします。
1. 内 **次の管理アクセスを許可：** 」セクションの「 」チェックボックスをオンにして、必要な管理アクセス権を付与します。

   これらのオプションを使用すると、次の機能を付与できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td><p>システム全体および特定のグループで使用する承認プロセスを作成および管理します。</p><p>このアクセス権がない場合、ユーザーは管理するアクセス権を持つ品目に対してアドホック承認プロセスのみを作成できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">会社</td> 
      <td><p>Workfrontでの新しい会社の追加と既存の会社の編集</p>
      <p>このアクセス権がない場合、ユーザーは既存の会社のみを表示できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td><p>グループ内でカスタムフォームを作成し、編集（フィールドの追加、編集、削除）します。</p><p>このアクセス権がない場合、ユーザーは、投稿や管理のアクセス権を持つオブジェクトに対してのみ、既存のフォームを添付できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">為替レート</td> 
      <td> <p>Workfrontに新しい通貨を追加します。</p> <p>このアクセス権がない場合、ユーザーは作成するプロジェクトに既存の通貨のみ追加できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td><p>Workfrontのオブジェクトに関するすべての費用を表示します。</p><p>この場合、ユーザーは新しい費用タイプを作成できません。</p><p>このアクセス権がない場合、ユーザーは次の項目のみを表示できます。</p>
       <ul>
        <li>管理するプロジェクト、タスクまたは問題に関する費用</li>
        <li>自費</li>
        <li>部下の費用</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">担当業務</td> 
      <td> <p>このアクセス権を持つユーザーは、次の操作を実行できます。</p> 
       <ul> 
        <li>既存のジョブの役割の表示と編集</li> 
        <li>新しいジョブの役割を追加</li> 
        <li>ロールの請求とコスト率を編集</li> 
       </ul> <p><b>重要</b>:プランナ・ユーザー管理アクセス権をジョブ・ロールに付与すると、「財務データ・アクセス」設定の「ロールの編集」「請求および原価率」がユーザーに対して自動的に有効になります。 後で、プランナ・ユーザーのジョブ・ロールへの管理アクセスを無効にした場合、「ロールの請求と原価率の編集」設定が有効なままなので、ジョブ・ロールはユーザーに対して表示されます。 これが発生し、ジョブの役割を表示するためにユーザーのアクセス権を削除する必要がある場合は、ユーザーの役割の請求とコスト率の編集権限設定を無効にする必要があります。 手順については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">マイ グループのマイルストーン</td> 
      <td>[ セットアップ ] の [ マイルストーンのパス ] メニューで、システム内のすべてのマイルストーンのパスを表示します。 ユーザーは、任意のグループに属するマイルストーンパスを編集または削除することもできます。 ユーザーは、どのグループにも割り当てられていないマイルストーンパスを管理（編集または削除）できません。<br><p>このアクセス権がない場合、ユーザーは既存のマイルストーンパスを表示し、アクセス権を持つ管理プロジェクトに適用することができます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダ通知</td> 
      <td>Workfrontでリマインダー通知を作成および管理します。<br>このアクセス権がない場合、ユーザーは通知の受信と表示に制限されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートと時間</td> 
      <td> <p>ユーザーがWorkfrontですべての時間とタイムシートを表示できるようにします。</p> <p>このオプションを無効にした場合、ユーザーは次の時間のみ表示できます：</p> 
       <ul> 
        <li>管理するプロジェクト、タスクまたは問題</li> 
        <li>自分のタイムシート</li> 
        <li>自分に報告する人のタイムシート</li> 
        <li>承認したタイムシート</li> 
       </ul> <p><b>メモ</b>:  <p>このオプションを有効にするか無効にするかに関わらず、グループ管理者は管理するグループとサブグループのタイムシートプロファイルを作成し、編集にアクセスできるユーザープロファイルを持つグループメンバに割り当てることができます。</p> <p>このオプションを有効にすると、管理するグループのユーザーだけでなく、システム内のすべてのユーザーのタイムシートプロファイル（および時間）によって生成されたタイムシートを表示できるので、一部のグループ管理者はアクセスできなくなります。 これほどアクセス権を必要としないグループ管理者に対しては、このオプションを無効にできます。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 完了したら、「 **保存**.
1. ユーザーに新しいアクセスレベルを割り当てます。詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >ユーザーに対する管理者アクセスを許可できます。 ユーザーがユーザーアカウントを管理できるように、ユーザーに管理者アクセス権を付与する方法について詳しくは、 [ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
