---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの編集
description: ダッシュボードの目的は、情報にすばやくアクセスできるようにすることです。 ダッシュボードに、レポート、カレンダーおよび外部ページを入力できます。
author: Nolan
feature: Reports and Dashboards
exl-id: de15ab45-4bcd-4638-b3d7-fc70a0866d2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# ダッシュボードの編集

ダッシュボードの目的は、情報にすばやくアクセスできるようにすることです。 Adobe Workfrontでは、次の項目をダッシュボードに入力できます。

* レポート

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* カレンダー

   カレンダーの作成について詳しくは、 [カレンダー](../../../reports-and-dashboards/reports/calendars/calendars.md).

* 外部ページ

   外部ページの作成について詳しくは、 [外部 Web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

これらの項目を作成してダッシュボードに追加した後は、ダッシュボードを編集して、そのダッシュボードに項目を追加したり、既存の項目を削除したり、ダッシュボード情報を編集したりできます。

ダッシュボードに変更を加えると、そのダッシュボードにアクセスできるすべてのユーザーに影響します。

ダッシュボードをユーザーと共有すると、すべてのレポート、カレンダーおよび外部ページも同じユーザーと共有されます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ダッシュボードを編集する前に、ダッシュボードを作成する必要があります。

ダッシュボードの作成について詳しくは、 [ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## ダッシュボードの編集

1. 編集するダッシュボードに移動します。
1. クリック **ダッシュボードのアクション**&#x200B;を選択し、「 **編集**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

   >[!TIP]
   >
   >ダッシュボードを削除する方法については、「 [ダッシュボードの削除](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/delete-dashboard.md).

1. 次のフィールドの編集を検討してください。

   * **名前**:ダッシュボードの名前を編集します。
   * **説明**:ダッシュボードの説明を指定します。

1. 内 **使用可能なレポートおよびカレンダー** セクションに、レポート、カレンダーまたは外部ページの名前を **名前またはタイプで検索…** フィールドを開き、レポートまたはカレンダーをレイアウトパネルから右にドラッグ&amp;ドロップします。

   >[!NOTE]
   >
   >項目を検索すると、最近作成された 2,000 個のレポートのいずれかが返されます。 Unicode 文字を含むレポート名は、検索結果に返されません。 ベストプラクティスとして、別のソースから名前をコピー&amp;ペーストするのではなく、名前を入力して、Workfrontでオブジェクトに名前を付ける際に Unicode 文字を含めないでください。

1. （オプション）目的のレイアウトに対応するラジオボタンをクリックして、ダッシュボードの新しいレイアウトを選択します。
1. （オプション）既存のレポートの名前にマウスを移動し、ごみ箱アイコンをクリックして、ダッシュボードから削除します。
1. （オプション）レポートの名前をクリックし、ドラッグして、レイアウトペインの目的の場所にドロップすることで、ダッシュボード上のレポートの順序を変更します。
1. （オプション）「 **外部ページを追加** をクリックして、ダッシュボードに外部ページを追加します。\
   または\
   ダッシュボードで既存の外部ページを見つけ、その上にマウスを移動して、 **編集** 外部ページを編集するアイコン。\
   ダッシュボードでの外部ページの追加や編集について詳しくは、 [外部 Web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. クリック **保存して閉じる**.
