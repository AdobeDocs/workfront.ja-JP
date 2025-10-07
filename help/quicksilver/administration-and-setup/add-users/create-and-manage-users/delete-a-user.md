---
title: ユーザーの削除
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 組織を離れたユーザーは Workfront から削除できますが、削除する代わりにディアクティベートすることをお勧めします。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 87%

---

# ユーザーの削除

>[!IMPORTANT]
>
>ここで説明する手順は、Adobe Business Platform にまだオンボーディングされていない組織にのみ適用されます。 Adobe Business Platform にオンボーディング済みの場合は、Adobe Admin Consoleでユーザーを削除する必要があります。
>
>組織が Adobe Business Platform に登録されているかどうかによって異なる手順のリストについては、[プラットフォームによる管理の違い（Adobe Workfront Fusion／Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

組織を離れたユーザーは、Adobe Workfront から削除することができます。

>[!IMPORTANT]
>
>システムからユーザを削除すると、そのユーザに関連付けられていて、今後も保持したい情報も削除されます。ユーザーを削除する代わりに非アクティブ化することをお勧めします。詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p><p>または</p><p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これら 2 つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーの削除とディアクティベートの違い

ユーザーをディアクティベートすると、次のことが発生します。

* Workfront Proof コンポーネントが Workfront アカウントに関連付けられている場合は、Workfront と Workfront Proof の両方に対するユーザーライセンスが削除されます。Workfront Proof について詳しくは、[Workfront Proof：記事インデックス](../../../workfront-proof/workfront-proof.md)を参照してください。
* ユーザーに作業を割り当てることができなくなります。
* ユーザーを更新に追加できなくなります。
* ユーザーをチームやグループに追加できなくなります。
* ユーザーにオブジェクトを共有できなくなります。
* 次のオブジェクトとの関連付けはそのまま残ります。

   * タスク、イシュー、プロジェクト、ポートフォリオ
   * ダッシュボード

     >[!NOTE]
     >
     >ユーザーをディアクティベートし、そのユーザーに関連付けられているレポートやダッシュボードを表示できなくなった場合は、「**このレポートを次のアクセス権で実行：**」フィールドを更新する必要がある場合があります。\
     >詳しくは、[ディアクティベートされたユーザーが所有するレポートにアクセスできないのはなぜですか？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) セクション（[レポートに関する FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)内）を参照してください。

   * ドキュメント
   * アップデート
   * 時間

* ユーザーがチェックアウトしたドキュメントは、そのユーザーがディアクティベートされてもチェックアウトされたままになります。再度チェックインできるのは、Workfront 管理者のみです。ドキュメントのチェックアウトについて詳しくは、[ドキュメントのチェックアウト](../../../documents/managing-documents/check-out-documents.md)を参照してください。

ユーザーを削除すると、次のことが発生します。

* Workfront Proof コンポーネントが Workfront アカウントに関連付けられている場合は、Workfront と Workfront Proof の両方に対するユーザーライセンスが削除されます。Workfront Proof について詳しくは、[Workfront Proof：記事インデックス](../../../workfront-proof/workfront-proof.md)を参照してください。
* ユーザーに作業を割り当てることができなくなります。
* ユーザーを更新に追加できなくなります。
* ユーザーをチームやグループに追加できなくなります。
* ユーザーにオブジェクトを共有できなくなります。
* ユーザーと次のオブジェクトの関連付けが削除されます。

   * タスク、イシュー、プロジェクト、ポートフォリオ
   * ダッシュボード

  <!--
     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.
     -->

   * アップデート
   * 時間

     >[!NOTE]
     >
     >これらのオブジェクトは Workfront に残りますが、オブジェクトの所有者は空になります。

* ユーザーがグローバルナビゲーションバーのドキュメントエリアでドキュメントをアップロードした場合、そのドキュメントも削除されます。
* ユーザーが自分の所有するドキュメントをチェックアウトし、（メインメニューからアクセスする）メインのドキュメントエリアにドキュメントがアップロードされた場合、そのドキュメントはユーザーと共に削除されます。ドキュメントのチェックアウトについて詳しくは、[ドキュメントのチェックアウト](../../../documents/managing-documents/check-out-documents.md)を参照してください。

ユーザーの非アクティブ化について詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。

一度に 1 人のユーザーを完全に削除することも、複数のユーザーを同時に完全に削除することもできます。個々のユーザーを削除する場合は、削除プロセスが完了するのを待ってから、Workfront の他のアクティビティに移動する必要があります。複数のユーザーを削除するプロセスは、バックグラウンドプロセスとして同時に実行されるので、ユーザーが削除されているときも Workfront を引き続き使用できます。

## 1 人以上のユーザーを削除

{{step-1-to-users}}

1. 削除する 1 人以上のユーザーを選択し、「詳細」メニュー ![ 詳細アイコン ](assets/more-icon.png) をクリックして、「**削除**」をクリックします。
1. 表示されるボックスで、「**削除**」をクリックして削除を確定します。

   ユーザーを削除するプロセスはバックグラウンドプロセスとして実行されるので、ユーザーが削除されているときも Workfront を引き続き使用できます。

   削除するユーザーの数によっては、処理に数分かかる場合も、数時間かかる場合もあります。

   Workfront でユーザーが削除されたことを示す確認メッセージが表示されてから、削除プロセスがバックグラウンドで完了するまで、システム内で引き続き表示される場合があります。

   後で、1 人または複数のユーザーが正常に削除されなかったことが判明した場合は、1 人ずつ削除してみてください。
