---
product-area: resource-management
navigation-topic: resource-planning
title: リンクを使用して「リソースプランナー」ユーザービューを共有
description: Adobe Workfrontでは、ダッシュボードに外部ページとして埋め込むことのできるリソースプランナーのユーザービューの一意の URL を生成するか、別のブラウザータブで別々に開くことができます。 これは、リソースプランナーの情報を、リソース領域に直接アクセスできない可能性のあるユーザーと共有する場合に役立ちます。
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# リンクを使用して「リソースプランナー」ユーザービューを共有

Adobe Workfrontでは、ダッシュボードに外部ページとして埋め込むことのできるリソースプランナーのユーザービューの一意の URL を生成するか、別のブラウザータブで別々に開くことができます。 これは、リソースプランナーの情報を、リソース領域に直接アクセスできない可能性のあるユーザーと共有する場合に役立ちます。

![](assets/rp-user-view-with-link-highlight-350x49.png)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理、プロジェクト、およびユーザーへの表示または高いアクセス権</p> <p>財務データへのアクセスを表示してコスト情報を表示 </p> <p><b>注意</b> まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リソースプランナーに表示するプロジェクトに対する権限を表示または上限に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。


リソース・プランナのユーザー・ビューの一意の URL を生成する際は、次の点を考慮してください。

* 一意の URL は、ユーザービューに対してのみ取得できます。 URL を生成するオプションがプロジェクトビューまたはロールビューに存在しません。
* この URL は、Work や Review のライセンスを持つユーザーなど、他のユーザーと共有できます。\
   他のユーザーと共有する URL からリソースプランナーの情報を表示するには、そのユーザーが他のユーザーを表示するアクセス権を持っている必要があります。
* URL を他のユーザーと共有する際に、次の情報が保存されます。

   * 期間のタイプ（週、月、四半期）。
   * 適用するフィルター。
   * ディスプレイのタイプ（時間または工数）。

リソース・プランナのユーザー・ビューで一意の URL を取得し、他のユーザーと共有する手順は、次のとおりです。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **リソース**.
1. で、「 」を選択します。 **ユーザー別に表示**.
1. （オプション）リソース・プランナに情報を表示する期間を選択します。 次の中から選択します。

   * 週
   * 月
   * 四半期

1. （オプション）情報を表示するかどうかを選択します。 **FTE** または **時間**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. （オプション）リソースプランナーにフィルタを適用します。\
   フィルターの適用について詳しくは、 [リソースプランナーの情報のフィルタリング](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. 次をクリック： **ハイパーリンク** アイコン\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. クリック **URL をコピー**.\
   これにより、ユーザービューのリソースプランナーの一意の URL がクリップボードにコピーされます。

1. （オプション）次のいずれかの操作をおこないます。  

   * URL を別のアプリケーションに貼り付けて、別のユーザーに送信します。\
      ユーザービューでリソースプランナーを表示するには、Workfrontにログインする必要があります。
   * 新しいブラウザ・タブまたはウィンドウを開き、コピーしたリンクを貼り付け、キーボードの「Enter」をクリックして、リソース・プランナを新しいタブまたはウィンドウで開きます。
   * 次の操作を実行します。

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. に移動します。 **レポート**>**ダッシュボード**>**新しいダッシュボード**>**外部ページを追加します。**

      1. クリップボードにコピーしたリンクをに貼り付けます。 **URL** フィールドに入力します。
      1. クリック **保存**&#x200B;を、 **保存して閉じる**.\
         これにより、URL がダッシュボードに埋め込まれ、リソースプランナーのユーザービューが別のダッシュボードに表示されます。

1. （オプション）URL をダッシュボードに埋め込む場合は、URL をレイアウトテンプレートに追加するか、リソース管理領域にアクセスできない他のユーザーと URL を共有することを検討します。\
   レイアウトテンプレートへのダッシュボードの追加について詳しくは、 [レイアウトテンプレートの作成と管理](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   ダッシュボードの共有について詳しくは、 [ダッシュボードの共有](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   共有 URL を表示すると、ユーザーは、最初にリソース・プランナに適用した設定で情報を確認できます。 共有 URL を表示するには、Workfrontにログインする必要があります。\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
