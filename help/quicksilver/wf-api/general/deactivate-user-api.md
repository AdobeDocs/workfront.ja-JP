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
workflow-type: ht
source-wordcount: '199'
ht-degree: 100%

---


# API を使用したユーザーの非アクティブ化

ユーザーが組織を離れた場合は、そのユーザーを非アクティブ化することで、そのユーザーが使用していた Adobe Workfront ライセンスを他のユーザーが利用できるようにし、誤ってそのユーザーに作業を割り当ててしまうのを防ぐことができます。ユーザーを非アクティブ化すると、作業の割り当てや、メモ、時間およびドキュメントとの関連付けなど、そのユーザーの作業履歴が保持されます。

ユーザーの非アクティブ化について詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。

コア API の使用については、[API の基本](../../wf-api/general/api-basics.md)を参照してください。

API を使用してユーザーを非アクティブ化するには、次の手順に従います。

1. 次の API リクエストを使用して API キーを生成します。

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 非アクティブ化するユーザーの GUID を見つけます。

   1. 次の API リクエストを使用して、システム内のすべてのユーザーの GUID を取得します。なお、現在アクティブなユーザーの場合は **isActive** フィールドは **true** を示し、現在非アクティブなユーザーの場合は **false** を示します。

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 非アクティブ化するユーザーの GUID を見つけ、次の **PUT** リクエストを使用してユーザーの **isActive** フィールドの値を **false** に変更します。

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. **isActive** フィールドの値が **true** から **false** に変わったことを応答が示します。これにより、ユーザーが非アクティブ化されたことがわかります。

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
