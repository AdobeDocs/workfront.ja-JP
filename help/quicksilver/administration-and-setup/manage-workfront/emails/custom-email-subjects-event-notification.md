---
navigation-topic: notifications
title: イベント通知用のメール件名のカスタマイズ
description: イベント通知でトリガーされるメールの件名行をカスタマイズできます。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 86%

---

# イベント通知のメールの件名をカスタマイズ

イベント通知でトリガーされるメールの件名行をカスタマイズできます。

件名行を変更すると、受信者のアクセスレベルに関係なく、システム内のすべてのユーザーに影響します。メールの件名に含まれるすべてのオブジェクトとフィールドが、ユーザーに表示されます。

一部のイベント通知には複数の件名が含まれています。つまり、これらのイベント通知には、その機能に基づいて複数のメール件名を含めることができます。

>[!IMPORTANT]
>
>件名行が複数のオブジェクトを参照している場合は、デフォルトのフィールドを削除する際に注意してください。以下は、そのような件名行を含むイベント通知のリストです。
>
>* 自分が更新を受信する対象者として追加されました
>* 自分のチームが更新を受信する対象として追加されました
>* スレッド参加者に対する作業アイテムコメント
>* 作業アイテムの割り当て先に対する作業アイテムコメント
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>リマインダー通知への管理アクセス権を持つ、プランナー以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イベント通知のメールの件名行をカスタマイズ {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. 左側のパネルで、**メール**／**通知**&#x200B;をクリックします。

1. 「**イベント通知**」タブをクリックします。
1. カスタマイズするイベント通知の名前をクリックして、**イベント通知**&#x200B;ボックスを開きます。
1. **メールの件名行**&#x200B;ボックスで、メールの件名のテキストおよびフィールド（カスタムフィールドを含む）を変更します。

   追加されたフィールドの名前は、データベース構造のキャメルケース構文と一致する必要があります。<!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. 「**アップデート**」をクリックして、メールの新しい件名行を保存します。

## 複数オブジェクトのメールのメール件名行をカスタマイズ

一部のイベント通知には、トリガーされるオブジェクトに応じて、複数の件名があります。

例えば、「自分が更新を受信する対象者として追加されました」には 2 つの異なる件名行があります。1 つ目はタスク、イシュー、テンプレートタスクおよびドキュメント（「referenceObject」とも呼ばれる）に関するもので、2 つ目はオブジェクト（「topReferenceObject」とも呼ばれる）に関するもので、これはユーザーがポートフォリオ、プログラムなどのコメントを作成できるようにするものです。

![ イベントの件名が複数ではありません ](assets/ev-multiple-subject.png)

タスク、イシュー、テンプレートタスクやドキュメントに関する会話にユーザーが含まれる場合は、最初の件名行を含むメールが生成されます。件名には「referenceObject:name」が含まれ、システムによってオブジェクトが定義され、件名フィールドに適切な名前が表示されます。 メールの件名行は、「プロジェクト ABC 上のタスク 123 についてのコメント」のようになります。

プロジェクトの会話に追加すると、2 番目の件名のメールが生成されます。ここで、件名には「topReferenceObject:name」が含まれており、Workfrontはどのオブジェクトが参照されたかを再度識別し、件名に「topReferenceObject:name」ではなくオブジェクト名を返します。 メールの件名行は、「プロジェクト ABC についてのコメント」のようになります。

メールの件名行を編集し、どちらかの件名行にフィールドを追加するには、この記事にある[イベント通知のメール件名行をカスタマイズ](#customize-email-subject-lines-for-event-notifications)を参照してください。

## 複数アクションのメールのメール件名行をカスタマイズ

一部のイベント通知には、オブジェクトに対して実行される様々なアクションの概要を示す複数のメール件名もあります。

例えば、ドキュメントをイシューに追加するリクエストは、2 種類の異なるメールをトリガーできるイベントです。1 つはドキュメントの追加時、もう 1 つはドキュメントの編集時です。



![ イベントの件名が複数ではありません ](assets/Ev-not-mult-subj-lines.png)

メールの件名行を編集し、どちらかの件名行にフィールドを追加するには、この記事にある[イベント通知のメール件名行をカスタマイズ](#customize-email-subject-lines-for-event-notifications)を参照してください。
