---
product-area: Canvas Dashboards
navigation-topic: report-types
title: ダッシュボードのフィルタリング
description: キャンバスダッシュボードの作成後に、フィルターを適用できます。
author: Courtney and Jenny
feature: Reports and Dashboards
hidefromtoc: true
hide: true
source-git-commit: d22cd176947387ce5f24e4fc91444b7aca698f5d
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 19%

---

# ダッシュボードのフィルタリング

>[!IMPORTANT]
>
>キャンバスダッシュボード機能は現在、ベータ版のステージに参加しているユーザーのみが利用できます。 詳しくは、[ キャンバスダッシュボードのベータ版情報 ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md) を参照してください。

プロンプトを含むダッシュボードにフィルターを適用できます__________

+++ 展開すると、アクセス要件が表示されます。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>任意 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>現在：プラン </p> 
<p>新規：標準</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>レポート、ダッシュボードおよびカレンダーへのアクセスを編集する</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>ダッシュボードの権限管理</p>
  </td> 
  </tr> 
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## 前提条件

ダッシュボードをフィルタリングするには、ダッシュボードを作成する必要があります。

詳しくは、[ キャンバスダッシュボードの作成 ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md) を参照してください。

## ダッシュボードのフィルタリング

{{step1-to-dashboards}}

1. 左側のパネルで、「**キャンバスダッシュボード**」をクリックします。

1. **キャンバスダッシュボード** ページで、フィルターを適用するダッシュボードを選択します。

1. ダッシュボードの詳細ページの左上隅にある「**フィルター**」をクリックします。 フィルターのサイドパネルが開きます。

1. **フィルターを編集** を選択します。 **ダッシュボードフィルター** ダイアログボックスが開きます。

1. （オプション）ルールを追加するには、次の手順に従います。

   1. ルールボックスの右側にある **編集** アイコンを選択します。

      ![ 編集アイコン ](assets/edit-icon.png)

   1. 「**条件を追加**」をクリックして、フィルターに使用するフィールドと、フィールドが満たす必要がある条件の種類を定義する修飾子を指定します。

   1. （任意）「**フィルターグループを追加**」をクリックして、別のフィルター条件セットを追加します。 セット間のデフォルトの演算子は AND です。演算子をクリックして OR に変更します。

1. プロンプトを追加するには、次の手順に従います。

   1. **プロンプトの追加** を選択します。 新しいフィールドが画面の右側に表示されます。

   1. **ラベルをカスタマイズ** フィールドにラベルを入力します。

   1. **フィールドを選択** をクリックしてから、________ードするフィールドを指定します。

1. カスタムプロンプトを追加するには、次の手順に従います。

   1. **カスタムプロンプトを追加** を選択します。 新しいフィールドが画面の右側に表示されます。

   1. （オプション）「**ラベルをカスタマイズ**」フィールドに新しいラベルを入力します。 デフォルトでは、ラベル *新規カスタムプロンプト* が割り当てられます。

   1. **新しいオプションを追加** をクリックします。

   1. **オプション値** フィールドに_____を入力します。

   1. 「**条件を追加**」をクリックして、フィルターに使用するフィールドと、フィールドが満たす必要がある条件の種類を定義する修飾子を指定します。

   1. （任意）「**フィルターグループを追加**」をクリックして、別のフィルター条件セットを追加します。 セット間のデフォルトの演算子は AND です。演算子をクリックして OR に変更します。

1. 「**保存**」をクリックして、フィルターをダッシュボードに適用します。