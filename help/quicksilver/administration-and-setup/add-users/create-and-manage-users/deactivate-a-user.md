---
title: ユーザーを非アクティブ化または再アクティブ化する
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront管理者は、ユーザーを非アクティブ化または再アクティブ化できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# ユーザーを非アクティブ化または再アクティブ化する

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>Adobe Admin Consoleでユーザーを非アクティブ化する手順については、この記事の「ユーザーの削除」の節を参照してください [ユーザーを個別に管理](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) または、Adobe Admin Console管理者に問い合わせてください。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

ユーザーが組織から退出し、Adobe Workfrontから削除する必要が生じる場合があります。 更新に追加したり、割り当てたりする際に、他のユーザーが混乱を招くので、システム内でユーザーをアクティブにしておく必要はありません。 ユーザーを非アクティブ化すると、システム内のユーザーを検索する際に、他のユーザーの名前が表示されなくなります。

管理者は、非アクティブなユーザーを「設定」領域で確認できます。

ユーザーはいつでも再アクティブ化できます。

>[!IMPORTANT]
>
>組織を退職したユーザーは、削除するのではなく、非アクティブ化することをお勧めします。 ユーザーを削除すると、そのユーザーに関連付けられたWorkfront内のすべての履歴が失われます。 これには、作業割り当て、注記、時間、ドキュメント、および一度作成したその他すべてのオブジェクトとの関連付けが含まれます。
>
>Workfrontでユーザーを非アクティブ化すると、Workfrontとデジタル校正の両方に対するユーザーのライセンスが削除されます。 また、ユーザーに作業を割り当てることはできなくなりました。 ユーザーを非アクティブ化すると、そのユーザーのWorkfrontライセンスおよび校正ライセンスを別のユーザーが使用できるようになります。非アクティブ化されたユーザーのプロファイルに含まれるその他の情報は、そのまま残ります。
>
>削除による影響とユーザーの非アクティブ化の影響について詳しくは、 [ユーザーの削除](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

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
   <td> <p>計画 </p>   </td> 
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

## ユーザーを非アクティブ化する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).

1. ユーザーを選択し、「その他」アイコンをクリックします。 ![](assets/more-icon.png)を選択し、「 **無効化**.

1. クリック **無効化** をクリックします。

## ユーザーのアクティベーション解除をスケジュール

管理者は、実際に組織を離れる前に、ユーザーに非アクティブ化のマークを付けたい場合があります。 例えば、契約上の拘束を受けているユーザーと協力している場合、そのユーザーは限られた期間システム内に存在し、その終了日を把握しています。 これらを、その日に非アクティブ化するようにスケジュール設定できます。

Workfront管理者とプランライセンスユーザーは、ユーザープロファイルにアクティベート解除日を表示できます。

ユーザーの非アクティブ化をスケジュールするには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).

1. ユーザー名を選択します。

   または

   （オプション）複数のユーザーを選択して、一括での非アクティブ化をスケジュールします。

1. 編集アイコンをクリックします。 ![](assets/edit-icon.png).
1. 表示されるユーザーを編集ボックスで、 **リソース計画** そこに行く
1. を有効にします。 **無効化をスケジュール** オプション。

1. 表示されるカレンダーで、 **予定されている非アクティブ化日**.

   >[!NOTE]
   >
   >* 時間ボックスでは、分単位ではなく、1 時間単位のみを選択できます。
   >* 現在の日を過ぎた時刻を選択した場合、Workfrontでは翌日の午前 12 時にアクティベート解除がスケジュールされます。 選択した時間は、アクティベーション解除をスケジュールしているユーザーのコンピュータータイムゾーンに一致します。


1. クリック **変更を保存**.

   ユーザーは、選択した日に非アクティブ化され、選択した時間が経過した後に非アクティブ化される場合があります。 複数のユーザーを一括で非アクティブ化するように選択した場合、選択したすべてのユーザーは、選択した時間が経過した後に、選択した日に非アクティブ化されることがあります。

非アクティブ化が予定されているユーザーについて常に知らせるために、非アクティブ化をスケジュールしたユーザーに関するレポートを作成することをお勧めします。 ユーザーが非アクティブ化された後に非アクティブ化がおこなわれたことを示す確認はありません。

## ユーザーの再アクティブ化

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).

1. ユーザーを選択し、「その他」アイコンをクリックします。 ![](assets/more-icon.png)を選択し、「 **有効化**.

1. 新しいを割り当て **アクセスレベル**」と入力します。

### ユーザーを再アクティブ化したときの校正の影響

非アクティブなユーザーは、割り当てられたデフォルトの校正の役割と配達確認用ライセンスを失います (Workfront Premium レガシープランを使用している場合 )。 ユーザーを再アクティブ化する場合は、次の操作を行う必要があります。

* ライセンスを再割り当てします (Workfront Premium レガシープランを使用している場合 )。 Workfrontの校正プランについて詳しくは、 [Workfrontの校正機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* 配達確認の役割が正しいことを確認します。 再アクティブ化された配達確認ユーザーには、新しいユーザーのデフォルトの配達確認の役割として指定されているものが割り当てられます。 詳しくは、 [既定の校正の役割を設定する](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) を参照してください。

## Workfront管理者の非アクティブ化とライセンスユーザーの計画について

Workfront管理者またはプランライセンスを持つユーザーを非アクティブ化する前に、そのユーザーが関与するWorkfrontオブジェクトやアクティビティを確認し、必要に応じて別のWorkfront管理者または Plan license user に関連付けることが重要です。

これらのオブジェクトやアクティビティには、次のものが含まれます。

* ユーザーに割り当てられたタスクまたはタスク
* ユーザーが所有するプロジェクト
* ユーザーのアクセス権で実行するように設定されたレポート
* ユーザーが所有するテンプレート
* ユーザーがリソースマネージャーとして設定されたプロジェクトとテンプレート
* Workfront管理者またはプランライセンスユーザーがデフォルトの担当者であるキュールーティングルールをリクエストします
* ユーザーを含むステージを持つ承認プロセス（特に、ステージで唯一の承認者であった場合）
* ユーザーを承認者として一覧表示するタイムシート
* ユーザーを承認者として一覧表示するタイムシートプロファイル
* ユーザーを含む自動ワークフローの校正

## ユーザーの非アクティブ化をスケジュールする際のリソース計画への影響

ユーザーを非アクティブ化するようにスケジュールすると、そのユーザーは、予算編成時間に使用できるとして「リソース・プランナ」に表示されなくなります。 資源プールに残っている場合は、資源プールナに表示されますが、使用可否は、予定されている無効化の日から 0 時間に設定されます。

リソース・プランナは、タスクのユーザーのすべての役割と計画完了日を考慮し、それに応じてリソースを計算します。

リソース・プランナの詳細は、 [リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
