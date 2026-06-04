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
TQID: https://experienceleague.adobe.com/GRPtXFkFhNHHeKMY0I05ckqLLwqsVzNCKY8wHLMaOpQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 189
ht-degree: 80%

---

# API を使用したユーザーの非アクティブ化

ユーザーが組織を離れた場合は、そのユーザーを非アクティブ化することで、そのユーザーが使用していた Adobe Workfront ライセンスを他のユーザーが利用できるようにし、誤ってそのユーザーに作業を割り当ててしまうのを防ぐことができます。 ユーザーを非アクティブ化すると、作業の割り当てや、メモ、時間およびドキュメントとの関連付けなど、そのユーザーの作業履歴が保持されます。

ユーザーの非アクティブ化について詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。

コア API の使用については、[API の基本](../../wf-api/general/api-basics.md)を参照してください。

API を使用してユーザーを非アクティブ化するには、次の手順に従います。

1. 次の API リクエストを使用して API キーを生成します。

   ```
   <domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
   ```

1. 非アクティブ化するユーザーの GUID を見つけます。

   次の API リクエストを使用して、システム内のすべてのユーザーの GUID を取得します。なお、現在アクティブなユーザーの場合は **isActive** フィールドは **true** を示し、現在非アクティブなユーザーの場合は **false** を示します。

   ```
   <domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
   ```

1. 次の&#x200B;**PUT** リクエストを使用して、ユーザーの&#x200B;**isActive** フィールド値を&#x200B;**false**&#x200B;に変更します。

   ```
   <domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
   ```

1. 応答は、**isActive** フィールドの値が&#x200B;**true**&#x200B;から&#x200B;**false**&#x200B;に変更され、ユーザーが非アクティブ化されたことを示します。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
