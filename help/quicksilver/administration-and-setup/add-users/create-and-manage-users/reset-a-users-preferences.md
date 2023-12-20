---
title: ユーザーの環境設定のリセット
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront管理者は、Workfrontシステム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。 個々のユーザーは、独自のユーザー設定をリセットすることもできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: ae063189eebb17a3341aabb978ee0f0e03d1e299
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# ユーザーの環境設定のリセット

<!-- Audited: 12/2023 -->

Adobe Workfront管理者は、Workfrontシステム内の任意のユーザーのユーザー環境設定をリセットまたは削除できます。

個々のユーザーは、独自のユーザー設定をリセットすることもできます。

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
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>：まだアクセス権がない場合は、Workfront管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 影響を受ける設定について

ユーザーの環境設定をリセットすると、一部の環境設定はシステムのデフォルトに戻り、それ以外の環境設定はクリアまたは削除されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>環境設定</strong> </th> 
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
   <td>最近使用した項目の一覧</td> 
   <td>クリア済み</td> 
  </tr> 
  <tr> 
   <td>お気に入りリスト</td> 
   <td>影響なし</td> 
  </tr> 
  <tr> 
   <td>ユーザーの環境設定</td> 
   <td> <p>システムのデフォルトに戻しました</p> <p>電子メール通知がシステムのデフォルトに戻ります。</p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー定義のカスタムタブ</td> 
   <td>削除済み</td> 
  </tr> 
  <tr> 
   <td>ユーザー定義のグローバルナビゲーションオプション</td> 
   <td>レイアウトテンプレート定義に戻すか、レイアウトテンプレートが割り当てられていない場合はシステムの既定に戻します。</td> 
  </tr> 
 </tbody> 
</table>

## ユーザーの環境設定をリセット

{{step-1-to-setup}}

1. 選択 **ログイン名**.
1. 環境設定をリセットするユーザーの名前を入力し始め、ドロップダウンリストに表示されたら名前をクリックします。
1. 選択  **ログイン**.
1. Web ブラウザーの上部にある「 URL 」フィールドで、 `/resetUser` 次より後 `workfront.com`.

   >[!NOTE]
   >
   >大文字と小文字が区別されます。 U 文字は大文字で、残りの文字は小文字で指定する必要があります。 例：
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. 押す **入力**.
1. すべてのユーザー環境設定をリセットするには、「 **リセット**.

   または

   カスタムタブのみをリセットするには、「 **タブをリセット**.
