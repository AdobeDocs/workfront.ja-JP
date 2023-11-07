---
content-type: api
product-area: user-management
navigation-topic: general-api
title: API を使用したユーザーの非アクティブ化
description: API を使用したユーザーの非アクティブ化
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# API を使用したユーザーの非アクティブ化

ユーザーが組織を離れた場合、そのユーザーを非アクティブ化して、Adobe Workfrontのライセンスを他のユーザーが利用できるようにし、誤って作業を割り当ててしまうのを防ぐことができます。 ユーザーを非アクティブ化すると、作業の割り当てや、メモ、時間、ドキュメントとの関連付けなど、作業履歴が保持されます。

ユーザーの非アクティブ化について詳しくは、 [ユーザーを非アクティブ化または再アクティブ化する](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Core API の使用について詳しくは、 [API の基本](../../wf-api/general/api-basics.md).

API を使用してユーザーを非アクティブ化するには：

1. 次の API リクエストを使用して API キーを生成します。

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 非アクティブ化するユーザーの GUID を見つけます。

   1. 次の API リクエストを使用して、システム内のすべてのユーザーの GUID を取得します。なお、 **isActive** フィールドショー **true** ( 現在アクティブで、 **false** 非アクティブ化されたユーザーの場合：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 非アクティブ化するユーザーの GUID を探すには、次を使用します。 **PUT** ユーザーの **isActive** フィールド値 **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 応答には、 **isActive** フィールド値が次の値から変更されました： **true** から **false**&#x200B;ユーザーが非アクティブ化されたことを示す：

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
