---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: ' [!DNL Adobe Workfront Fusion] における日時書式設定のトークン'
description: 日時書式設定の次のトークンが [!DNL Adobe Workfront Fusion mapping] パネルで使用可能です。
author: Becky
feature: Workfront Fusion
exl-id: 19d0608e-7902-4d09-b71d-e6ae8ed7a6fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '365'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] における日時書式設定のトークン

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を、組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 年、月、日のトークン

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>トークン </th> 
   <th>出力 </th> 
   <th> <p>説明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>YY </code> </td> 
   <td><code>70 71 ... 29 30</code> </td> 
   <td> <p> 2 桁の年</p> </td> 
  </tr> 
  <tr> 
   <td><code>YYYY </code> </td> 
   <td><code>1970 1971 ... 2029 2030 </code> </td> 
   <td> <p>4 桁の年</p> </td> 
  </tr> 
  <tr> 
   <td><code>Y</code> </td> 
   <td><code>1970 1971 ... 9999 +10000 +10001</code> </td> 
   <td> <p>[!UICONTROL Year with any number of digits and sign]</p> </td> 
  </tr> 
  <tr> 
   <td><code>Q</code> </td> 
   <td><code>1 2 3 4 </code> </td> 
   <td> <p> 四半期</p> </td> 
  </tr> 
  <tr> 
   <td><code>Qo</code> </td> 
   <td><code>1st 2nd 3rd 4th </code></td> 
   <td> <p>四半期（序数付き）</p> </td> 
  </tr> 
  <tr> 
   <td><code>M</code> </td> 
   <td><code>1 2 ... 11 12</code></td> 
   <td> <p>月の数字</p> </td> 
  </tr> 
  <tr> 
   <td><code>Mo </code> </td> 
   <td><code>1st 2nd ... 11th 12th</code> </td> 
   <td> <p>[!UICONTROL Month]（序数付き）</p> </td> 
  </tr> 
  <tr> 
   <td><code>MM</code> </td> 
   <td><code>01 02 ... 11 12 </code> </td> 
   <td> <p> 月番号（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMM</code> </td> 
   <td><code>Jan Feb ... Nov Dec</code></td> 
   <td> <p> 月名の省略形</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMMM</code> </td> 
   <td><code> January February ... November December</code> </td> 
   <td> <p> 月名</p> </td> 
  </tr> 
  <tr> 
   <td><code>D</code> </td> 
   <td><code>1 2 ... 30 31 </code></td> 
   <td> <p>日</p> </td> 
  </tr> 
  <tr> 
   <td><code>Do</code> </td> 
   <td><code>1st 2nd ... 30th 31st</code></td> 
   <td> <p> 序数付きの月の日</p> </td> 
  </tr> 
  <tr> 
   <td><code>DD</code> </td> 
   <td><code>01 02 ... 30 31</code></td> 
   <td> <p> 月の日（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDD</code> </td> 
   <td><code>1 2 ... 364 365 </code></td> 
   <td> <p>通日</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDo</code> </td> 
   <td><code>1st 2nd ... 364th 365th</code> </td> 
   <td> <p>[!UICONTROL Day of year]（序数付き）</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDD </code> </td> 
   <td><code>001 002 ... 364 365</code> </td> 
   <td> <p> 年間通算日（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
 </tbody> 
</table>

## 週年、週、週日のトークン

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>トークン </th> 
   <th>出力 </th> 
   <th> <p>説明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>d</code> </td> 
   <td><code>0 1 ... 5 6 </code> </td> 
   <td> <p> 曜日</p> </td> 
  </tr> 
  <tr> 
   <td><code>do</code> </td> 
   <td><code>0th 1st ... 5th 6th </code> </td> 
   <td> <p>[!UICONTROL Day of week with ordinal]</p> </td> 
  </tr> 
  <tr> 
   <td><code>dd </code> </td> 
   <td><code>Su Mo ... Fr Sa </code> </td> 
   <td> <p>曜日の省略形</p> </td> 
  </tr> 
  <tr> 
   <td><code>ddd</code> </td> 
   <td><code>Sun Mon ... Fri Sat </code> </td> 
   <td> <p> 曜日の省略形</p> </td> 
  </tr> 
  <tr> 
   <td><code>dddd </code> </td> 
   <td><code>Sunday Monday ... Friday Saturday</code> </td> 
   <td> <p> 曜日名</p> </td> 
  </tr> 
  <tr> 
   <td><code>E</code> </td> 
   <td><code>1 2 ... 6 7 </code> </td> 
   <td> <p> 曜日（ISO）</p> </td> 
  </tr> 
  <tr> 
   <td><code>w </code> </td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>年間通算週</p> </td> 
  </tr> 
  <tr> 
   <td><code>wo </code> </td> 
   <td><code>1st 2nd ... 52nd 53rd</code> </td> 
   <td> <p>[!UICONTROL Week of year with ordinal]</p> </td> 
  </tr> 
  <tr> 
   <td><code>ww </code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p>年間通算週（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>W</code></td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>年間通算週（ISO）</p> </td> 
  </tr> 
  <tr> 
   <td><code>Wo</code> </td> 
   <td><code>1st 2nd ... 52nd 53rd </code> </td> 
   <td> <p> 序数付きの年間通算週（ISO）</p> </td> 
  </tr> 
  <tr> 
   <td><code>WW</code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p> 先頭のゼロで桁揃えした年間通算週（ISO）</p> </td> 
  </tr> 
  <tr> 
   <td><code>gg</code></td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>年間通算週</p> </td> 
  </tr> 
  <tr> 
   <td><code>gggg </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> 年間通算週</p> </td> 
  </tr> 
  <tr> 
   <td><code>GG </code> </td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>年間通算週（ISO）</p> </td> 
  </tr> 
  <tr> 
   <td><code>GGGG </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> 年間通算週（ISO）</p> </td> 
  </tr> 
 </tbody> 
