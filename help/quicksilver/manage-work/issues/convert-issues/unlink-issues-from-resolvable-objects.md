---
product-area: projects
navigation-topic: convert-issues
title: 解決オブジェクトから問題のリンクを解除
description: イシューをプロジェクトまたはタスクに変換してプロジェクトまたはタスクを作成する場合は、元のイシューを保持するオプションがあります。 問題の変換時にこのオプションを使用するには、Adobe Workfrontの管理者がこの設定を有効にする必要があります。 問題をプロジェクトやタスクに変換する方法について詳しくは、「 Adobe Workfrontでの問題の変換の概要」を参照してください。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 解決オブジェクトから問題のリンクを解除

イシューをプロジェクトまたはタスクに変換してプロジェクトまたはタスクを作成する場合は、元のイシューを保持するオプションがあります。 問題の変換時にこのオプションを使用するには、Adobe Workfrontの管理者がこの設定を有効にする必要があります。\
問題をプロジェクトやタスクに変換する方法について詳しくは、 [Adobe Workfrontでの変換の問題の概要](../../../manage-work/issues/convert-issues/convert-issues.md).

プロジェクトまたはタスクに変換されたイシューを保持する場合、イシューの解決はプロジェクトまたはタスクに関連付けられます。 問題がプロジェクトまたはタスクの解決可能なオブジェクトになります。 プロジェクトまたはタスクは、イシューのオブジェクトの解決です。

問題を別の問題に手動でリンクすることもできます。 2 つ目の問題は、最初の問題（この場合は Resolving Object）になります。\
オブジェクトの解決の詳細については、 [オブジェクトの解決と解決の概要](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>問題のステータスは、[ 解決中のオブジェクト ] のステータスに応じて自動的に変化するので、変更できません。

イシューからプロジェクト、タスク、またはイシューを削除すると、イシューの解決のリンクをプロジェクト、タスク、またはイシューの解決のリンクを解除できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>問題へのアクセスを編集</p> <p>タスクおよびプロジェクトへのアクセスを表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>問題に関する権限の管理</p> <p>タスクまたはプロジェクトに対する権限を表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクト、タスクまたはイシューからイシューのリンクを解除する

1. プロジェクト、タスク、またはイシューにリンクされているイシューに移動します。
1. 次をクリック： **問題の詳細** 」セクションに入力します。
1. 次に移動： **概要** 領域 **問題の詳細** 」セクションに入力します。
1. 内 **解決者** フィールドで、解決可能なオブジェクトタイプを削除します。\
   イシューは、プロジェクト、タスクまたはイシューによって解決できます。

   これにより、問題の解決オブジェクトが削除されます。

1. クリック **保存** **変更点**.\
   問題がプロジェクト、タスクまたは問題にリンクされなくなり、問題を個別に解決できるようになりました。
