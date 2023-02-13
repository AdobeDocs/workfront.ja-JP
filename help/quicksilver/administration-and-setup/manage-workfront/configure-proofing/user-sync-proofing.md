---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe WorkfrontとWorkfrontの配達確認間のユーザー同期
description: ユーザー情報がAdobe WorkfrontからWorkfront配達確認に同期される。Workfront Proof からWorkfrontには同期されません。 このため、ユーザーを作成または変更する際は常にWorkfront内で変更を加える必要があります。 Workfront Proof 内でユーザーに変更を加えることはできません。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe WorkfrontとWorkfrontの配達確認間のユーザー同期

ユーザー情報がAdobe WorkfrontからWorkfront配達確認に同期される。Workfront Proof からWorkfrontには同期されません。 このため、ユーザーを作成または変更する際は常にWorkfront内で変更を加える必要があります。 Workfront Proof 内でユーザーに変更を加えることはできません。

以下の節では、WorkfrontからWorkfront Proof へのユーザー同期に関する情報を提供します。

## 同期される情報

Workfrontは、次のユーザー情報をWorkfront Proof に同期します。

* 名前（ユーザーの姓名）
* メールアドレス

## 同期が発生した場合

次の状況で、ユーザー情報がWorkfrontからWorkfront Proof に同期されます。

* ユーザーの情報がWorkfrontで更新される
* ユーザーがWorkfrontで作成される

Workfront Proof に同じ E メールアドレスを持つユーザーが存在するかどうかに応じて、次のいずれかが発生します。

* **一致する E メールを持つユーザーがWorkfrontの配達確認に存在せず、**

   * **ユーザーに対して校正が有効になっています：** ユーザーがWorkfrontの配達確認でユーザーとして作成されます。
   * **次のユーザーに対しては、校正機能が有効になっていません：** ユーザーがWorkfrontの配達確認で連絡先として作成されます。

* **一致する E メールを持つユーザーがWorkfrontの配達確認に存在する場合：** Workfrontでそのユーザーの校正が有効になって（有効になっていない場合）、2 人のユーザー間で情報が同期されます。

   詳しくは、 [ユーザーの校正アクセスを設定する](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [ユーザーの校正アクセスを設定する](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >一致する E メールを持つユーザーが、独自の検証環境または別の検証環境に存在する場合、Workfrontは、ユーザーのアカウント ID を E メールのサフィックスとして追加して、エイリアス E メールアドレスを作成します。 例： *username+accountid@domain.com*. エイリアス E メールが作成された場合でも、ユーザーには配達確認通知が届きます。
