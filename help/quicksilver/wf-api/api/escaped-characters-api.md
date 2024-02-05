---
content-type: api
navigation-topic: api-navigation-topic
title: API 応答のエスケープ文字
description: API 応答のエスケープ文字
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 100%

---

# API 応答のエスケープ文字

一部の API 応答の構文には、エスケープ文字の、`\`（バックスラッシュ）を含みます。エスケープ文字は、エスケープ文字の直後の文字または文字列が特別な値を持つことを示します。例えば、`tab`「t」の文字ではなく、`t`「t」の文字として解釈される`\t`読み取り装置に伝えます。バックスラッシュの後に 1 つ以上の文字を含む文字列は、エスケープシーケンスと呼ばれます。

16 進エスケープシーケンスでは、有効な 16 進数を使用する必要があります。次の表に、Adobe Workfront API 応答でエンコードされるエスケープシーケンスを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>エスケープシーケンス</strong> </th> 
   <th><strong>Unicode 文字</strong> </th> 
   <th><strong>表示</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>ここで、<em>x</em>は、0 ～ 7 の数値を表す 16 進数コードです</p> </td> 
   <td>0-7</td> 
   <td>コードポイント 0～7 で表される Unicode 文字</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>バックスペース</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>タブ</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>改行</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>「垂直」タブ</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>フォームフィード</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>キャリッジリターン</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>ここで、xx は 14～31 の数値の 16 進数コードです</em> </p> </td> 
   <td>14 - 31</td> 
   <td>コードポイント 14～31 で表される Unicode 文字</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/（フォワードスラッシュ）</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt;（未満）</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\（バックスラッシュ）</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>ここで、<em>xxxx</em> は、127 を超える任意の数の 16 進数コードです</p> </td> 
   <td>128+</td> 
   <td>127 を超える任意のコードポイントに対する Unicode 文字</td> 
  </tr> 
 </tbody> 
</table>
