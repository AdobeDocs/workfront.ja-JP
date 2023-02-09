---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：列の幅を永続的に編集する'
description: 余白をドラッグ&ドロップして目的の幅に合わせて一時的に列の幅を変更できます。 詳細については、「列の幅と順序を変更する」を参照してください。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 表示：列の幅を永続的に編集する

余白をドラッグ&amp;ドロップして目的の幅に合わせて一時的に列の幅を変更できます。 詳しくは、 [列の幅と順序を変更する](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

ビューの任意の列の幅は、ビューの編集時に列のテキストモードを使用して永久的に変更できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 列の幅を永続的に編集する

>[!IMPORTANT]
>
>この記事の「列の幅と順序を一時的に変更する」の説明に従って、列の幅を手動で変更する場合 [列の幅と順序を変更する](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 列の幅を恒久的に変更した後は、手動によるサイズ変更に応じて列の幅が保持され、次の手順に従って更新された列の幅が上書きされます。 キャッシュをクリアした後、または別のブラウザーからログインした後、次の手順で定義した幅に従って列を表示できます。

1. オブジェクトのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、 **新しいビュー**.

1. クリック **列を追加** をクリックして新しい列を追加します。

   または

   既存の列の列見出しをクリックします。

1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 次のコードを列のテキストモードに追加します。

   ```
   width=200
   usewidths=true
   ```

   の **幅** 行には、列を表示するビューの幅を表す任意の数値（ピクセル単位）を指定します。

1. クリック **保存**&#x200B;を、 **ビューを保存**.
