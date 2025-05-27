---
content-type: api
navigation-topic: general-api
title: イベント購読のバージョン管理
description: Event Subscription API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: f34f48d974db200d9ce1815c805885707ab27f6d
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 1%

---

# イベント購読のバージョン管理

Workfrontには、2 つのバージョンのイベント購読があります。 この記事では、これらの違いについて説明します。

新しいバージョンはWorkfront API に対する変更ではなく、イベント購読機能に対する変更です。

イベント購読をアップグレードまたはダウングレードする機能により、イベントの構造に変更が加えられても既存の購読が壊れずに、イベント購読に隙間なく新しいバージョンのテストとアップグレードが可能になります。


イベント購読を別のバージョンにアップグレードまたはダウングレードすると、バージョン変更後 5 分間、イベント配信ごとに重複したイベントが届きます。 重複には、イベント購読バージョン 1 とバージョン 2 がそれぞれ 1 つずつ含まれます。 これにより、イベント購読バージョンの変更に伴うイベントが見逃されなくなります。

イベント購読のアップグレードまたはダウングレードに使用されるエンドポイントについて詳しくは、イベント購読 API 記事の [ イベント購読のバージョン管理 ](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) を参照してください。

>[!IMPORTANT]
>
>次のリリースは、イベント購読のバージョン管理に影響します。
>
>* **25.2 リリース** （2025 年 4 月 10 日（PT））:25.2 リリース以降に作成された新しいサブスクリプションはすべて、バージョン 2 として作成されます。
>* **2026 年 1 月 15 日**：残りのすべてのバージョン 1 サブスクリプションがバージョン 2 に移行されます。

## バージョン 1 とバージョン 2 の間の変更

イベント購読バージョン 2 に対して次の変更が行われました。


