---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: ユーザーのプルーフアクセスの設定
description: Adobe Workfront 管理者または Workfront Proof 管理者は、Workfront と Workfront Proof でプルーフを作成および表示するためのユーザーのアクセス権を設定できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '1244'
ht-degree: 100%

---

# ユーザーのプルーフアクセスの設定

Adobe Workfront 管理者または Workfront Proof 管理者は、Workfront と Workfront Proof でプルーフを作成および表示するためのユーザーのアクセス権を設定できます。

基本プルーフと統合プルーフで利用可能なプルーフ機能について詳しくは、[Workfront でのプルーフ機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront 管理者または Workfront Proof 管理者である必要があります。Workfront 管理者について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ユーザーのプルーフ機能を有効または無効にする（従来プランのみ） {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

従来の Select または Premium の Workfront プランを使用している場合は、Workfront 管理者として、ユーザーのプルーフ機能を有効または無効にできます。

ユーザーのプルーフ機能を有効にすると、Workfront でユーザーのプルーフを自動的に生成するオプションが有効になります。

ユーザーをプルーフユーザーとして有効にできますが、Workfront のメインメニューから Workfront Proof インターフェイスに直接移動するには、管理者権限が必要です。Workfront システムのすべてのプルーフユーザーに対してこのオプションを有効にする方法について詳しくは、[Workfront のメインメニューから Workfront Proof へのアクセスをすべてのユーザーに設定](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users)を参照してください。

1. **メインメニュー**&#x200B;で、「**ユーザー**」を選択します。

1. ユーザーを選択し、**編集**&#x200B;アイコンをクリックします。
1. 「**アクセス**」セクションで、「**プルーフユーザー**」を選択または選択解除します。

## ユーザーのプルーフ権限プロファイルを設定

選択した権限プロファイルは、組織内に存在する各プルーフユーザーに付与されます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**ユーザー**![](assets/users-icon-in-main-menu.png)をクリックします。
1. 1 人または複数のユーザーを選択し、「**編集**」をクリックします。

1. 「**アクセス**」セクションで、**プルーフ権限プロファイル**&#x200B;ドロップダウンメニューで次のいずれかの Workfront Proof 権限オプションをクリックします。

   >[!NOTE]
   >
   >従来の Workfront プランの場合は、前述の[ユーザーのプルーフ機能を有効または無効にする（従来プランのみ）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)の節の説明に従って、「**プルーフユーザー**」オプションが有効になっていることを確認します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>スーパーバイザ－</strong> </td> 
      <td>ユーザーは、組織のアカウントで作成されたすべてのプルーフを管理および表示できます。また、プルーフに追加されたレビュアーを編集することもできます。この権限プロファイルを持つユーザーは、ユーザーの管理や Workfront Proof 設定の編集を行うことはできません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>マネージャー</strong> </td> 
      <td> <p> ユーザーは、組織のアカウントで作成された、または所有するプルーフを管理および表示できます。レビュアーとして追加された場合にのみ、他のユーザーのプルーフを表示できます。これはデフォルト設定です。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理者</strong> </td> 
      <td> ユーザーには、Workfront Proof 管理者権限が付与され、アカウント設定を編集できます。ユーザーは、組織のアカウントで作成されたすべてのプルーフを管理および表示できます。これには、レビュアー、プルーフおよびコメントの追加と削除が含まれます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>カスタム</strong> </td> 
      <td> <p>Workfront Proof でカスタム権限プロファイルを設定している場合にのみ使用できます。</p> <p><b>メモ</b>：  <p>ここで付与する権限プロファイルが、Workfront でのユーザーのアクセスレベル設定よりも高いアクセス権でないことを確認します（<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照）。アクセス権が高い場合、ユーザーは Workfront Proof において Workfront ではアクセスできないプルーフにアクセスできるようになります。</p> <p>これは、<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Adobe Workfront から Workfront Proof へのアクセス</a>で説明されるように、すべての Workfront ユーザーが Workfront から直接 Workfront Proof にアクセスできるようにする予定がある場合に特に重要です。</p> <p>デフォルトでは、Workfront 管理者のみが、Workfront グローバルナビゲーションバーから Workfront Proof サイトへの直接リンクにアクセスできます。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   選択した権限プロファイルは、組織内に存在する各プルーフユーザーに付与されます。

1. 「**変更を保存**」をクリックして、ユーザー設定の更新を完了します。

   >[!NOTE]
   >
   >Workfront でユーザーを作成または更新し、そのユーザーの Workfront メールアドレスが Workfront Proof のライセンスユーザーのものと一致すると、システムは Workfront 内でユーザーに対するプルーフを有効にします。詳しくは、[Adobe Workfront と Workfront Proof 間のユーザー同期](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md)を参照してください。

### 考慮事項

権限を設定する際は、次の点を考慮してください。

* ユーザーの権限プロファイルを権限の少ないプロファイルに変更すると、Workfront 内の既存のプルーフを表示できなくなる場合があります。これは、ユーザーが Workfront 内の別のユーザーとタスクを共有する際に、タスクに関連付けられたプルーフを共有しないと発生する可能性があります（[Adobe Workfront 内でのプルーフの共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)の [Adobe Workfront 内でのプルーフの共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)を参照）。
* Workfront 環境が Workfront Proof Premium アカウントと統合されている場合にのみ、Workfront から Workfront Proof 権限を設定できます。この節で説明したように、プルーフを使できない場合は、Workfront 管理者に問い合わせてください。
* Workfront 環境の少なくとも 1 人のユーザーにプルーフの管理者権限が必要となります。すべてのユーザーからプルーフの管理者権限を削除しようとすると、エラーメッセージが表示されます。
* ユーザーの Workfront アクセスレベルをシステム管理者以外のレベルに変更すると、そのユーザーの Workfront Proof 権限プロファイルはデフォルトでマネージャーに設定されます。

* Workfront のアクセスレベルをシステム管理者に変更すると、プルーフ権限プロファイルが管理者に変わります。

## Workfront のメインメニューから Workfront Proof へのアクセスをすべてのユーザーに設定 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

デフォルトでは、[Adobe Workfront から Workfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) で説明されているように、Workfront 内の管理者権限を持つユーザーのみが Workfront Proof にアクセスできます。

Workfront サポートに連絡してリクエストを送信することで、すべてのユーザーに Workfront メインメニュー内の Workfront Proof ボタンへのアクセスを許可できます。

>[!IMPORTANT]
>
> すべての Workfront ユーザーが Workfront グローバルナビゲーションバーから直接 Workfront Proof にアクセスできるようにする場合は、各ユーザーの権限プロファイルが Workfront 内のユーザーのアクセスレベルを超えるアクセスを提供しないようにしてください。これにより、ユーザーは Workfront 内でアクセスできない Workfront Proof 内のプルーフにアクセスできなくなります。詳しくは、[ユーザーの校正を有効または無効にする（従来のプランのみ）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)を参照してください。

## デスクトッププルーフビューアーへのユーザーアクセスを設定

組織内のユーザーがインタラクティブコンテンツのレビューに web プルーフビューアーではなくデスクトッププルーフビューアーを使用したい場合は、ユーザーがインタラクティブコンテンツのプルーフを開いたときにデスクトッププルーフビューアーが自動的に起動するように設定できます。デスクトッププルーフビューアーと web プルーフビューアーの違いについては、[デスクトッププルーフビューアーについて理解する](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) および [web プルーフビューアーとデスクトッププルーフビューアーの概要の違い](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)を参照してください。

1. Workfront から、グローバルナビゲーションバーの Workfront Proof アイコンをクリックして、Workfront Proof にアクセスします。

   ![](assets/proof-access-proofhq-350x39.png)

1. Workfront Proof の右上隅にある **アカウント設定**&#x200B;をクリックし、「**設定**」タブを選択します。

1. **プルーフのデフォルト**&#x200B;で、**インタラクティブプルーフ用デスクトッププルーフビューアー**&#x200B;行の最後にある&#x200B;**設定**&#x200B;をクリックします。

1. 記事[組織のプルーフ設定を構成](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)の[デスクトップビューアー](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)の説明に従って、デスクトッププルーフビューアーの設定を変更します。

1. 「**保存**」をクリックします。

## インタラクティブなプルーフ用にカスタムデバイスを構成

カスタムデバイスをシステムに追加すると、ユーザーはインタラクティブコンテンツを確認し、デスクトッププルーフビューアーを使用しているときに特定のデバイスでコンテンツがどのように表示されるかをシミュレートできます。（この機能は、ユーザーがインタラクティブコンテンツをレビューできる web プルーフビューアーでは利用できませんが、さまざまなデバイスではなく、さまざまな解像度で表示される場合に限ります。）

詳しくは、[プルーフビューアーでインタラクティブプルーフ解像度を変更](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)を参照してください。

1. [Adobe Workfront から Workfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) の説明に従って、Workfront から Workfront Proof インターフェイスにアクセスします。
1. 記事[組織のプルーフ設定を構成](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)の[プルーフ用にカスタムデバイスを設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)の説明に従って、デスクトッププルーフビューアーの設定を変更します。
