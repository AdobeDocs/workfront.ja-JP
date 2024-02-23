---
title: ユーザーの環境設定をリセット
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 管理者は、Workfront システム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。個々のユーザーは、独自のユーザー環境設定をリセットすることもできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: c3cb97a36c29b90bbc9d8438d8811cc23266d894
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 79%

---

# ユーザーの環境設定をリセット

<!-- Audited: 12/2023 -->

Adobe Workfront 管理者は、Workfront システム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。

個々のユーザーは、独自のユーザー環境設定をリセットすることもできます。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p> システムのデフォルトに戻しました</p> <p>既存のビューは削除されません。 もう一度選択できます。</p> </td> 
  </tr> 
  <tr> 
   <td>フィルター</td> 
   <td> <p>システムのデフォルトに戻しました</p> <p>既存のフィルターは削除されません。 もう一度選択できます。</p> </td> 
  </tr> 
  <tr> 
   <td>グループ化</td> 
   <td> <p>システムのデフォルトに戻しました</p> <p>既存のグループは削除されません。 もう一度選択できます。</p> </td> 
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
   <td> <p>システムのデフォルトに戻しました</p> <p>電子メール通知がシステムのデフォルトに戻ります。 デフォルトの通知は、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Adobe Workfrontで使用可能なイベント通知</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー定義のカスタムタブ</td> 
   <td>削除されました</td> 
  </tr> 
  <tr> 
   <td>ユーザー定義のグローバルナビゲーションオプション</td> 
   <td>レイアウトテンプレート定義に戻すか、レイアウトテンプレートが割り当てられていない場合はシステムの既定に戻します。</td> 
  </tr> 
 </tbody> 
</table>

## ユーザーの環境設定をリセット

{{step-1-to-setup}}

1. 「**別のユーザーとしてログイン**」を選択します。
1. 環境設定をリセットするユーザーの名前を入力し始め、ドロップダウンリストに表示されたら名前をクリックします。
1. 「**ログイン**」を選択します。
1. Web ブラウザーの上部にある「URL」フィールドで、`workfront.com` の後に `/resetUser` を追加します。

   >[!NOTE]
   >
   >大文字と小文字が区別されます。U 文字は大文字で、残りの文字は小文字にする必要があります。例：
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. **Enter** キーを押します。
1. すべてのユーザー環境設定をリセットするには、「**リセット**」を選択します。

   または

   カスタムタブのみをリセットするには、「**タブのリセット**」を選択します。
