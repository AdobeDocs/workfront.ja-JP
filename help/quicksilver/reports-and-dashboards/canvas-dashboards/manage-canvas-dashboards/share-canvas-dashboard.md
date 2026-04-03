---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: キャンバスダッシュボードの共有
description: Canvas ダッシュボードを他のAdobe Workfront ユーザーと共有して、他のユーザーが閲覧または編集できるようにすることができます。
author: Courtney
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 13%

---

# キャンバスダッシュボードの共有

>[!IMPORTANT]
>
>Canvas ダッシュボード機能は現在、ベータ版ステージに参加しているユーザーのみが利用できます。 機能の一部が完了していないか、この段階で意図したとおりに動作しない可能性があります。 ご利用のエクスペリエンスに関するフィードバックは、Canvas ダッシュボードのベータ版の概要の記事の「[&#x200B; フィードバックを提供](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)」セクションの指示に従って送信してください。<br>
>バグや技術的な問題についてフィードバックがある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[&#x200B; カスタマーサポートにお問い合わせください](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>を参照してください
>このベータ版は、次のクラウドプロバイダーでは利用できないことに注意してください。
>
>* Amazon Web Services用に独自のキーを持ち込む
>* Azure
>* Google Cloud Platform

Canvas ダッシュボードを他のAdobe Workfront ユーザーと共有して、他のユーザーが閲覧または編集できるようにすることができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>標準 </p> 
<p>プラン</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>レポート、ダッシュボードおよびカレンダーの表示アクセス権</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>ダッシュボードでダッシュボードを共有するための権限を表示します</p>
   <p>ダッシュボードの権限を管理して、ダッシュボードの権限を割り当てます</p>
  </td> 
  </tr>
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## ダッシュボードの共有に関する考慮事項

* ダッシュボードは、ユーザー、チーム、グループ、担当業務、または会社のリソースに共有できます。

* デフォルトでは、ダッシュボードの作成者には、ダッシュボードの管理権限があります。

* 管理権限を持つシステム管理者とユーザーは、ダッシュボードへの表示または管理アクセス権を付与できます。

* ダッシュボードへの表示権限を持つユーザーは、ダッシュボードへの表示アクセス権を付与できます。

* ダッシュボードを共有する場合、共有されているリソースは、ダッシュボードに表示されるレポートに対する権限を継承します。

* ダッシュボードがレイアウトテンプレートを通じて配布されると、ダッシュボード（およびそのレポート）の自動表示権限が、レイアウトテンプレートに割り当てられたすべてのリソースに付与されます。


## キャンバスダッシュボードの共有


{{step1-to-dashboards}}

1. 左側のパネルで、「**キャンバスダッシュボード**」をクリックします。

1. **Canvas ダッシュボード** ページで、共有するダッシュボードを選択します。

1. ページの右上隅にある「**共有**」ボタンをクリックします。 **ダッシュボード共有** ダイアログボックスが表示されます。

   ![共有ボタン &#x200B;](assets/share-button.png)

1. 「**アクセスを許可する**」フィールドで、キャンバスダッシュボードを共有する特定のユーザー、チーム、役割、グループ、または会社の名前を入力し始め、ドロップダウンリストに表示されたら選択します。

1. （オプション）ダッシュボードへのリソースのアクセス権を編集するには、名前の横にある&#x200B;**表示**&#x200B;をクリックし、表示されるドロップダウンリストで&#x200B;**管理**&#x200B;を選択します。

   >[!NOTE]
   >
   > ユーザーがアクセスレベルを通じて割り当てられたダッシュボードに対する編集権限を持っていない場合、ダッシュボードに管理権限を割り当てることはできません。

1. ダッシュボードを共有するリソースごとに、手順5～6を繰り返します。

1. 「**共有**」ボタンをクリックします。 受信者には、ダッシュボードが共有されたことを知らせるメール通知が届きます。これで、**ダッシュボード** > **キャンバスダッシュボード** > **共有ダッシュボード**&#x200B;にアクセスできます。

   >[!NOTE]
   >
   > 個々のユーザーの好みやメール通知のシステム除外が適用される場合があります。<br>
   > 通知は、ユーザーと直接共有した場合にのみ送信されます。 グループ、役割、会社、およびチームへの共有では、メール通知は生成されません。<br>
   > レイアウトテンプレートから継承された権限では、ダッシュボードへのアクセスに関するメール通知は生成されません。
