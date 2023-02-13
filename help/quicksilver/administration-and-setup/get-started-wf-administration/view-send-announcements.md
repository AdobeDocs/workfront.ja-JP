---
user-type: administrator
product-area: system-administration
navigation-topic: start-with-workfront-administration
title: お知らせの送信
description: Adobe Workfront管理者は、お知らせページを使用して、お知らせをユーザーに送信できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 413e3051-fcb5-44d7-b6bd-6b05d39935e8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 1%

---

# お知らせの送信

Adobe Workfront管理者は、お知らせページを使用して、お知らせをユーザーに送信できます。

Workfrontからのお知らせメッセージには、通常、新機能とリリース、プロセスの変更などに関する情報が含まれます。

お知らせの表示については、 [アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

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
   <td> <p>Workfront管理者である。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーにお知らせを送信

以下を使用して、 **お知らせ** Workfrontから送信されたお知らせを転送し、新しいお知らせを作成することで、Workfrontシステムのユーザーとコミュニケーションを取るためのページ。 Workfrontシステム内の特定のユーザー、グループ、チームまたは会社にお知らせを送信できます。

* [Workfrontのお知らせをユーザーに転送する](#forward-workfront-announcements-to-users)
* [新しいお知らせの作成](#compose-new-announcements)

### Workfrontのお知らせをユーザーに転送する {#forward-workfront-announcements-to-users}

Workfrontから受け取ったメッセージを、システム内のユーザーに簡単に転送できます。

1. お知らせページに移動するには、 **通知** Workfrontインターフェイスの右上隅にあるアイコンをクリックし、 **すべてのお知らせ**.

   ![](assets/announcement-access-350x212.png)

1. の **お知らせ** ページで、転送するメッセージを選択します。
1. クリック **進む**.
1. 内 **送信先** ボックスに、お知らせメッセージを受け取るユーザー、グループ、チーム、または会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。 複数のユーザー、グループ、チームまたは会社を追加するには、この手順を繰り返します。

   または

   お知らせをシステム内のすべてのユーザーに転送するには、次のように入力します。 **全員**&#x200B;をクリックし、ドロップダウンリストに表示されたらクリックします。

1. 手順 3( [新しいお知らせの作成](#compose-new-announcements).

### 新しいお知らせの作成 {#compose-new-announcements}

1. お知らせページに移動するには、 **通知** Workfrontインターフェイスの右上隅にあるアイコンをクリックし、 **すべてのお知らせ**.

   ![](assets/announcement-access-350x212.png)

1. の **お知らせ** ページ、クリック **新しいお知らせ。**

1. 内 **送信先** ボックスに、お知らせメッセージを受け取るユーザー、グループ、チーム、または会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。 複数のユーザー、グループ、チームまたは会社を追加するには、この手順を繰り返します。

   デフォルトでは、新しいお知らせメッセージを送信する場合、 **全員** がこのフィールドに事前に入力されている。 システム内のすべてのユーザーがアナウンスメッセージを受け取りたくない場合は、 **全員** を選択します。

1. 次の追加情報を指定します。

   | 件名 | お知らせの件名を指定します。 |
   |---|---|
   | ここにメッセージを入力してください | メッセージのコンテンツを指定します。 メッセージエディターでは、太字、斜体、下線、箇条書きと番号付きのリスト、ハイパーリンクなど、一般的なマークアップを含めることができます。 |
   | 添付 | クリック&#x200B;**添付ファイルを追加** 次に、メッセージに添付するファイルを参照して選択します。 |

   {style=&quot;table-layout:auto&quot;}

1. （オプション）「 **ドラフトとして保存** ：メッセージ（受信者リスト、件名、添付ファイルを含む）を下書きとして保存します。

1. （オプション）下書きを表示するには、 **お知らせ** 領域、クリック **ドラフト**.

1. クリック **送信。**

   ユーザーは、「 [アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 受け取るWorkfrontのお知らせのタイプを制限

Workfrontの管理者は、特定の種類のメッセージの受信を登録解除できます。

デフォルトでは、Workfrontから送信されたすべてのメッセージを受信します。 これは推奨される設定です。

1. の **お知らせ** ページ、クリック **設定。**
1. メッセージの受信を停止するトピックを選択します。
1. クリック **設定を保存します。**
