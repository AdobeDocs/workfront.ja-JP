---
title: ユーザーの削除
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 組織を離れたユーザーは Workfront から削除できますが、削除する代わりにディアクティベートすることをお勧めします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: b3717fc89e45983b80471fdd629c79b82086c6ff
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 97%

---

# ユーザーの削除

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

この記事の手順を実行するには、以下を保有している必要があります。

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
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。 </p> </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>この 2 つのオプションのうち、ユーザー<b>管理者（グループユーザー）</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>アクセスレベルの<b>ユーザー</b>設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーの削除とディアクティベートの違い

ユーザーをディアクティベートすると、次のことが発生します。

* Workfront Proof コンポーネントが Workfront アカウントに関連付けられている場合は、Workfront と Workfront Proof の両方に対するユーザーライセンスが削除されます。Workfront Proof について詳しくは、 [Workfront Proof：記事インデックス](../../../workfront-proof/workfront-proof.md).
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

* Workfront Proof コンポーネントが Workfront アカウントに関連付けられている場合は、Workfront と Workfront Proof の両方に対するユーザーライセンスが削除されます。Workfront Proof について詳しくは、 [Workfront Proof：記事インデックス](../../../workfront-proof/workfront-proof.md).
* ユーザーに作業を割り当てることができなくなります。
* ユーザーを更新に追加できなくなります。
* ユーザーをチームやグループに追加できなくなります。
* ユーザーにオブジェクトを共有できなくなります。
* ユーザーと次のオブジェクトの関連付けが削除されます。

   * タスク、イシュー、プロジェクト、ポートフォリオ
   * ダッシュボード

     >[!NOTE]
     >
     >また、削除したユーザーに関連付けられていたダッシュボードを含んだカスタムセクションへのアクセス権も失われます。\
     >詳しくは、[削除されたユーザーが所有していたレポートを含んだダッシュボードにアクセスするには、どうすればよいですか？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how)の節（[レポートに関する FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) の記事内）を参照してください。

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

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**ユーザー**」をクリックします。
1. 削除するユーザーを少なくとも 1 人選択し、その他メニュー ![](assets/more-icon.png) をクリックします。次に「**削除**」をクリックします。
1. 表示されるボックスで、「**削除**」をクリックして削除を確定します。

   ユーザーを削除するプロセスはバックグラウンドプロセスとして実行されるので、ユーザーが削除されているときも Workfront を引き続き使用できます。

   削除するユーザーの数によっては、処理に数分かかる場合も、数時間かかる場合もあります。

   Workfront でユーザーが削除されたことを示す確認メッセージが表示されてから、削除プロセスがバックグラウンドで完了するまで、システム内で引き続き表示される場合があります。

   後で、1 人または複数のユーザーが正常に削除されなかったことが判明した場合は、1 人ずつ削除してみてください。
