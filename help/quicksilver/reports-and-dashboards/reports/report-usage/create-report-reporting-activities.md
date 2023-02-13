---
product-area: reporting
keywords: 変更，所有者，共有，レポート，共有，実行，ユーザー，アクセス，権限，入力，最終，閲覧，日付，レポート，アクティビティ
navigation-topic: report-usage
title: レポートアクティビティに関するレポートの作成
description: レポートに関するレポートを作成する際に、特定のレポート情報を識別できます。レポートが非アクティブなユーザーに割り当てられているか、非アクティブなユーザーのアクセス権でレポートが実行されるか、削除する予定のレポートにアクセスするかなどです。
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 2%

---

# レポートアクティビティに関するレポートの作成

レポートに関するレポートを作成する際に、特定のレポート情報を識別できます。レポートが非アクティブなユーザーに割り当てられているか、非アクティブなユーザーのアクセス権でレポートが実行されるか、削除する予定のレポートにアクセスするかなどです。

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

## 既存のレポートに関するレポートの作成 {#create-the-report-about-existing-reports}

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある
1. クリック **レポート**&#x200B;を、 **新しいレポート**.
1. 内 **新しいレポート** ドロップダウンメニューで、「 **レポート** ：既存のレポートに関するレポートを作成します。

1. 内 **列（表示）** 」タブで、レポートに追加する列を選択します。\
   次のフィールドの一部が役立つ場合があります。

   | フィールド | 説明 |
   |---|---|
   | **実行ユーザ：名前** | これは、 **このレポートを実行する際のアクセス権は次のとおりです。** フィールドに値を入力します。 このユーザーが非アクティブになっている場合、レポートの共有先となるユーザーに対してはレポートは表示されません。 |
   | **と共有** | これらはすべて、レポートの共有先のエンティティです。 |
   | **エントリ者** | これはレポートの所有者です。 |
   | **最終表示日** | これは、ユーザーがレポートを最後に閲覧した日時です。 |

   {style=&quot;table-layout:auto&quot;}

1. （オプション）レポートのリストを、非アクティブな特定のユーザーに限定するには：

   1. を選択します。 **フィルター** 「 」タブで、「 **フィルタールールを追加**.

   1. フィルターを追加 **実行ユーザ ID** > **次と等しい**.

   1. フィルターに追加する非アクティブなユーザーの名前を入力し、リストに表示されたら、名前をクリックします。
   1. レポートに含める非アクティブなユーザーをすべて選択するまで、手順 C を繰り返します。

1. （オプション）レポートのリストを予定レポートに制限するには：

   1. を選択します。 **フィルター** 「 」タブで、「 **フィルタールールを追加**.

   1. フィルターを追加 **予定レポート ID** > **空白でない**.

1. クリック **保存して閉じる**」をクリックし、レポートの名前を入力して、 **レポートを保存**.

   レポート情報が表示されます。

1. （オプション）このレポートを Excel にエクスポートし、コンピューターに保存します。\
   レポートのエクスポートについて詳しくは、 [データを書き出し](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## レポートに関する情報の更新

レポートを作成した後、必要に応じてレポートを更新できます。

1. 更新するレポートに移動します。
1. 実行するアクションに応じて、次のいずれかの操作をおこないます。

   * を更新します。 **このレポートを実行する際のアクセス権は次のとおりです。** アクティブなユーザーのフィールド：詳しくは、 [別のユーザーのアクセス権を持つレポートの実行と配信](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * レポートのコピーを作成します。詳しくは、 [レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * レポートの削除：詳しくは、 [レポートの正確なコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) 記事のセクション [レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * レポートの共有：詳しくは、 [Adobe Workfrontでのレポートの共有](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. （条件付き）元のレポートをコピーする場合は、 [既存のレポートに関するレポートの作成](#create-the-report-about-existing-reports) をクリックして、新しいコピーを元のレポートと同じエンティティと共有します。
