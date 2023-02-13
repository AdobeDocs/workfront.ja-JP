---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Adobe Workfrontの校正ライセンスを持つユーザーの一覧
description: Adobe Workfrontのどのユーザーが現在「ユーザーは配達確認を生成できます」オプションを有効にしているかは、次のいずれかの方法で表示できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Adobe Workfrontの校正ライセンスを持つユーザーの一覧

Adobe Workfrontのどのユーザーが現在「ユーザーは配達確認を生成できます」オプションを有効にしているかは、次のいずれかの方法で表示できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>レガシープラン：選択またはプレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループの作成</p> </li> 
    </ul> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## ユーザーレポートの作成

ユーザーレポートを作成して、配達確認を生成できるユーザーを表示できます。

1. に移動します。 **レポート** 領域
1. 次をクリック： **新しいレポート** ドロップダウンメニューで、 **ユーザーレポート**.

1. の **フィルター** タブ、クリック **フィルタールールを追加**.

1. 使用可能フィールドで、を展開します。 **ユーザー**&#x200B;を選択し、「 **配達確認ライセンスを持っている**.

1. 選択 **次と等しい** > **True**.

   ![report_proflicens.png](assets/report-prooflicenses-350x135.png)

1. クリック **保存して閉じる**.

   このレポートには、Workfrontで、校正ライセンスが割り当てられているすべてのユーザーが表示されます。

## 人物ビューの更新

People ビューに新しい列を追加して、配達確認を生成できるユーザーを表示できます。

1. 次に移動： **人** 領域
1. 次をクリック： **人** タブをクリックします。
1. 内 **表示** ドロップダウンメニューで、次のいずれかの操作を行います。

   * この情報を既存のビューに追加するには、カスタマイズするビューを選択し、 **表示をカスタマイズ**.
   * この情報を新しいビューに追加するには、 **新しいビュー**.

1. クリック **列を追加**.
1. 使用可能フィールドで、を展開します。 **ユーザー**&#x200B;を選択し、「 **配達確認ライセンスを持っている**.

1. クリック **完了**&#x200B;を選択し、「 **ビューを保存** または **新しいビューとして保存**.

   ビューが表示されます **True** または **False** ユーザーに校正用ライセンスが割り当てられているかどうかに応じて異なります。
