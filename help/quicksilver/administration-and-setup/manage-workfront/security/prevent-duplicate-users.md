---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 重複するユーザーを防ぐ
description: Adobe Workfrontで新しいユーザーを作成する場合、電子メールアドレスが大文字と小文字で異なる場合 (JohnDoe@example.comやjohndoe@example.comなど ) でも、別のユーザーが既に使用している電子メールアドレスを使用できなくなりました。 また、今後の認証の強化に備えて、すべてのユーザーがWorkfrontインスタンス内で一意の E メールアドレスを持つようにします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 重複するユーザーを防ぐ

Adobe Workfrontで新しいユーザーを作成する場合、電子メールアドレスが大文字と小文字で異なる場合 (JohnDoe@example.comやjohndoe@example.comなど ) でも、別のユーザーが既に使用している電子メールアドレスを使用できなくなりました。 また、今後の認証の強化に備えて、すべてのユーザーがWorkfrontインスタンス内で一意の E メールアドレスを持つようにします。

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
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 一意の電子メールアドレスを持つユーザーの作成

2019.4 リリース以降、Workfrontで新しいユーザーを作成する際に、別のユーザーが既に使用している電子メールアドレスを使用できなくなりました。電子メールアドレスが大文字と小文字で異なる場合も同様です。 例えば、別のユーザーの電子メールアドレスがJohnDoe@example.comである場合、その電子メールアドレスをjohndoe@example.comとするユーザーを作成することはできません。

## Workfrontインスタンスの既存ユーザーの電子メールアドレスを更新する

Workfront管理者は、大文字と小文字のみが異なる、一致する E メールアドレスを持つ既存のユーザーを更新する必要があります。
Workfrontインスタンス内で重複した E メールアドレスを修正するには：

1. 重複するユーザーを調べて、不要になったユーザーを特定します。

   1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **ユーザー**. ![](assets/users-icon-in-main-menu.png)

   1. 内 **フィルター** メニュー、選択 **すべて**.

   1. 内 **表示** メニュー、選択 **ユーザーログイン**.

   1. 内 **グループ化** メニュー、選択 **なし**.

   1. 「ユーザーログイン」表示をカスタマイズします。

      1. クリック **表示** > **表示をカスタマイズ**.

      1. を **ID** 列に **電子メールアドレス** 列。

      1. ビューの名前を変更して保存します。
   1. 新しいグループを作成します。

      1. クリック **グループ化** > **新しいグループ化**.

      1. クリック **テキストモードに切り替え** をクリックします。
      1. 次のテキストモードコードを貼り付けます。

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. グループ名を変更し、保存します。



1. 次のいずれかの操作を行います。

   * （推奨される方法）追加の各アカウントについて、ユーザーの電子メールアドレスに+アドレスを追加します。

      組織内の 1 人のユーザーが複数のユーザーアカウントにアクセスする必要がある場合は、このオプションを選択します。 お使いの電子メールプロバイダーでプラスアドレス指定がサポートされていない場合は、Workfrontアカウントごとに別の電子メールアカウントを提供する必要があります。

      例えば、John Doe は、毎日使用するアカウントに 1 つのユーザーアカウントを割り当て、テスト目的に 1 つを使用することができます。

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * E メールアドレスに次のテキストを追加して、フェイクドメインを使用するようにドメインを変更します。

      `.inactive`

      例えば、John Doe が次のドメインを持っているとします。（一意である必要があります）。

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      パスワードのリセットには有効な電子メールアドレスが必要なので、これらのアカウントにログインできなくなりました。 これらのアカウントには、ログイン名機能を使用してのみアクセスできます。

   * 不要なユーザーの削除

      >[!IMPORTANT]
      >
      >このオプションは、誤って作成されたアカウントまたはテストアカウントに対してのみ選択します。 このオプションは、通常、ログインがゼロまたは 1 回誤った場合にのみ実行されます。 定期的に使用されているアカウントは削除しないでください。



Workfrontインスタンスのユーザーが、大文字と小文字の違いによって異なる電子メールアドレスを持つ場合、Workfrontから、追加情報とタイムラインを、それらのユーザーを更新する必要が生じた際に連絡が来ます。
