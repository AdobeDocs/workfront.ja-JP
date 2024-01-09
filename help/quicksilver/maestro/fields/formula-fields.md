---
title: 数式フィールドの概要
description: Adobeマエストロでは、関数と既存のフィールドを使用して新しいカスタム値を計算する数式フィールドを作成できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# 数式フィールドの概要

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--**********ADD TO miniTOC************>

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

既存のフィールドを参照し、数式でAdobeすると、カスタムフィールドを作成できます。 これをおこなうには、カスタムの数式タイプフィールドを作成します。

数式フィールドは、レコードタイプの他のフィールドの既存の値と、既存の値の計算方法を示す関数を使用して、新しい値を生成します。

詳しくは、 [フィールドの作成](../fields/create-fields.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

## 数式フィールドに関する考慮事項

* 数式フィールドは、同じレコードタイプに属するフィールドを参照します。 数式フィールドを作成する際に、他のレコードタイプのフィールドを参照することはできません。 <!--is this still accurate??-->
* 数式フィールドを保存した後で、そのフィールドの種類を変更することはできません。
* 数式フィールドを保存した後で、その計算を更新し、同じタイプのすべてのレコードに対して、計算結果を自動的に更新できます。
* リンクされたレコードタイプのルックアップフィールドは使用できません。
* Maestro インタフェースに表示される数式で参照するフィールドを追加する必要があります。

## サポートされる数式

Workfrontの計算フィールドからのすべての数式を使用できます。 詳しくは、 [計算データ式の概要](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

また、Maestro 数式フィールドでは、次の式を使用できます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>式</th> 
   <th>説明と例</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>区切り文字で連結された文字列を返します。</p> <p>式の形式は次のとおりです。

    ARRAYJOIN(delimiter,array)
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>一意の値を持つ配列を返します。</p> <p>式の形式は次のとおりです。

    ARRAYUNIQUE（配列）
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>日付と時刻のタイムゾーンを特定のタイムゾーンに設定します。</p> <p>式の形式は次のとおりです。

    SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>1 年の週の数を返します。必要に応じて、週の開始日を指定できます（日曜日は 1、月曜日は 2）。 省略した場合、週はデフォルトで日曜日に開始します。</p> <p>式の形式は次のとおりです。

    WEEKOFYEAR(date,2)
    または
    WEEKOFYEAR(date)
</p>
   </td></tr>

</table>





