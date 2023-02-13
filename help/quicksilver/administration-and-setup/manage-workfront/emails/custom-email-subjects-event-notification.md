---
navigation-topic: notifications
title: イベント通知の電子メールの件名をカスタマイズする
description: イベント通知でトリガーされる電子メールの件名行をカスタマイズできます。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 4%

---

# イベント通知の電子メールの件名をカスタマイズする

イベント通知でトリガーされる電子メールの件名行をカスタマイズできます。

件名行を変更すると、受信者のアクセスレベルに関係なく、システム内のすべてのユーザーに影響します。 電子メールの件名に含まれるすべてのオブジェクトとフィールドが表示されます。

一部のイベント通知には複数の件名が含まれています。つまり、これらのイベント通知の機能に基づいて、複数の電子メール件名を持つことができます。

>[!IMPORTANT]
>
>件名行が複数のオブジェクトを参照している場合は、デフォルトのフィールドを削除する際に注意してください。 以下は、このような件名行を含むイベント通知のリストです。
>
>* 自分が更新を受信する対象者として追加された
>* 自分チームが更新を受信する対象として追加された
>* スレッド参加者宛作業アイテム コメント
>* 作業アイテム割り当て先宛作業アイテム コメント
>


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プランナー以上（リマインダー通知への管理アクセス権を持つ）</p> <p>プランのユーザー管理アクセス権の付与については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## イベント通知用の電子メールの件名行のカスタマイズ {#customize-email-subject-lines-for-event-notifications}

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **電子メール** > **通知**.

1. 次をクリック： **イベント通知** タブをクリックします。
1. カスタマイズするイベント通知の名前をクリックして、 **イベント通知** ボックス
1. 内 **メールの件名行** 」ボックスで、電子メールの件名のテキストおよびフィールド（カスタムフィールドを含む）を変更します。

   追加するフィールドの名前は、データベース構造のキャメルケース構文と一致する必要があります。 <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. クリック **更新** ：メールの新しい件名行を保存します。

## 複数オブジェクトの電子メールの電子メール件名行のカスタマイズ

一部のイベント通知には、イベントの対象となるオブジェクトに応じて、複数の件名がトリガーされます。

例えば、「Some include me on a directed update」には、2 つの異なる件名が含まれます。1 つ目はタスク、問題点、テンプレートタスク、ドキュメント（「referenceObject」とも呼ばれます）、もう 1 つは、ポートフォリオ、プログラムなどのコメントをユーザーが作成できるオブジェクト（「topReferenceObject」とも呼ばれます）です。

![](assets/Ev-not-mult-subj-lines.png)

タスク、イシュー、テンプレートタスク、またはドキュメントに関する会話にユーザーが含まれる場合は、最初の件名行で E メールが生成されます。 件名行には「referenceObject:name」が含まれ、システムはオブジェクトを定義し、適切な名前を件名フィールドに表示します。 E メールの件名行は次のようになります。&quot;Project ABC のタスク 123 に対するコメント。&quot;

プロジェクトの会話に追加すると、2 番目の件名の E メールが生成されます。 件名行には「topReferenceObject:name」が含まれ、Workfrontは参照されたオブジェクトを識別し、件名内の「topReferenceObject:name」の代わりにそのオブジェクト名を返します。 E メールの件名行は次のようになります。「Project ABC に対するコメント。」

E メールの件名行を編集し、いずれかの件名行にフィールドを追加するには、 [イベント通知用の電子メールの件名行のカスタマイズ](#customize-email-subject-lines-for-event-notifications) 」を参照してください。

## 複数アクションの E メールの E メール件名行のカスタマイズ

また、イベント通知には、オブジェクトに対して実行される様々なアクションの概要を示す複数の電子メール件名が含まれています。

例えば、問題にドキュメントを追加するように要求するイベントは、次の 2 つの異なる E メールをトリガーにできます。1 つはドキュメントの追加時に、もう 1 つはドキュメントの編集時に使用します。

![](assets/ev-not-mult-subj-lines-diff-actions.png)

E メールの件名行を編集し、いずれかの件名行にフィールドを追加するには、 [イベント通知用の電子メールの件名行のカスタマイズ](#customize-email-subject-lines-for-event-notifications) 」を参照してください。
