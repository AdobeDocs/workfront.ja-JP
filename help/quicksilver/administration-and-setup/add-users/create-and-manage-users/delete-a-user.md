---
title: ユーザーの削除
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: ユーザーが組織を離れたとき、はそのユーザーをWorkfrontから削除できますが、削除する代わりにユーザーを非アクティブ化することをお勧めします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# ユーザーの削除

ユーザーが組織を離れたときに、そのユーザーをAdobe Workfrontから削除できます。

>[!IMPORTANT]
>
>* システムからユーザを削除すると、保持したいユーザに関連付けられた情報も削除されます。 ユーザーを削除する代わりに非アクティブ化することをお勧めします。 詳しくは、 [ユーザーを非アクティブ化または再アクティブ化する](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>ユーザーの削除 [!DNL Adobe Admin Console] でユーザーを非アクティブ化 [!DNL Workfront]を削除することはできませんが、 [!DNL Workfront].
>
>  Adobe Admin Consoleでユーザーを削除する手順については、この記事の「ユーザーの恒久的な削除」の節を参照してください [ユーザーを個別に管理](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) または、Adobe Admin Console管理者に問い合わせてください。
>
>  組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

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
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> </li> 
     <li> <p><b>ユーザー</b> 設定を <b>編集</b> アクセス、 <b>作成</b> そして少なくとも 2 つのうち 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>この 2 つのオプションのうち、ユーザー <b>管理者（グループユーザー）</b> が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>詳しくは、 <b>ユーザー</b> アクセスレベルでの設定については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーの削除と非アクティブ化

ユーザーを非アクティブ化すると、次のことが発生します。

* Workfront配達確認コンポーネントがWorkfrontアカウントに関連付けられている場合、WorkfrontとWorkfrontの両方に対するユーザーのライセンスを削除します。 Workfront Proof について詳しくは、 [Workfront Proof](../../../workfront-proof/workfront-proof.md).
* ユーザーは作業を割り当てることができなくなりました。
* ユーザーを更新に追加できなくなりました。
* ユーザーをチームやグループに追加できなくなりました。
* オブジェクトをユーザーと共有できなくなりました。
* 次のオブジェクトとの関連付けはそのまま維持されます。

   * タスク、問題、プロジェクト、ポートフォリオ
   * ダッシュボード

      >[!NOTE]
      >
      >ユーザーを非アクティブ化して、ユーザーに関連付けられたレポートやダッシュボードを表示できなくなった場合は、 **このレポートを実行する際のアクセス権は次のとおりです。** フィールドに入力します。\
      >詳しくは、 [非アクティブなユーザーが所有するレポートにアクセスできないのはなぜですか？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) セクション [レポートの FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 記事。

   * ドキュメント
   * 更新
   * 時間

* ユーザーがチェックアウトしたドキュメントは、非アクティブ化してもチェックアウトされたままです。 再度チェックインできるのは、Workfront管理者のみです。 ドキュメントのチェックアウトの詳細については、 [ドキュメントをチェックアウト](../../../documents/managing-documents/check-out-documents.md).

ユーザーを削除すると、次のことが発生します。

* Workfront配達確認コンポーネントがWorkfrontアカウントに関連付けられている場合、WorkfrontとWorkfrontの両方に対するユーザーのライセンスを削除します。 Workfront Proof について詳しくは、 [Workfront Proof](../../../workfront-proof/workfront-proof.md).
* ユーザーは作業を割り当てることができなくなりました。
* ユーザーを更新に追加できなくなりました。
* ユーザーをチームやグループに追加できなくなりました。
* オブジェクトをユーザーと共有できなくなりました。
* 次のオブジェクトに対するユーザーの関連付けを削除します。

   * タスク、問題、プロジェクト、ポートフォリオ
   * ダッシュボード

      >[!NOTE]
      >
      >また、削除したユーザーに関連付けられたダッシュボードを含むカスタムセクションへのアクセス権も失われます。\
      >詳しくは、 [削除されたユーザーが所有するレポートを含むダッシュボードにアクセスするには、どうすればよいですか？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) セクション [レポートの FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 記事。

   * 更新
   * 時間

      >[!NOTE]
      >
      >これらのオブジェクトはWorkfrontに残りますが、オブジェクトの所有者は空になります。

* ユーザーがグローバルナビゲーションバーの「ドキュメント」領域でドキュメントをアップロードした場合、そのドキュメントも削除されます。
* ユーザーが自分の所有するドキュメントをチェックアウトし、（メインメニューからアクセスする）メインのドキュメント領域にドキュメントがアップロードされた場合、そのドキュメントはユーザーと共に削除されます。 ドキュメントのチェックアウトの詳細については、 [ドキュメントをチェックアウト](../../../documents/managing-documents/check-out-documents.md).

ユーザーの非アクティブ化について詳しくは、 [ユーザーを非アクティブ化または再アクティブ化する](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

一度に 1 人のユーザーを完全に削除することも、複数のユーザーを同時に完全に削除することもできます。 個々のユーザーを削除する場合は、削除プロセスが完了するのを待ってから、Workfrontの他のアクティビティに移動する必要があります。 複数のユーザーを削除するプロセスは、バックグラウンドプロセスとして同時に実行されるので、ユーザーが削除された後もWorkfrontを引き続き使用できます。

## 1 人以上のユーザーを削除

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **ユーザー**.
1. 削除するユーザーを少なくとも 1 人選択し、その他メニューをクリックします ![](assets/more-icon.png)を選択し、「 **削除**.
1. 表示されるボックスで、 **削除** 削除を確定します。

   ユーザーを削除するプロセスは、バックグラウンドプロセスとして実行されるので、ユーザーが削除された後もWorkfrontを引き続き使用できます。

   削除するユーザーの数によっては、処理に数分かかる場合も、数時間かかる場合もあります。

   Workfrontでユーザーが削除されたことを示す確認メッセージが表示されたら、削除プロセスがバックグラウンドで完了するまで、システム内で引き続き表示されます。

   後で、1 人または複数のユーザーが正常に削除されなかったことが判明した場合は、一度に 1 人ずつ削除してみてください。
