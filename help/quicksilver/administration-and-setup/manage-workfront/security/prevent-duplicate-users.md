---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: メールアドレスの重複を防止
description: Adobe Workfront で新規ユーザーを作成する場合、大文字と小文字でメールアドレスが異なる場合でも（例えば、JohnDoe@example.com と johndoe@example.com など）、別のユーザーがすでに使用しているメールアドレスを使用できません。さらに、将来の認証強化に備えて、すべてのユーザーが Workfront インスタンスで一意のメールアドレスを持っていることを確認してください。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: ht
source-wordcount: '608'
ht-degree: 100%

---

# メールアドレスの重複を防止

Adobe Workfront で新規ユーザーを作成する場合、大文字と小文字でメールアドレスが異なる場合でも（例えば、JohnDoe@example.com と johndoe@example.com など）、別のユーザーがすでに使用しているメールアドレスを使用できません。さらに、将来の認証強化に備えて、すべてのユーザーが Workfront インスタンスで一意のメールアドレスを持っていることを確認してください。

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
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 一意のメールアドレスを持つユーザーを作成

2019.4 リリース以降、Workfront で新規ユーザーを作成する場合、大文字と小文字でメールアドレスが異なる場合でも、別のユーザーがすでに使用しているメールアドレスを使用できません。例えば、別のユーザーが johndoe@example.com というメールアドレスを持っている場合、JohnDoe@example.com というメールアドレスを持つユーザーを作成することはできません。

## Workfront インスタンスの既存ユーザーのメールアドレスを更新

Workfront 管理者は、大文字と小文字が異なるだけで一致するメールアドレスを持つ既存のユーザーを更新する必要があります。
Workfront インスタンス内の重複したメールアドレスを修正するには、次の手順を実行します。

1. 重複したユーザーを調べて、どのユーザーが不要になったかを判断します。

   1. Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**ユーザー** を選択します。![](assets/users-icon-in-main-menu.png)

   1. **フィルター**&#x200B;メニューで、「**すべて**」を選択します。

   1. **表示**&#x200B;メニューで、**ユーザーログイン**&#x200B;を選択します。

   1. **グループ化**&#x200B;メニューで、**なし**&#x200B;を選択します。

   1. ユーザーログイン表示をカスタマイズします。

      1. **表示**／**ビューのカスタマイズ**&#x200B;をクリックします。

      1. **ID** 列を **メールアドレス** 列に置き換えます。

      1. ビューの名前を変更して保存。

   1. 新しいグループを作成。

      1. **グループ化**／**新しいグループ化**&#x200B;をクリックします。

      1. ページの右上隅にある&#x200B;**テキストモードに切り替える**&#x200B;をクリックします。
      1. 次のテキストモードコードを貼り付けます。

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. グループ名を変更し、保存します。

1. 次のいずれかの操作を行います。

   * （推奨されるメソッド）追加アカウントごとに、ユーザーのメールアドレスに + アドレスを追加します。

     組織内の 1 人のユーザーが複数のユーザーアカウントにアクセスする必要がある場合は、このオプションを選択します。メールプロバイダーでプラスアドレス指定がサポートされていない場合は、Workfront アカウントごとに個別のメールアカウントを提供する必要があります。

     例えば、John Doe というユーザーは、日常使用アカウント用に 1 つ、テスト目的で使用するユーザーアカウントを 1 つ持つことができます：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * 次のテキストをメールアドレスに追加して、偽のドメインを使用するようにドメインを変更します。

     `.inactive`

     例：John Doe というユーザーは次のドメインを持つことができます：（これらは一意である必要があります。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     パスワードのリセットには有効なメールアドレスが必要であるため、これらのアカウントにはログインできなくなります。これらのアカウントには、ログイン機能を使用する場合のみアクセスできます。

   * 不要なユーザーの削除

     >[!IMPORTANT]
     >
     >このオプションは、誤って作成されたアカウントまたはテストアカウントの場合にのみ選択してください。このオプションは通常、ログイン間違いが 0 または 1 つあるアカウントに対してのみ実行されます。定期的に使用されているアカウントは決して削除しないでください。

Workfront インスタンス内に大文字と小文字が異なるだけでメールアドレスが同じユーザーがいる場合、Workfront から追加のお知らせと変更が必要な期限をご連絡します。
