---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: キックスタートのシナリオ：会社、グループ、役割およびユーザーのキックスタートの準備
description: Adobe Workfront の実装を開始する際に、データを手動で入力する代わりに、顧客リスト、内部部門、担当業務、ユーザー情報を読み込むことができます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 52%

---

# キックスタートのシナリオ：会社、グループ、役割およびユーザーのキックスタートの準備

Adobe Workfront の実装を開始する際に、データを手動で入力する代わりに、顧客リスト、内部部門、担当業務、ユーザー情報を読み込むことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 読み込みできるもの

インポートする会社、グループ、役割を次の表に示します。

| 会社 | グループ | 役割 |
|---|---|---|
| Acme, Co <p>Workfront, Inc. <p>_あなたの会社_ <p>XYZ, Inc. | 財務 <p>IT <p>マーケティング <p>販売 | ビジネスアナリスト <p>コントローラークリエイティブ <p>Designer <p>リソース管理者 <p>スクラムマスター <p>テクニカルライター <p>Web 開発者 |

{style="table-layout:auto"}

役割名は一意である必要があります。 既存の担当業務はインポートできません。

次の表に、読み込むユーザーと、それぞれの複数のユーザー属性を示します。

### ユーザー 1

| 属性 | 値 |
|---|---|
| **名前（名）** | Chris |
| **名前（姓）** | Manning |
| **ユーザー名またはメール** | mailto:cmanning@foo.com |
| **パスワード** | updateMe |
| **アクセス** | チームメンバー |
| **会社** | &lt;*あなたの会社*> |
| **ホーム グループ** | マーケティング |
| **担当業務** | ビジネスアナリスト |

{style="table-layout:auto"}

### ユーザー 2

| 属性 | 値 |
|---|---|
| **名** | Jennifer |
| **姓** | Campbell |
| **ユーザー名／E メール** | jcampbell@foo.com |
| **パスワード** | updateMe |
| **アクセス** | プロジェクトマネージャー |
| **会社** | &lt;*あなたの会社*> |
| **ホーム グループ** | マーケティング |
| **担当業務** | プロジェクトマネージャー |

{style="table-layout:auto"}

### ユーザー 3

| 属性 | 値 |
|---|---|
| **名** | Jill |
| **姓** | Sullivan |
| **ユーザー名／E メール** | jsullivan@foo.com |
| **パスワード** | updateMe |
| **アクセス** | ヘルプデスク |
| **会社** | &lt;*あなたの会社*> |
| **ホーム グループ** | 販売 |
| **担当業務** | 販売担当者 |

{style="table-layout:auto"}

### ユーザー 4

| 属性 | 値 |
|---|---|
| **名** | Marc |
| **姓** | Lewis |
| **ユーザー名／E メール** | mlewis@foo.com |
| **パスワード** | updateMe |
| **アクセス** | ポートフォリオマネージャー |
| **会社** | &lt;*あなたの会社*> |
| **ホームグループ** | 財務 |
| **担当業務** | コントローラー |

{style="table-layout:auto"}

### ユーザー 5

| 属性 | 値 |
|---|---|
| **名前（名）** | Pam |
| **名前（姓）** | Reynolds |
| **ユーザー名またはメール** | preynolds@foo.com |
| **パスワード** | updateMe |
| **アクセス** | プロジェクトマネージャー |
| **会社** | *会社>* |
| **ホームグループ** | マーケティング |
| **担当業務** | IT |

{style="table-layout:auto"}

### ユーザー 6

| 属性 | 値 |
|---|---|
| **名前（名）** | Ray |
| **名前（姓）** | Andrews |
| **ユーザー名またはメール** | randrews@foo.com |
| **パスワード** | updateMe |
| **アクセス** | 管理者 |
| **会社** | *会社>* |
| **ホームグループ** | リソース管理者 |
| **担当業務** | なし |

{style="table-layout:auto"}

## キックスタートテンプレートのダウンロード

{{step-1-to-setup}}

1. **システム**／**キックスタート**／**データを読み込み**&#x200B;をクリックします。

1. **その他のオプション**&#x200B;をクリックして、読み込みオプションの完全なリストを表示します。
1. 読み込むアクセスレベル、会社、グループ、担当業務、ユーザーの各オブジェクトを選択します。
1. 「**ダウンロード**」をクリックします。

## 会社情報を入力

1. ダウンロードした **Workfront.xlsx** ファイルを開きます。

   >[!TIP]
   >
   >非常に幅の広いデータシートを扱う場合は、スプレッドシートエディターのウィンドウ枠の固定（または同等のツール）を使用して、スプレッドシートを簡単に操作できるようにすることが可能です。

1. **CMPY Company** シートに移動します。

   会社が既にシステム内にない場合は、空にする必要があります。

   ![ 会社シート ](assets/cmpysheet-350x16.png)![ 会社 ID](assets/companyid--1--350x78.png)

1. **isNew** 列に **TRUE** と入力します。

   追加される会社ごとに、このアクションを繰り返します。（この例では、4 つの会社が追加されているので、3～6 行目でこのアクションを実行します）。

   ![ 会社が新しくなりました ](assets/cmpyisnew-350x86.png)

1. 一意の **ID** を入力します。

   各行に ID を入力する必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![ 会社が新しくなりました ](assets/cmpyisnew-350x86.png)

1. **setName** 列に各顧客の名前を入力します。

   ![ 会社 ID](assets/companyid-350x78.png)

1. **グループ グループ** シートに移動します。

   Workfront で既にグループを作成している場合を除き、このシートには、Workfront のすべてのアカウントでプロビジョニングされたデフォルトグループのみが表示されます。

   ![ グループシート ](assets/groupsheet-350x15.png)![ 空のグループシート ](assets/emptygroupsheet-350x85.png)

