---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront と Workfront Proof 間のユーザー同期
description: ユーザー情報は、Adobe Workfront から Workfront Proof に同期されます。Workfront Proof から Workfront には同期されません。このため、ユーザーを作成または変更する際は常に Workfront 内で変更を加える必要があります。Workfront Proof 内でユーザーに変更を加えることはできません。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: ht
source-wordcount: '332'
ht-degree: 100%

---

# Adobe Workfront と Workfront Proof 間のユーザー同期

ユーザー情報は、Adobe Workfront から Workfront Proof に同期されます。Workfront Proof から Workfront には同期されません。このため、ユーザーを作成または変更する際は常に Workfront 内で変更を加える必要があります。Workfront Proof 内でユーザーに変更を加えることはできません。

以下の節では、Workfront から Workfront Proof へのユーザー同期に関する情報を提供します。

## 同期される情報

Workfront は、次のユーザー情報を Workfront Proof に同期します。

* 名前（ユーザーの姓名）
* メールアドレス

## 同期が発生するタイミング

次の状況になった場合、ユーザー情報が Workfront からWorkfront Proof に同期されます。

* ユーザーの情報が Workfront で更新される
* ユーザーが Workfront で作成される

Workfront Proof に同じメールアドレスを持つユーザーが存在するかどうかに応じて、次のいずれかが発生します。

* **一致するメールを持つユーザーが Workfront Proof に存在せず、**

   * **ユーザーに対してプルーフが有効になっている場合：**&#x200B;ユーザーが Workfront Proof でユーザーとして作成されます。
   * **次のユーザーに対してプルーフが有効になっていない場合：**&#x200B;ユーザーが Workfront Proof で連絡先として作成されます。

* **一致するメールを持つユーザーが Workfront Proof に存在する場合：** Workfront でそのユーザーのプルーフが有効になり（既に有効になっていない場合）、2 人のユーザー間で情報が同期されます。

  詳しくは、[ユーザーのプルーフアクセスの設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)内の[ユーザーのプルーフアクセスの設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)を参照してください。

  >[!IMPORTANT]
  >
  >一致するメールを持つユーザーが、ユーザー自身のまたは別のプルーフ環境に存在する場合、Workfront は、ユーザーのアカウント ID をメールの接尾辞として追加して、エイリアスメールアドレスを作成します。例：*username+accountid@domain.com*&#x200B;エイリアスメールが作成された場合でも、ユーザーにはプルーフが届きます。
