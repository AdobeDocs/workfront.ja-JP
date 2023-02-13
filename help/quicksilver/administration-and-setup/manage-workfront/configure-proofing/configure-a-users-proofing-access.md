---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: ユーザーの校正アクセスを設定する
description: Adobe Workfront管理者またはWorkfrontの配達確認管理者は、WorkfrontとWorkfrontの配達確認を作成および表示するためのユーザーのアクセス権を設定できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# ユーザーの校正アクセスを設定する

Adobe Workfront管理者またはWorkfrontの配達確認管理者は、WorkfrontとWorkfrontの配達確認を作成および表示するためのユーザーのアクセス権を設定できます。

基本校正と統合校正に使用できる校正機能について詳しくは、 [Workfrontの校正機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront管理者またはWorkfront Proof 管理者である必要があります。 Workfront管理者について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ユーザーの校正を有効または無効にする（レガシープランのみ） {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

従来の Select または Premium Workfrontプランを使用している場合は、Workfront管理者として、ユーザーの校正機能を有効または無効にできます。

ユーザーの校正を有効にすると、Workfrontでユーザーの配達確認を自動的に生成するオプションが有効になります。

ユーザーは校正ユーザーとして有効にできますが、WorkfrontのメインメニューからWorkfront Proof インターフェイスに直接移動するには、管理者権限が必要です。 Workfrontシステムのすべての校正ユーザーに対してこのオプションを有効にする方法について詳しくは、 [WorkfrontのメインメニューからのWorkfront配達確認へのアクセスを、すべてのユーザーに設定します](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. 内 **メインメニュー**&#x200B;を選択します。 **ユーザー**.

1. ユーザーを選択し、 **編集** アイコン
1. 内 **アクセス** セクション、選択または選択解除 **ユーザーが配達確認を生成できる**.

## ユーザーの配達確認権限プロファイルの設定

選択した権限プロファイルは、組織内に存在する各配達確認のユーザーに付与されます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).
1. 1 人または複数のユーザーを選択し、「 **編集**.

1. 内 **アクセス** 」セクションで、「 Workfront Proof 権限」オプション ( **配達確認権限プロファイル** ドロップダウンメニュー：

   >[!NOTE]
   >
   >レガシーWorkfrontプランの場合は、 **ユーザーが配達確認を生成できる** オプションが有効になっている場合は、前述の節で説明したように [ユーザーの校正を有効または無効にする（レガシープランのみ）](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>スーパーバイザ－</strong> </td> 
      <td>ユーザーは、組織のアカウントで作成されたすべての配達確認を管理および表示できます。 また、配達確認に追加されたレビュー担当者を編集することもできます。 この権限プロファイルを持つユーザーは、ユーザーの管理やWorkfront Proof 設定の編集をおこなうことができません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>マネージャー</strong> </td> 
      <td> <p> ユーザーは、組織のアカウントで作成または所有する配達確認を管理および表示できます。 レビュー担当者として追加された場合にのみ、他のユーザーの配達確認を表示できます。 これはデフォルト設定です。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理者</strong> </td> 
      <td> ユーザーには、Workfront Proof の管理者権限が付与され、アカウント設定を編集できます。 ユーザーは、組織のアカウントで作成されたすべての配達確認を管理および表示できます。 これには、レビュー担当者、配達確認、コメントの追加と削除が含まれます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザー定義</strong> </td> 
      <td> <p>Workfront Proof 内でカスタム権限プロファイルを設定している場合にのみ使用できます。</p> <p><b>メモ</b>:  <p>ここで許可した権限プロファイルが、Workfrontでのユーザーのアクセスレベル設定よりも高いアクセス権を提供しないようにします ( <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>) をクリックします。 アクセス権が高い場合、ユーザーはWorkfront配達確認内で、Workfront内でアクセスできないという配達確認にアクセスできます。</p> <p>これは、すべてのWorkfrontユーザーがWorkfrontから直接Workfront配達確認にアクセスできるようにする予定がある場合に特に重要です。詳しくは、 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Adobe WorkfrontからWorkfront Proof にアクセス</a>.</p> <p>デフォルトでは、Workfront管理者のみが、WorkfrontグローバルナビゲーションバーからWorkfront Proof サイトへの直接リンクにアクセスできます。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   選択した権限プロファイルは、組織内に存在する各配達確認のユーザーに付与されます。

1. クリック **変更を保存** をクリックして、ユーザー設定の更新を完了します。

   >[!NOTE]
   >
   >Workfrontでユーザーを作成または更新し、そのユーザーのWorkfront電子メールアドレスがライセンス済みのWorkfront配達確認ユーザーの電子メールアドレスと一致する場合、Workfront内でのユーザーの校正が可能になります。 詳しくは、 [Adobe WorkfrontとWorkfrontの配達確認間のユーザー同期](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### 注意点

権限を設定する際は、次の点を考慮してください。

* ユーザーの権限プロファイルを権限の少ないプロファイルに変更すると、Workfront内の既存の配達確認を表示できなくなる場合があります。 これは、ユーザーがWorkfront内のユーザーとタスクを共有したが、タスクに関連付けられた配達確認を共有していない場合に発生する可能性があります ( [Adobe Workfront内での配達確認の共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Adobe Workfront内での配達確認の共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)) をクリックします。
* Workfront環境がWorkfront Proof Premium アカウントと統合されている場合にのみ、WorkfrontからWorkfrontの配達確認権限を設定できます。 この節で説明したように、校正を使用できない場合は、Workfront管理者にお問い合わせください。
* Workfront環境の少なくとも 1 人のユーザーに、校正のための管理者権限が必要です。 すべてのユーザーから校正のための管理者権限を削除しようとすると、エラーメッセージが表示されます。
* ユーザーのWorkfrontアクセスレベルをシステム管理者以外のレベルに変更すると、そのユーザーのWorkfront配達確認権限プロファイルはデフォルトで Manager に設定されます。

* Workfrontのアクセスレベルをシステム管理者に変更すると、配達確認権限プロファイルが「管理者」に変わります。

## WorkfrontのメインメニューからのWorkfront配達確認へのアクセスを、すべてのユーザーに設定します {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

デフォルトでは、Workfront内の管理者権限を持つユーザーのみが、説明に従ってWorkfrontの配達確認にアクセスできます  [Adobe WorkfrontからWorkfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Workfrontのメインメニュー内の「 Workfront Proof 」ボタンへのアクセス権をすべてのユーザーに付与するには、Workfrontサポートに問い合わせ、リクエストを送信します。

>[!IMPORTANT]
>
> すべてのWorkfrontユーザーがWorkfrontグローバルナビゲーションバーから直接Workfront配達確認にアクセスできるようにする場合は、各ユーザーの権限プロファイルがWorkfront内のユーザーのアクセスレベルより多くのアクセスを提供しないようにします。 これにより、ユーザーは、Workfront Proof 内で、Workfront内でアクセスできない配達確認にアクセスできなくなります。 詳しくは、 [ユーザーの校正を有効または無効にする（レガシープランのみ）](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## デスクトップ校正ビューアへのユーザーアクセスを設定する

組織内のユーザーが Web 校正ビューアの代わりにデスクトップ校正ビューアを使用してインタラクティブコンテンツを確認する場合は、インタラクティブコンテンツの配達確認を開いたときにデスクトップ校正ビューアが自動的に起動するように設定できます。 デスクトップ校正ビューアと Web 校正ビューアの違いについて詳しくは、 [デスクトップ校正ビューアについて](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) および [Web 校正ビューアとデスクトップ校正ビューアの違いの概要](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Workfrontで、グローバルナビゲーションバーの「 Workfront配達確認」アイコンをクリックして、Workfront配達確認にアクセスします。

   ![](assets/proof-access-proofhq-350x39.png)

1. クリック **アカウント設定** Workfront Proof の右上隅近くにある **設定** タブをクリックします。

1. の下 **配達確認のデフォルト**( **インタラクティブ校正用デスクトップ校正ビューア** 行、クリック **設定**.

1. デスクトップ校正ビューアの設定を変更します。詳しくは、 [デスクトップ校正ビューア](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) 記事内 [組織の配達確認設定を構成します](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. 「**保存**」をクリックします。

## インタラクティブな配達確認のカスタムデバイスの設定

任意のカスタムデバイスをシステムに追加して、ユーザーがデスクトップ校正ビューアを使用しているときに、インタラクティブなコンテンツを確認し、特定のデバイスでのコンテンツの表示をシミュレートできます。 （この機能は Web 校正ビューアでは使用できません。ユーザーはインタラクティブコンテンツを確認できますが、様々なデバイスでは表示されず、様々な解像度で表示されます。）

詳しくは、 [校正ビューアでインタラクティブな配達確認の解像度を変更](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Workfrontから、Workfront Proof インターフェイスにアクセスします ( [Adobe WorkfrontからWorkfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. デスクトップ校正ビューアの設定を変更します。詳しくは、 [配達確認用のカスタムデバイスの設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) 記事内 [組織の配達確認設定を構成します](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
