---
content-type: api
navigation-topic: general-api
title: イベント購読のバージョン管理
description: Event Subscription API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
TQID: https://experienceleague.adobe.com/cJnPxNppHK0lh8A6GQKNoUCCBrRUKdMvU3ym6zdHCXo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1055
ht-degree: 17%

---

# イベント登録のバージョン管理

Workfront には、2 つのバージョンのイベント登録があります。 この記事では、それらの違いについて説明します。

新しいバージョンは Workfront API に対する変更ではなく、イベント登録機能に対する変更です。

イベント登録のアップグレードまたはダウングレード機能により、イベントの構造に変更が加えられても既存の登録には影響せず、イベント登録を中断することなく新しいバージョンのテストとアップグレードができます。


イベント登録を別のバージョンにアップグレードまたはダウングレードすると、バージョン変更後 5 分間にわたって、イベント配信ごとに重複したイベントが配信されます。 重複したイベントには、イベント登録バージョン 1 とバージョン 2 がそれぞれ 1 つずつ含まれます。 これにより、イベント登録バージョンを変更しても、イベントを見落とすことがなくなります。

イベントサブスクリプションのアップグレードまたはダウングレードに使用されるエンドポイントについて詳しくは、「イベントサブスクリプション API」の「[&#x200B; イベントサブスクリプションのバージョン管理](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)」を参照してください。

>[!IMPORTANT]
>
>次のリリースは、イベントのサブスクリプションのバージョン管理に影響します。
>
>* **25.2 リリース** （2025年4月10日）: 25.2 リリース以降に作成されたすべての新しいサブスクリプションは、バージョン 2として作成されます。
>* **2026年1月15日**：残りのバージョン 1 サブスクリプションはすべてバージョン 2に移行されます。

## バージョン 1とバージョン 2の変更点

イベント サブスクリプション バージョン 2に対して、次の変更が行われました。


### 一般的な変更


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
   <th> <p><b>修復アクション</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>計算パラメーター値</p> </td> 
   <td> <p>計算されたパラメーター値を持つカスタムフォームを含むテンプレートから作成されたオブジェクトはすべて、<code>CREATE</code> イベントが送信され、次に<code>UPDATE</code>がパラメーター値（計算フィールドとその値を含む）とともに送信されます。 </p> </td> 
   <td> <p>計算されたパラメーター値を含むカスタムフォームを含むテンプレートからオブジェクトを作成する場合、<code>CREATE</code> イベントのみが送信され、計算フィールドを含むパラメーター値が含まれます。</p> </td> 
   <td> <p><code>UPDATE</code> イベントのサブスクリプションがあり、計算されたパラメーター値を使用してオブジェクトを作成した後に<code>UPDATE</code> イベントを受信することを想定している場合、その<code>UPDATE</code> イベントは受信されなくなります。 オブジェクトの作成時に計算パラメーター値を表示するには、追加の<code>CREATE</code> サブスクリプションを作成する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>複数選択テキストフィールド</p> </td> 
   <td> <p>複数選択タイプフィールドに変更を含む任意のタイプのイベントの場合、フィールドに1つの値のみが含まれている場合、変換され、文字列として送信されます。 それ以外の場合は、配列として送信されます。 </p><p>例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> は変換され、<code>myMultiSelectField: "oneValue"</code>として送信されます。</li><li><code>myMultiSelectField: ["first", "second"]</code> は<code>myMultiSelectField: ["first", "second"]</code>として送信されます。</li></ul> </td> 
   <td> <p>配列内の値の数に関係なく、配列として送信されます。 </p><p>例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> は<code>myMultiSelectField: ["oneValue"]</code>として送信されます。</li><li><code>myMultiSelectField: ["first", "second"]</code> は<code>myMultiSelectField: ["first", "second"]</code>として送信されます。</li></ul> </td> 
   <td> <p>複数選択フィールドにフィルターを含むサブスクリプションがあり、その値が文字列である場合は、その値を配列として持つ同じフィルターを使用して、新しいサブスクリプションを作成する必要があります。 </p> </td> 
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
   <th> <b>影響を受けるフィールド </b> </th> 
   <th> <b> バージョン 1 （以前の動作） </b></th> 
   <th> <b> バージョン 2 （変更） </b> </th> 
   <th> <b>修正アクション </b> </th> 
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
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されることが誤って表示されることがありました。</td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、これらのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他の値が変更された場合は表示されません。
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントに、影響を受けるフィールドが<code>null</code>から<code>object id</code>に変更されたことが誤って表示されました。 </td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、これらのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他の値が変更された場合は表示されません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>ドキュメントが削除された場合、<code>DELETE</code> イベントは、影響を受けるフィールドをbefore状態の空の配列として誤って表示しました。    </td> 
   <td><code>DELETE</code> イベントは、影響を受けるフィールドをbefore状態で正しく表示します。</td> 
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
   <td>このオブジェクトが更新されると、2つの<code>UPDATE</code> イベントが送信されます。 最初のイベントには影響を受けるフィールドが含まれず、2番目のイベントには含まれていました。</td> 
   <td>影響を受けるフィールドを含むすべてのフィールド更新は、1つの<code>UPDATE</code> イベントにのみ存在し、2つ目の不要なイベントは送信されません。     </td> 
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
   <td>任意のパラメーター値が経費で更新された場合、<code>UPDATE</code> イベントに誤って<code>EXPNS</code>から<code>PROJ</code>へのtopReferenceObjCodeの変更が表示され、<code>referenceObjectName</code>が<code>null</code>から<code>string value of project name</code>への変更が表示されました。      </td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、これらのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他の値が変更された場合は表示されません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>費用オブジェクトが削除されると、<code>DELETE</code> イベントが送信される前に、影響を受けるフィールドをnullに変更する<code>UPDATE</code> イベントが送信されました。    </td> 
   <td>追加の<code>UPDATE</code> イベントは送信されません。 <code>DELETE</code> イベントには、before状態の影響を受けるフィールドの正しい値があります。 </td> 
   <td><code>UPDATE</code> イベントの影響を受けるフィールドのフィルターがあり、オブジェクトが削除されたときに受信することを想定している場合は、その<code>UPDATE</code> イベントは受信されなくなります。オブジェクトが削除されたときにこれらのフィールドを表示するには、追加の<code>DELETE</code> サブスクリプションを作成する必要があります。
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
   <td>このオブジェクトが削除された場合、<code>DELETE</code> イベントは、影響を受けるフィールドを誤ってbefore状態の<code>null</code>として表示しました。 </td> 
   <td><code>DELETE</code> イベントは、影響を受けるフィールドをbefore状態で正しく表示します。</td> 
   <td>なし。 <code>DELETE</code> イベントは引き続き送信されますが、影響を受けるフィールドの正しいデータが表示されるようになりました。 </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントに、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されたことが誤って表示されました。 </td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、そのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他のパラメーター値が変更された場合は表示されません。
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
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されることが誤って表示されることがありました。</td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントに、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されたことが誤って表示されました。 </td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、そのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他のパラメーター値が変更された場合は表示されません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されることが誤って表示されることがありました。</td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、そのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他のパラメーター値が変更された場合は表示されません。
  </tr> 
  <tr> 
   <th rowspan="2">タスク</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトのパラメーター値が更新されると、<code>UPDATE</code> イベントに、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されたことが誤って表示されました。 </td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、そのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他のパラメーター値が変更された場合は表示されません。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>このオブジェクトが更新されると、<code>UPDATE</code> イベントで、影響を受けるフィールドが<code>null</code>から<code>ID value</code>に変更されることが誤って表示されることがありました。</td> 
   <td>すべての<code>UPDATE</code> イベントには、影響を受けるフィールドの正しい値が表示されます。</td> 
   <td>なし。影響を受けるフィールドにフィルターがある場合は、そのフィールドが実際に変更された場合にのみ<code>UPDATE</code> イベントが表示されます。他のパラメーター値が変更された場合は表示されません。
 </tbody> 
</table>


## Workfront Fusion シナリオでのイベントサブスクリプションバージョンの更新

Workfront Fusionでは、イベントサブスクリプションを使用して、Workfrontからトリガーへの変更を監視します。 Fusionがシナリオで直接使用するイベント購読バージョンを更新するには、Workfront/イベントペイロードバージョンを更新モジュールを使用します。

このモジュールの使用方法については、Workfront Fusion ドキュメントの[Workfront モジュール &#x200B;](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules)を参照してください。

ウェビナーの録画など、イベント登録のアップグレード中に Workfront Fusion シナリオを保持する方法について詳しくは、[イベント登録 V2 のアップグレード中の Fusion シナリオの保持](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/td-p/754182)を参照してください。
