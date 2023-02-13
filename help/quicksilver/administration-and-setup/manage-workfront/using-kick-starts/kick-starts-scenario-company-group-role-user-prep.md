---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: '''キック開始シナリオ：会社、グループ、役割、ユーザーのキックスタートの準備`'
description: データを手動で入力する代わりに、Adobe Workfrontの実装を開始する際に、顧客リスト、内部部門、役割、ユーザー情報をインポートできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# キック開始シナリオ：会社、グループ、役割、およびユーザーのキックスタートの準備

データを手動で入力する代わりに、Adobe Workfrontの実装を開始する際に、顧客リスト、内部部門、役割、ユーザー情報をインポートできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 読み込み可能な内容

次の表に、インポートする会社、グループ、ロールを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>会社</strong> </th> 
   <th><strong>グループ</strong> </th> 
   <th><strong>役割</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront</p> <p><em>会社</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">財務</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">マーケティング </p> <p valign="top" rowspan="7">販売</p> </td> 
   <td valign="top"> <p valign="top">ビジネスアナリスト</p> <p valign="top">コントローラークリエイティブ</p> <p valign="top">設計者</p> <p valign="top">リソース管理者</p> <p valign="top">スクラムマスター</p> <p valign="top">テクニカルライター</p> <p valign="top">Web 開発者</p> </td> 
  </tr> 
 </tbody> 
</table>

ロール名は一意である必要があります。既存のジョブロールはインポートできません。

次の表に、読み込むユーザーと、それぞれの複数のユーザー属性を示します。

### ユーザー 1

| **名** | クリス |
|---|---|
| **姓** | マニング |
| **ユーザー名/電子メール** | mailto:cmanning@foo.com |
| **パスワード** | updateMe |
| **アクセス** | チーム メンバー |
| **会社** | &lt;*会社 >* |
| **ホーム グループ** | マーケティング |
| **担当業務** | ビジネスアナリスト |

{style=&quot;table-layout:auto&quot;}

### ユーザー 2

| **名** | ジェニファー |
|---|---|
| **姓** | キャンベル |
| **ユーザー名/電子メール** | jcampbell@foo.com |
| **パスワード** | updateMe |
| **アクセス** | プロジェクト マネージャ |
| **会社** | &lt;*会社 >* |
| **ホーム グループ** | マーケティング |
| **担当業務** | プロジェクト マネージャ |

{style=&quot;table-layout:auto&quot;}

### ユーザー 3

| **名** | ジル |
|---|---|
| **姓** | サリバン |
| **ユーザー名/電子メール** | jsullivan@foo.com |
| **パスワード** | updateMe |
| **アクセス** | ヘルプ デスク |
| **会社** | &lt;*会社 >* |
| **ホーム グループ** | 販売 |
| **担当業務** | 営業担当 |

{style=&quot;table-layout:auto&quot;}

### ユーザー 4

| **名** | マルク |
|---|---|
| **姓** | ルイス |
| **ユーザー名/電子メール** | mlewis@foo.com |
| **パスワード** | updateMe |
| **アクセス** | ポートフォリオマネージャー |
| **会社** | &lt;*会社 >* |
| **ホーム グループ** | 財務 |
| **担当業務** | コントローラ |

{style=&quot;table-layout:auto&quot;}

### ユーザー 5

| **名** | パム |
|---|---|
| **姓** | レイノルズ |
| **ユーザー名/電子メール** | preynolds@foo.com |
| **パスワード** | updateMe |
| **アクセス** | プロジェクト マネージャ |
| **会社** | *会社 >* |
| **ホーム グループ** | マーケティング |
| **担当業務** | IT |

{style=&quot;table-layout:auto&quot;}

### ユーザー 6

| **名** | レイ |
|---|---|
| **姓** | Andrews |
| **ユーザー名/電子メール** | randrews@foo.com |
| **パスワード** | updateMe |
| **アクセス** | 管理者 |
| **会社** | *会社 >* |
| **ホーム グループ** | リソース管理者 |
| **担当業務** | なし |

{style=&quot;table-layout:auto&quot;}

## キックスタートテンプレートのダウンロード

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **キックスタート** > **データをインポートします。**

1. クリック **その他のオプション** 読み込みオプションの完全なリストを確認するには、を参照してください。
1. インポートするアクセスレベル、会社、グループ、ジョブの役割、ユーザーの各オブジェクトを選択します。

## 会社情報を入力

1. を開きます。 **Workfront.xlsx** ファイルをダウンロードしました。

   >[!TIP]
   >
   >非常に幅の広いデータシートを扱う場合は、スプレッドシートエディタの [ フリーズウィンドウ ]（または同等のツール）を使用して、スプレッドシートを簡単に操作できるようにすることができます。

1. 「CMPY Company」シートに移動します。

   会社が既にシステムに存在しない限り、空にする必要があります。 ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. TRUE を **isNew** 列。
1. 追加される会社ごとに、このアクションを繰り返します。 （この例では、4 つの会社が追加されているので、3 ～ 6 行目でこのアクションを実行します。）

   ![](assets/cmpyisnew-350x86.png)

1. 一意の ID を指定します。

   これは、ID 列の各行に対しておこなう必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![](assets/cmpyisnew-350x86.png)

1. 名前を設定します。

   各顧客の名前を **setName** 列。

   ![](assets/companyid-350x78.png)

1. 「グループ」シートに移動します。

   Workfrontで既にグループを作成している場合を除き、このシートにはWorkfrontのすべてのアカウントでプロビジョニングされたデフォルトグループのみが表示されます。

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. を **isNew** 列。シナリオに従って、4 つのグループがインポートされるので、「isNew」列に TRUE を 4 ～ 7 行に指定します。
1. 一意の ID を指定します。

   これは、ID 列の各行に対しておこなう必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![](assets/groupids-350x85.png)

1. 名前を設定します。

   内の各部門の名前を指定します **setName** 列。

   ![](assets/groupnames-350x85.png)

   役割情報を指定します。 「役割」シートに移動します。

1. アカウントで既にロールを作成または削除している場合を除き、このシートにはWorkfrontのすべてのアカウントでプロビジョニングされた 8 つのロールが表示されます。

   ![](assets/groupnames-350x85.png)

1. True 文を設定します。

   7 つのジョブロールがインポート中で、&#39;isNew&#39;列の行 12 ～ 18 に TRUE を入力します。

   ![](assets/roleisnew-350x104.png)

1. 一意の ID を指定します。

   これは、ID 列の各行に対しておこなう必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. 各ロールの名前を setName 列に入力して指定します。

   ![](assets/roleisnew-350x104.png)

1. 必要に応じて、追加の詳細を入力します。

   必要に応じて、作成する役割の請求率、コスト率、説明を含めます。

1. 「ユーザー」シートに移動して、ユーザー情報を入力します。

   アカウントで既にユーザーを作成している場合を除き、このシートにはWorkfrontのすべてのアカウントでプロビジョニングされた管理者ユーザーのみが表示されます。

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. 6 人のユーザーがインポートされるので、「isNew」列の行 4 ～ 9 に TRUE を指定して True 値を設定します。

   ![](assets/userisnew-350x52.png)

1. ID 列の各行に一意の ID を指定して、一意の ID を設定します。 通常、1 で始まる整数は、新しいレコードに対して適切に機能します。

   ![](assets/userisnew-350x52.png)

1. 各ユーザーの名前を「setFirstName」列と「setLastName」列に入力します。

   ![](assets/usernames-350x52.png)

1. 「setEmail」、「setPassword」、「setUsername」の各列に値を指定して、詳細値を設定します。

   ![](assets/usercredentials-350x52.png)

1. アクセスレベルの値を指定します。

   たとえば、チームメンバーの Chris Manning は、「ACSLVL アクセスレベル」シートでチームメンバーアクセスレベルの ID を検索します。 ID をクリップボードにコピーし、「ユーザーユーザー」シートで、に貼り付けます。 **setAccessLevelID** 列をクリスの行に追加します。

   ユーザーおよびアクセスレベルごとに、この手順を繰り返します。

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. ホームグループの詳細を指定します。

   シナリオによると、Chris Manning はマーケティンググループに属しています。 グループグループシートで、マーケティンググループの ID を探し、クリップボードにコピーして、「ユーザー」シートの **setHomeGroupID**&#x200B;列をクリスの行に追加します。&#x200B;ユーザーとグループの割り当てごとに、この手順を繰り返します。

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. 会社の詳細を指定します。

   このシナリオのすべてのユーザーは、同じ会社に属しています。 「CMPY Company」シートで、「Your Own Company」の ID を探し、その ID をクリップボードにコピーし、「USER User」タブで、「setCompanyID」列の各行にこの値を貼り付けま&#x200B;す。

   ユーザーとグループの割り当てごとに、この手順を繰り返します。

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. ジョブロールの詳細を指定します。

   シナリオによると、Chris Manning はビジネスアナリストの役割を持ちます。 「役割」シートで、Business Analyst の役割の ID を探し、クリップボードにコピーし、「ユーザー」シートで、「Chris」行の「setRoleID」列に貼り付けます。&#x200B;ユーザーとグループの割り当てごとに、この手順を繰り返します。

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. 必要に応じて、その他のユーザーの詳細を入力し、ファイルを保存します。
1. Excel ファイルをインポートします。

   次に示す指示に従います。 **キックスタートファイルの読み込み** 」の節を参照してください。