</table>

## 時間、分、秒、ミリ秒、オフセットのトークン

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>トークン </p> </th> 
   <th>出力 </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>H</code> </td> 
   <td><code>0 1 ... 22 23</code></td> 
   <td> <p>24 時間表示の時</p> </td> 
  </tr> 
  <tr> 
   <td><code>HH</code> </td> 
   <td><code>00 01 ... 22 23</code></td> 
   <td> <p> 24 時間表示の時（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>h</code> </td> 
   <td><code>1 2 ... 11 12</code></td> 
   <td> <p> 12 時間表示の時</p> </td> 
  </tr> 
  <tr> 
   <td><code>hh </code> </td> 
   <td><code>01 02 ... 11 12</code> </td> 
   <td> <p> 12 時間表示の時（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>k</code> </td> 
   <td><code>1 2 ... 23 24</code></td> 
   <td> <p> 24 時間表示の時</p> </td> 
  </tr> 
  <tr> 
   <td><code>kk</code></td> 
   <td><code>01 02 ... 23 24</code> </td> 
   <td> <p> 24 時間表示の時（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>A</code></td> 
   <td><code>AM PM </code> </td> 
   <td> <p>PM または AM（大文字）</p> </td> 
  </tr> 
  <tr> 
   <td><code>a</code> </td> 
   <td><code>am pm </code> </td> 
   <td> <p> pm または am（小文字）</p> </td> 
  </tr> 
  <tr> 
   <td><code>m</code> </td> 
   <td><code> 0 1 ... 58 59</code> </td> 
   <td> <p> 分</p> </td> 
  </tr> 
  <tr> 
   <td><code>mm</code> </td> 
   <td><code>00 01 ... 58 59</code> </td> 
   <td> <p>[!UICONTROL Minutes with]（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>s</code> </td> 
   <td><code>0 1 ... 58 59</code> </td> 
   <td> <p> 秒</p> </td> 
  </tr> 
  <tr> 
   <td><code>ss</code> </td> 
   <td><code>00 01 ... 58 59</code></td> 
   <td> <p>秒（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>S</code> </td> 
   <td><code>0 1 ... 8 9 </code> </td> 
   <td> <p> 分数秒</p> </td> 
  </tr> 
  <tr> 
   <td><code>SS</code> </td> 
   <td><code>00 01 ... 98 99</code> </td> 
   <td> <p> 小数点以下の秒（先頭のゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSS</code> </td> 
   <td><code>000 001 ... 998 999</code> </td> 
   <td> <p> 小数点以下の秒（先頭の 2 つのゼロで桁揃え）</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSSS ... SSSSSSSSS</code> </td> 
   <td><code>000[0..] 001[0..] ... 998[0..] 999[0..] </code> </td> 
   <td> <p> 分数秒</p> </td> 
  </tr> 
  <tr> 
   <td><code>Z</code> </td> 
   <td><code>-07:00 -06:00 ... +06:00 +07:00 </code></td> 
   <td> <p>タイムゾーン</p> </td> 
  </tr> 
  <tr> 
   <td><code>ZZ</code> </td> 
   <td><code>-0700 -0600 ... +0600 +0700 </code></td> 
   <td> <p>タイムゾーン</p> </td> 
  </tr> 
  <tr> 
   <td><code>X</code> </td> 
   <td><code>1360013296</code> </td> 
   <td> <p> UNIX タイムスタンプ</p> </td> 
  </tr> 
  <tr> 
   <td><code>x</code> </td> 
   <td><code>1360013296123</code></td> 
   <td> <p> UNIX ミリ秒タイムスタンプ</p> </td> 
  </tr> 
 </tbody> 
</table>
