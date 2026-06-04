---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: フィールドの文字数制限
description: Adobe Workfront の特定のフィールドでは、フィールドに入力できる文字の数を制限しています。 Workfront では、後で検索できるように、コンテンツのインデックスを作成します。 Workfront システムの高品質なパフォーマンスを確保するために、文字制限が適用されます。
author: Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
TQID: https://experienceleague.adobe.com/5oa9RRT-VOFngI2UJncfwlVYfHXilftl8kpetBBY7-k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 97%

---

# フィールドの文字数制限

Adobe Workfront の特定のフィールドでは、フィールドに入力できる文字の数を制限しています。 Workfront では、後で検索できるように、コンテンツのインデックスを作成します。 Workfront システムの高品質なパフォーマンスを確保するために、文字制限が適用されます。

制限に近づくと、カウンターが表示されます。 制限を超えると、超過した文字がハイライト表示され、テキストを投稿できなくなります。 許可された限度内に収まるまで、文字を削除します。

文字数の上限は、使用しているフィールドによって異なります。 以下に示す制限は、ラテン文字（英語など）を使用する言語に適用されます。 拡張文字や 2 バイト文字を含んだ言語の場合は、この制限値が小さくなる可能性があります。

Workfront 管理者またはグループ管理者は、フィールドの文字制限を変更できません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>フィールドタイプ</strong> </p> </th> 
   <th> <p><strong>文字数制限（</strong><strong>スペースを含む）</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>カスタムフォーム内の書式付きテキストフィールド</td> 
   <td>15,000</td> 
  </tr> 
  <tr> 
   <td> <p>ステータスの更新</p> </td> 
   <td> <p>15,000</p>
   <p> API を使用する場合は 4,000 文字</p> </td> 
  </tr> 
  <tr> 
   <td> <p>更新</p> </td> 
   <td> <p>15,000</p> 
   <p> API を使用する場合は 4,000 文字</p></td> 
  </tr> 
  <tr> 
   <td> <p>説明（ドキュメント、タスク、イシュー、ポートフォリオ、プログラムおよびプロジェクト）</p> </td> 
   <td> <p>4,000</p> </td> 
  </tr> 
  <tr> 
   <td>カスタムフォームの説明フィールド</td> 
   <td>4,000</td> 
  </tr> 
  <tr> 
   <td> <p>カスタムデータ段落または1行テキスト  </p> </td> 
   <td> <p>2,000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Report Builder の説明フィールド</p> </td> 
   <td> <p>512</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ドロップダウンメニューラベル</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
  <tr> 
   <td> <p>オブジェクト名</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
 </tbody> 
</table>