### 一般的な変更点


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>影響を受けるフィールド</b></p> </th> 
   <th> <p><b>バージョン 1 （以前の動作）</b></p> </th> 
   <th> <p><b>バージョン 2 （変更）</b></p> </th> 
   <th> <p><b>修正アクション</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>計算されたパラメーター値</p> </td> 
   <td> <p>計算されたパラメーター値を含むカスタムフォームを含むテンプレートから作成されたオブジェクトの場合、<code>CREATE</code> イベントが送信された後に、パラメーター値（計算フィールドとその値を含む）を含む <code>UPDATE</code> が送信されます。 </p> </td> 
   <td> <p>計算されたパラメーター値を持つカスタムフォームを含むテンプレートからオブジェクトが作成された場合、<code>CREATE</code> イベントのみが送信され、計算フィールドを含むパラメーター値が含まれます。</p> </td> 
   <td> <p><code>UPDATE</code> イベントの購読があり、計算されたパラメーター値でオブジェクトを作成した後に <code>UPDATE</code> イベントを受け取る予定がある場合、その <code>UPDATE</code> イベントは受け取らなくなります。 オブジェクトの作成時に計算されたパラメーター値を表示する場合は、追加の <code>CREATE</code> サブスクリプションを作成する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>複数選択タイプフィールド</p> </td> 
   <td> <p>複数選択タイプのフィールドに対する変更を含むイベントタイプの場合、フィールドに値が 1 つしか含まれていなければ、変換されて文字列として送信されます。 それ以外の場合は、配列として送信されます。 </p><p>例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> は変換され、<code>myMultiSelectField: "oneValue"</code> として送信されます。</li><li><code>myMultiSelectField: ["first", "second"]</code> は <code>myMultiSelectField: ["first", "second"]</code> として送信されます。</li></ul> </td> 
   <td> <p>配列内の値の数に関係なく、配列として送信されます。 </p><p>例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> は <code>myMultiSelectField: ["oneValue"]</code> として送信されます。</li><li><code>myMultiSelectField: ["first", "second"]</code> は <code>myMultiSelectField: ["first", "second"]</code> として送信されます。</li></ul> </td> 
   <td> <p>複数選択フィールドに対するフィルターを持つ購読があり、値を文字列とする場合、値を配列として持つのと同じフィルターを持つ新しい購読を作成する必要があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### オブジェクト固有の変更

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b> オブジェクトコード </b> </th> 
   <th> <b> 影響を受けるフィールド </b> </th> 
   <th> <b> バージョン 1 （以前の動作） </b></th> 
   <th> <b> バージョン 2 （変更） </b> </th> 
   <th> <b> 是正措置 </b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されることが誤って表示されることがありました。</td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、<code>UPDATE</code> のイベントは、これらのフィールドが実際に変更された場合にのみ受け取り、その他の値が変更された場合には受け取りません。
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>object id</code> に変更されたことが誤って表示されていました。 </td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、<code>UPDATE</code> のイベントは、これらのフィールドが実際に変更された場合にのみ受け取り、その他の値が変更された場合には受け取りません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>ドキュメントが削除されると、<code>DELETE</code> イベントで、影響を受けるフィールドが事前状態の空の配列として誤って表示されていました。    </td> 
   <td><code>DELETE</code> イベントは、影響を受けるフィールドを事前状態で正しく表示します。</td> 
   <td>なし。<code>DELETE</code> イベントは引き続き送信されますが、影響を受けるフィールドの正しいデータが表示されるようになりました。 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、2 つの <code>UPDATE</code> イベントが送信されます。 最初のイベントには影響を受けるフィールドは含まれませんでしたが、2 番目のイベントには含まれていました。</td> 
   <td>影響を受けるフィールドを含むすべてのフィールド更新が 1 つの <code>UPDATE</code> イベントにのみ存在し、2 つ目の不要なイベントは送信されません。     </td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、イベントは最初のイベントで配信されます。 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>任意のパラメーター値が費用で更新された場合、<code>UPDATE</code> イベントで、topReferenceObjCode が <code>EXPNS</code> から <code>PROJ</code> に変更され、<code>referenceObjectName</code> が <code>null</code> から <code>string value of project name</code> に変更されたことが誤って表示されていました。      </td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、<code>UPDATE</code> のイベントは、これらのフィールドが実際に変更された場合にのみ受け取り、その他の値が変更された場合には受け取りません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>費用オブジェクトが削除されると、<code>UPDATE</code> イベントが送信され、<code>DELETE</code> イベントが送信される前に、影響を受けるフィールドが null に変更されました。    </td> 
   <td>追加の <code>UPDATE</code> イベントは送信されません。 <code>DELETE</code> イベントには、before 状態の影響を受けるフィールドに対する正しい値があります。 </td> 
   <td><code>UPDATE</code> イベントの影響を受けるフィールドのフィルターがあり、オブジェクトが削除されたときに受け取ることを期待していた場合、その <code>UPDATE</code> イベントは受け取らなくなります。 オブジェクトの削除時にこれらのフィールドを表示する場合は、追加の <code>DELETE</code> サブスクリプションを作成する必要があります。
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">時間</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが削除されると、<code>DELETE</code> イベントで、影響を受けるフィールドが <code>null</code> のように誤って表示されていました。 </td> 
   <td><code>DELETE</code> イベントは、影響を受けるフィールドを事前状態で正しく表示します。</td> 
   <td>なし。<code>DELETE</code> イベントは引き続き送信されますが、影響を受けるフィールドの正しいデータが表示されるようになりました。 </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されたことが誤って表示されていました。 </td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、そのフィールドが実際に変更された場合にのみ <code>UPDATE</code> イベントが返され、他のパラメーター値が変更された場合には返されません。
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されることが誤って表示されることがありました。</td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されたことが誤って表示されていました。 </td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、そのフィールドが実際に変更された場合にのみ <code>UPDATE</code> イベントが返され、他のパラメーター値が変更された場合には返されません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されることが誤って表示されることがありました。</td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、そのフィールドが実際に変更された場合にのみ <code>UPDATE</code> イベントが返され、他のパラメーター値が変更された場合には返されません。
  </tr> 
  <tr> 
   <th rowspan="2">タスク</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されたことが誤って表示されていました。 </td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、そのフィールドが実際に変更された場合にのみ <code>UPDATE</code> イベントが返され、他のパラメーター値が変更された場合には返されません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが <code>null</code> から <code>ID value</code> に変更されることが誤って表示されることがありました。</td> 
   <td>すべての <code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合、そのフィールドが実際に変更された場合にのみ <code>UPDATE</code> イベントが返され、他のパラメーター値が変更された場合には返されません。
 </tbody> 
</table>


## Workfront Fusion シナリオのイベント購読バージョンの更新

Workfront Fusion は、イベント購読を使用して、トリガーシナリオに対するWorkfrontの変化を監視します。 Fusion がシナリオで直接使用するイベント購読のバージョンは、Workfront/イベントのペイロードバージョンを更新モジュールを使用して更新できます。

このモジュールの使用方法については、Workfront Fusion ドキュメントの [Workfront モジュール ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules) を参照してください。

ウェビナーの録画など、イベント購読のアップグレード中にWorkfront Fusion シナリオを保持する方法については、[ イベント購読 V2 のアップグレード中に Fusion シナリオを保持する ](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/td-p/754182?profile.language=ja) を参照してください。
