---
product-area: programs
navigation-topic: create and manage programs
title: プログラムの作成
description: プログラムとは、プロジェクトの境界を越えた共通の戦略、目標、または目標を共有するプロジェクトの集まりを表します。 プログラムは、ポートフォリオ外には存在できません。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# プログラムの作成

プログラムとは、プロジェクトの境界を越えた共通の戦略、目標、または目標を共有するプロジェクトの集まりを表します。 プログラムは、ポートフォリオ外には存在できません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!UICONTROL 編集 ] によるPortfolioとプログラムへのアクセス </p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオに対する [!UICONTROL 管理 ] 権限</p> <p>プログラムを作成したら、そのプログラムに対する [!UICONTROL 管理 ] 権限がデフォルトで与えられます</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## プログラムの作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. 次のいずれかの操作を行います。

   * からプログラムを作成する [!UICONTROL プログラム] 領域：

      1. クリック **[!UICONTROL プログラム]** をクリックします。
      1. クリック **[!UICONTROL 新規プログラム]**.
      1. 表示されるボックスに、既存のPortfolioの名前を **[!UICONTROL 選択Portfolio]** フィールドに入力します。
      1. 新しいプログラムの名前を **[!UICONTROL 名前]** フィールドに入力します。
      1. 「**[!UICONTROL 保存]**」をクリックします。
   * からプログラムを作成する [!UICONTROL Portfolio] 領域：

      1. クリック **[!UICONTROL Portfolio]** 内 [!UICONTROL メインメニュー]」、「ポートフォリオ」の順にクリックします。
      1. 左側のパネルで、 **[!UICONTROL プログラム]**.
      1. 次をクリック： **[!UICONTROL 新規プログラム]** ドロップダウンメニューから、 **[!UICONTROL 新規プログラム]**.


1. プログラムの名前を **[!UICONTROL 名称未設定プログラム]** フィールドに入力します。

   名前は 255 文字までです。

1. （オプション）「 **[!UICONTROL プログラムマネージャ]** を設定し、更新する必要があります。

   >[!TIP]
   >
   >プログラムの作成者は、デフォルトでプログラムマネージャとして設定されます。

1. クリック **[!UICONTROL プログラムの詳細]** をクリックします。
1. 任意のフィールドをダブルクリックして、 **[!UICONTROL 概要]** 領域
1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>フィールド</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td> <p>プログラムの説明を指定します。</p> <p>説明は、プログラムのランディングページに表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL プログラムマネージャー ]</td> 
      <td> <p>プログラムマネージャーとして機能させるユーザーの名前を入力し、ドロップダウンリストに表示されたら、そのユーザーの名前をクリックします。 これは、[!UICONTROL プログラム所有者 ] と同じです。 </p> <p>ヒント：また、プログラムヘッダーでプログラムマネージャーを更新することもできます。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL グループ ] </td> 
      <td> <p>グループがプログラムを所有している場合、またはプログラムの完了を担当している場合は、1 つのグループの名前を追加します。 </p> <p>適切なグループを選択していることを確認するには、グループにマウスポインターを置いて [!UICONTROL information] アイコンをクリックします <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプションおよび条件付き） **[!UICONTROL カスタムフォームを追加]** ボックスを使用して、ポートフォリオのカスタムフォームを選択し、カスタムフィールドを更新します。

   >[!TIP]
   >
   >プログラムをプログラムに添付するには、プログラムのカスタムフォームが既に作成されている必要があります。

1. （オプション）任意のフィールドをダブルクリックして、カスタムフォームの情報を更新します。
1. クリック **[!UICONTROL プロジェクト]** 左のパネルで、 **[!UICONTROL プロジェクトを追加]** をクリックして、プログラムにプロジェクトを追加します。

   プログラムへのプロジェクトの追加については、 [プログラムにプロジェクトを追加する](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. クリック **[!UICONTROL 変更を保存]**.
1. （オプション） **[!UICONTROL その他のメニュー]** ![](assets/more-icon.png) プログラム名の横にあるをクリックし、 **[!UICONTROL プログラムの無効化]**.

   プログラムを非アクティブ化すると、ユーザーがプロジェクトに追加しようとすると、そのプログラムはプログラムのリストに表示されなくなります。 引き続き、 [!UICONTROL プログラム] 領域

## プログラムヘッダーの概要

ヘッダーには、プログラムに関する限定的な情報が表示されます。

プログラムのヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ヘッダー情報</td> 
   <td> <p><strong>メモ</strong> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ポートフォリオ名を示すパンくず</td> 
   <td>プログラムのヘッダーから、プログラムが属するポートフォリオにアクセスできます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プログラム名</td> 
   <td>ヘッダーでプログラム名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプの名前とアクティベーションステータス</td> 
   <td>プログラムを表示すると、「プログラム」という単語は緑色の輪郭で表示されます。 プログラムが [!UICONTROL アクティブ ] とマークされていない場合、「[!UICONTROL 非アクティブ ]」という単語が横に表示され、アウトラインは灰色で表示されます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プログラムのアクション領域 </td> 
   <td> <p>プログラムの詳細情報や編集オプションにアクセスするには、次のいずれかをクリックします。</p> 
    <ul> 
     <li>お気に入りのリストにプログラムを追加する星形のアイコン</li> 
     <li> <p>[!UICONTROL 詳細 ] メニュー <img src="assets/qs-more-menu.png"> 次のいずれかを実行するには： </p> 
      <ul> 
       <li>プログラムを編集</li> 
       <li>無効にします。 プログラムを非アクティブ化すると、プロジェクトレベルでプロジェクトに関連付けられなくなります。 </li> 
       <li> <p>削除します。 プログラムを削除しても、プログラム内のプロジェクトは削除されません。 プロジェクトとプログラムとの関連付けが削除されます。 </p> </li> 
       <li>他のユーザーと共有する</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完了率 ]</td> 
   <td> <p>ヘッダーのプログラムの [!UICONTROL 完了率 ] を編集することはできません。 この情報は、プログラムのプロジェクトから更新されます。 デフォルトでは、プログラムの完了率は、[!UICONTROL 現在 ] ステータスと [!UICONTROL 承認済み ] ステータスのプロジェクトの完了率の値の平均です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プログラムマネージャー ]</td> 
   <td> <p>ヘッダーでプログラムマネージャーを編集できます。 これは、[!UICONTROL プログラム所有者 ] と同じです。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 計画完了日 ]</td> 
   <td>ヘッダーでプログラムの完了率を編集することはできません。 プログラムの完了率は、ヘッダー内のプロジェクトの完了率の平均です。 ここで表されるプロジェクトは、ステータスが [!UICONTROL Current] および [!UICONTROL Approved] のプロジェクトです。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アクティブプロジェクト条件 ]</td> 
   <td>これは、[!UICONTROL Condition] が [!UICONTROL On Target]、[!UICONTROL At Risk]、[!UICONTROL In Trable] のいずれかに設定されている、プログラム内のプロジェクトの割合の計算です。 ここで表されるプロジェクトは、ステータスが [!UICONTROL Current] および [!UICONTROL Approved] のプロジェクトです。 </td> 
  </tr> 
 </tbody> 
</table>

## プログラムの移動

既存のプログラムをポートフォリオに追加できます。 2 つの異なるポートフォリオにプログラムが存在することはできないので、既存のプログラムを追加すると、ポートフォリオ間でプログラムが永続的に移動します。

詳しくは、 [ポートフォリオに既存のプログラムを追加する](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
