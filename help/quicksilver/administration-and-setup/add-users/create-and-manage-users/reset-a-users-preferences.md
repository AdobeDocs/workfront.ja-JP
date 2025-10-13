---
title: ユーザーの環境設定のリセット
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 管理者は、Workfront システム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。個々のユーザーは、独自のユーザー環境設定をリセットすることもできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 4a7362ae663b73ce48f049556145b4de3e6a6ac9
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 85%

---

# ユーザーの環境設定をリセット

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Adobe Workfront 管理者は、Workfront システム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。

個々のユーザーは、独自のユーザー環境設定をリセットすることもできます。

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
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 影響を受ける設定について

ユーザーの環境設定をリセットすると、一部の環境設定はシステムのデフォルトに戻り、それ以外の環境設定はクリアまたは削除されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>設定</strong> </th> 
   <th><strong>リセット後のステータス</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ビュー</td> 
   <td> <p> システムのデフォルトに戻しました</p> <p>既存のビューは削除されません。もう一度選択できます。</p> </td> 
  </tr> 
  <tr> 
   <td>フィルター</td> 
   <td> <p>システムのデフォルトに戻しました</p> <p>既存のフィルターは削除されません。もう一度選択できます。</p> </td> 
  </tr> 
  <tr> 
   <td>グループ化</td> 
   <td> <p>システムのデフォルトに戻しました</p> <p>既存のグループは削除されません。もう一度選択できます。</p> </td> 
  </tr> 
  <tr> 
   <td>最近使用した項目のリスト</td> 
   <td>クリア済み</td> 
  </tr> 
  <tr> 
   <td>お気に入りリスト</td> 
   <td>影響なし</td> 
  </tr> 
  <tr> 
   <td>ユーザーの環境設定</td> 
   <td> <p>システムのデフォルトに戻しました</p> <p>メール通知がシステムのデフォルトに戻ります。デフォルトの通知については、<a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Adobe Workfront で使用可能なイベント通知</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー定義のカスタムタブ</td> 
   <td>削除されました</td> 
  </tr> 
  <tr> 
   <td>ユーザー定義のグローバルナビゲーションオプション</td> 
   <td>レイアウトテンプレートが割り当てられていない場合は、レイアウトテンプレート定義に戻すか、システムのデフォルトに戻します。</td> 
  </tr> 
 </tbody> 
</table>

<!-- Display this table and hide the HTML table above, when the unshim is released.
| Preference | Status after the reset |
| --- | --- |
| Views | Reverted to the system default <p>Existing views are not deleted. You can select them again.</p> |
| Filters | Reverted to the system default <p>Existing filters are not deleted. You can select them again.</p> |
| Groupings | Reverted to the system default <p>Existing groupings are not deleted. You can select them again.</p> |
| Recent items list | Cleared |
| Favorites list | Unaffected |
| User Preferences | Reverted to the system default <p>Email notifications revert to the system defaults. The default notifications are listed in [Event notifications available in Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |
-->

## ユーザーの環境設定をリセット

{{step-1-to-setup}}

1. 「**別のユーザーとしてログイン**」を選択します。
1. 環境設定をリセットするユーザーの名前を入力し始め、ドロップダウンリストに表示されたら名前をクリックします。
1. 「**ログイン**」を選択します。
1. 組織がAdobe Unified Experience にオンボーディングされていない場合は、次の手順に従います。

   * Web ブラウザーの上部にある「URL」フィールドで、`workfront.com` の後に `/resetUser` を追加します。

     >[!NOTE]
     >
     >大文字と小文字が区別されます。U 文字は大文字で、残りの文字は小文字にする必要があります。例：
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. 組織がAdobe Unified Experience にオンボーディングされた場合は、次の手順に従います。

   * Web ブラウザーの上部にある URL フィールドで、`/resetUser` の後に `workfront` を追加します。

     >[!NOTE]
     >
     >大文字と小文字が区別されます。U 文字は大文字で、残りの文字は小文字にする必要があります。例：
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. **Enter** キーを押します。
1. すべてのユーザー環境設定をリセットするには、「**リセット**」を選択します。

<!--When this is unshimmed, adjust the comment tags to hide these last two lines, because the Reset Tabs button is going away.-->
または

カスタムタブのみをリセットするには、「**タブのリセット**」を選択します。
