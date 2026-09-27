---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe WorkfrontとWorkfront Proof間のユーザーの同期
description: ユーザー情報は、Adobe Workfront から Workfront Proof に同期されます。Workfront Proof から Workfront には同期されません。 このため、ユーザーを作成または変更する際は常に Workfront 内で変更を加える必要があります。 Workfront Proof 内でユーザーに変更を加えることはできません。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
TQID: 'https://experienceleague.adobe.com/oHi8YTmAgh3KY1xfh6psNCLr4Gng0iniB3LUqbBzcOw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 97%
---
# Adobe Workfront と Workfront Proof 間のユーザー同期

ユーザー情報は、Adobe Workfront から Workfront Proof に同期されます。Workfront Proof から Workfront には同期されません。 このため、ユーザーを作成または変更する際は常に Workfront 内で変更を加える必要があります。 Workfront Proof 内でユーザーに変更を加えることはできません。

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
  >一致するメールを持つユーザーが、ユーザー自身のまたは別のプルーフ環境に存在する場合、Workfront は、ユーザーのアカウント ID をメールの接尾辞として追加して、エイリアスメールアドレスを作成します。 例：*username+accountid@domain.com* エイリアスメールが作成された場合でも、ユーザーにはプルーフが届きます。
