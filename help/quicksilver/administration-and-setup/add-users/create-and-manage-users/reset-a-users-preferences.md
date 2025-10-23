---
title: ユーザーの環境設定のリセット
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 管理者は、Workfront システム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。個々のユーザーは、独自のユーザー環境設定をリセットすることもできます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 73%

---

# ユーザーの環境設定をリセット

<!-- Audited: 12/2023 -->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。これはプレビューサンドボックス環境でのみ使用でき、実稼動環境への段階的なロールアウトでリリースされています。</span>

Adobe Workfront 管理者は、Workfront システム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。

個々のユーザーは、独自のユーザー環境設定をリセットすることもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 影響を受ける設定について

ユーザーの環境設定をリセットすると、一部の環境設定はシステムのデフォルトに戻り、それ以外の環境設定はクリアまたは削除されます。

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| 設定 | リセット後のステータス |
| --- | --- |
| ビュー | システムのデフォルトに戻しました <p>既存のビューは削除されません。もう一度選択できます。</p> |
| フィルター | システムのデフォルトに戻しました <p>既存のフィルターは削除されません。もう一度選択できます。</p> |
| グループ化 | システムのデフォルトに戻しました <p>既存のグループは削除されません。もう一度選択できます。</p> |
| 最近使用した項目リスト | クリア済み |
| お気に入りリスト | 影響なし |
| ユーザーの環境設定 | システムのデフォルトに戻しました <p>メール通知がシステムのデフォルトに戻ります。デフォルトの通知については、[Adobe Workfront で使用可能なイベント通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)を参照してください。</p> |

</div>

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

<div class="preview">

1. すべてのユーザー環境設定をリセットするには、「**リセット**」をクリックします。

   または

   カスタム タブのみをリセットするには、[**左ナビゲーションのリセット**] をクリックします。

</div>