1. **isNew** 列に **TRUE** と入力します。

   シナリオに従って 4 つのグループがインポートされるので、行 4 ～ 7 の **isNew** 列に **TRUE** と入力します。

1. 一意の **ID** を入力します。

   各行に ID を入力する必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![ グループ ID](assets/groupids-350x85.png)

1. **setName** 列に各部門の名前を入力します。

   ![ グループ名 ](assets/groupnames-350x85.png)

1. **役割** シートに移動します。

   アカウントで既に役割を作成または削除している場合を除き、このシートには、Workfront のすべてのアカウントでプロビジョニングされた 8 つの役割が表示されます。

   ![ グループ名 ](assets/groupnames-350x85.png)

1. **isNew** 列に **TRUE** と入力します。

   シナリオに従って 7 つの担当業務がインポートされるので、12～18 行目の **isNew** 列に **TRUE** と入力します。

   ![Role is new](assets/roleisnew-350x104.png)

1. 一意の **ID** を入力します。

   各行に ID を入力する必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![Role is new](assets/roleisnew--1--350x104.png)

1. **setName** 列に各役割の名前を入力します。

   ![Role is new](assets/roleisnew-350x104.png)

1. 必要に応じて、追加の詳細を入力します。

   必要に応じて、作成する役割の請求率、コスト率、説明を含めます。

1. **ユーザーユーザー** シートに移動します。

   アカウントで既にユーザーを作成している場合を除き、このシートには、Workfront のすべてのアカウントでプロビジョニングされた管理者ユーザーのみが表示されます。

   ![ ユーザーシート ](assets/usersheet-350x16.png)![ 空のユーザーシート ](assets/emptyusersheet-350x52.png)

1. **isNew** 列に **TRUE** と入力します。

   シナリオに従って 6 人のユーザーがインポートされるので、行 4 ～ 9 の **isNew** 列に **TRUE** と入力します。

   ![ 新規ユーザー ](assets/userisnew-350x52.png)

1. 一意の **ID** を入力します。

   各行に ID を入力する必要があります。 1 で始まる整数は、新しいレコードを作成する際に適切に機能します。

   ![ 新規ユーザー ](assets/userisnew-350x52.png)

1. **setFirstName** 列と **setLastName** 列に各ユーザーの名前を入力します。

   ![ ユーザー名 ](assets/usernames-350x52.png)

1. **setEmail**、**setPassword**、および **setUsername** 列に値を入力して、詳細な値を設定します。

   ![ ユーザー資格情報 ](assets/usercredentials-350x52.png)

1. アクセスレベルの値を指定します。

   例えば、Chris Manning はチームメンバーです。 チーム メンバ アクセス レベルの **ACSLVL アクセス レベル** シートで ID を検索します。 ID をコピーし、「**USER ユーザー**」シートでそのユーザーの行の **setAccessLevelID** 列に貼り付けます。

   ユーザーおよびアクセスレベルごとに、この手順を繰り返します。

   ![ アクセス レベル ID をコピー ](assets/copyalid-350x171.png)![ アクセス レベル ID を貼り付け ](assets/pastealid-350x59.png)

1. ユーザーのホームグループの詳細を入力します。

   シナリオによると、Chris Manning はマーケティンググループに所属しています。「**GROUP Group**」シートでマーケティンググループの ID を探してコピーし、「**USER User**」シートでユーザー行の「**setHomeGroupID**」列に貼り付けます。&#x200B;ユーザーとグループの割り当てごとに、この手順を繰り返します。

   ![ グループ ID をコピー ](assets/copygroupid-1-350x133.png)![ グループ ID を貼り付け ](assets/pastegroupid-350x59.png)

1. ユーザーの会社の詳細を入力します。

   このシナリオのすべてのユーザーは、同じ会社に属しています。 **CMPY 会社** シートで **Your Own Company** 会社の ID を探し、その ID をコピーして、「**USER ユーザー**」タブで **setCompanyID** 列の各行にこの値を貼り付け&#x200B;す。

   ユーザーとグループの割り当てごとに、この手順を繰り返します。

   ![ 会社 ID](assets/companyid--1--350x78.png)![ 会社 ID を貼り付け ](assets/pastecompanyid-350x84.png)

1. ユーザーの担当業務の詳細を入力します。

   シナリオによると、Chris Manning にはビジネスアナリストの役割があります。**ROLE Role** シートで Business Analyst ロールの ID を探してコピーし、「**USER User** シートでユーザーの行の **setRoleID** 列に貼り付けます。&#x200B;ユーザーとグループの割り当てごとに、この手順を繰り返します。

   ![ 役割 ID をコピー ](assets/copyroleid-350x149.png)![ 役割 ID を貼り付け ](assets/pasteroleid-350x95.png)

1. 必要に応じて、その他のユーザーの詳細を入力し、ファイルを保存します。
1. Excel ファイルを読み込みます。

   [キックスタートテンプレートを使用した Adobe Workfront へのデータの読み込み](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)で示されている手順に従います。

>[!NOTE]
>
>Workfrontに読み込まれたユーザーは、非アクティブ化され、承認待ちのステータスで作成されます。
> 
>組織がAdobe Admin Consoleに移行されており、ユーザーのステータスが数分以内に非アクティブおよび承認保留中から変わらない場合、ユーザーのバッチをAdobe Admin Consoleに直接追加できます。
>
>手順については、アドビドキュメントの[複数ユーザーの管理 | CSV の一括アップロード](https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html)を参照してください。
