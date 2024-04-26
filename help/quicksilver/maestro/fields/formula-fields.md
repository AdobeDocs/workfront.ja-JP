---
title: 数式フィールドの概要
description: Adobe Workfront Planning では、関数と既存のフィールドを使用して新しいカスタム値を計算する式フィールドを作成できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 38%

---

# 数式フィールドの概要

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{maestro-important-intro}}

既存のフィールドを参照し、式タイプのフィールドで接続することで、Adobe Workfront Planning でカスタムフィールドを作成できます。

数式フィールドは、レコードタイプの他のフィールドの既存の値と、既存の値の計算方法を示す関数を使用して、新しい値を生成します。

詳しくは、記事の「式」の節を参照してください [フィールドの作成](../fields/create-fields.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning ベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Workfront の計画用のアクセス制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限を管理</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## 式フィールドに関する考慮事項

* 式フィールドは、同じレコードタイプに属するフィールドを参照します。 式フィールドを作成するときに、他のレコードタイプのフィールドを参照することはできません。 <!--is this still accurate??-->
* 式フィールドを保存した後で、そのフィールド タイプを変更することはできません。
* 式フィールドを保存した後に計算を更新すると、同じタイプのすべてのレコードに対する計算結果が自動的に更新されます。
* Workfront Planning インタフェースに表示される式で参照するフィールドを追加する必要があります。

## サポートされる式

Adobe Workfront Planning の式フィールドでは、Workfrontの計算フィールドからのすべての式をサポートしています。 詳しくは、を参照してください [計算データ式の概要](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

さらに、Workfront Planning 式フィールドでは、次の式をサポートしています：

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
   <td> <p>区切り文字によって連結された文字列を返します。</p> <p>式の形式は次のとおりです。

<code>ARRAYJOIN （delimiter,array）</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>一意の値を持つ配列を返します。</p> <p>式の形式は次のとおりです。

<code>ARRAYUNIQUE （array）</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>レコードの ID を返します。 各レコードには一意の ID があります。</p> <p>式の形式は次のとおりです。

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>日時のタイムゾーンを特定のタイムゾーンに設定します。</p> <p>式の形式は次のとおりです。

<code>SETTIMEZONE （date,&#39;アメリカ/ロサンゼルス&#39;）</code>
</p>
   </td></tr>

<tr> 
   <td><strong>平年</strong> </td> 
   <td> <p>年の週数を返します。必要に応じて、週の開始日を指定できます (日曜日の場合は 1、月曜日の場合は 2 を使用)。省略した場合、デフォルトでは週は日曜日に開始します。</p> <p>式の形式は次のとおりです。

<code>WEEKOFYEAR （date,2）</code>
または
<code>WEEKOFYEAR （date）</code>
</p>
   </td></tr>

</table>
