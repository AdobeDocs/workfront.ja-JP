---
product-area: projects
navigation-topic: financials
title: プロジェクトの財務エリアで情報を管理します
description: プロジェクトの財務エリアで情報を管理します
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 3%

---

# プロジェクトの財務エリアで情報を管理します

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

プロジェクトの財務情報を表示または編集するには、「プロジェクトの詳細」セクションの「財務」領域にアクセスします。 この領域で表示または編集できるフィールドは限られています。 プロジェクトのすべての情報を編集する方法については、を参照してください。 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセス権を表示または高くします</p> <p>プロジェクトおよび財務データへのアクセスを編集して、プロジェクトの財務情報を編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務の表示権限を含むプロジェクト以上に対する権限を表示します</p> <p>プロジェクトの財務情報を編集するための財務管理を含むプロジェクトに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 金融分野の概要

「財務」領域で情報を表示または編集する際は、次の点に注意してください。

* [ プロジェクトの詳細 ] の [ 財務 ] 領域に表示される財務情報は、タスクからプロジェクトレベルにロールアップされる値と、プロジェクトに直接入力された情報を表します。 一部の財務情報は、プロジェクトでもタスク・レベルでも管理できます。
* プロジェクトの財務領域を表示するには、プロジェクトでの表示権限と、アクセスレベルからの財務データへのアクセス権が必要です。
* 財務領域の情報を編集するには、プロジェクトに対する管理権限と、アクセスレベルからの財務データへのアクセス権が必要です。 ただし、この領域の情報を編集するのはプロジェクトの所有者のみにすることをお勧めします。

## プロジェクトの財務情報の表示

1. プロジェクトに移動します。
1. クリック **プロジェクトの詳細** をクリックします。
1. 次をクリック： **編集** アイコン ![](assets/edit-icon.png) 「詳細」セクションの右上隅で、 **金融**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Workfrontの管理者がレイアウトテンプレートを設定した方法によっては、「概要」セクションが最初に表示されない場合があります。表示されない場合は折りたたまれます。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. プロジェクトの「財務」領域で、次のフィールドを表示します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">パフォーマンス インデックス メソッド</td> 
      <td> Workfrontが達成額指標の計算に使用する方法を制御します。 時間ベースとコストベースのどちらでもかまいません。 <br>PIM の詳細については、を参照してください。 <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">パフォーマンスインデックスメソッド (PIM) の設定</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>これらは、プロジェクトのパフォーマンスを特定の時間に示すプロジェクトのパフォーマンス指標です。 その値は、パフォーマンスインデックスメソッドに基づいて計算されます。<br>詳しくは、次の記事を参照してください。 </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">コスト効果指数 (CPI) の計算</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">スケジュールパフォーマンスインデックスの計算 (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">CSI(Calculate Cost Schedule Performance Index)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成時総コスト見積り</td> 
      <td> PIM (Performance Index Method) が時間ベースの場合は、プロジェクトの推定総コストを時間単位で表し、Performance Index Method (PIM) がコストベースの場合は、通貨値で表します。<br>「完了時の推定」の計算の詳細については、「 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完了時の推定 (EAC) を計算</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">予算</td> 
      <td>これはプロジェクトの予算セットです。 これは、プロジェクト所有者が手動で指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定コスト</td> 
      <td>これらは、プロジェクトの他のアクティビティとは無関係に、プロジェクトの固定コストです。 プロジェクト所有者が手動で入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定コスト</td> 
      <td>タスクの担当者（ジョブの役割またはユーザー）に関連付けられた予定時間と率に基づく、プロジェクトの概算コストです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際のコスト</td> 
      <td>プロジェクトで発生するすべてのコスト。 「実績原価」は、すべての実績原価の合計です。労務費（実績時間と、それらを記録する役割またはユーザーに関連付けられたレートに基づく）、費用、固定費は、プロジェクトまたはタスクに関連付けることができます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定収益</td> 
      <td>プロジェクトスケジュールに基づいて期待される収益を設定します。 固定売上高は、プロジェクト所有者が手動で指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定収益</td> 
      <td>予定時間とタスクの担当者（ジョブの役割またはユーザー）に関連付けられたレートに基づいて予測される収益。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">実収益</td> 
      <td>タスクの担当者（ジョブの役割またはユーザー）に関連付けられた実績時間および率に基づくプロジェクトの実績収入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">請求済み収益</td> 
      <td> <p>請求レコードにキャプチャされたクライアントまたは他の関係者に請求される収益。 請求レコードの詳細については、「 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">請求レコードの作成</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## プロジェクトの財務情報の編集

プロジェクト所有者は、プロジェクトの「財務」サブタブの情報を編集できます。

「プロジェクト財務」サブタブの情報を編集する手順は、次のとおりです。

1. 自分が所有しているプロジェクトに移動します。

   >[!NOTE]
   >
   >次の手順を実行するには、プロジェクトに対する管理権限が必要です。 また、プロジェクトの「財務」サブタブを変更するのは、プロジェクト所有者のみにすることをお勧めします。

1. クリック **プロジェクトの詳細** をクリックします。
1. 次をクリック： **編集** アイコン ![](assets/edit-icon.png) 「詳細」セクションの右上隅で、 **金融** . 「財務」領域が開き、編集できます。
1. フィールドをシングルクリックまたはクリックして、編集可能なフィールドを編集します。 **+追加** をクリックして、空のフィールドに情報を追加します。

   >[!TIP]
   >
   >Workfrontによって自動的に計算されるフィールドや、編集権限を持っていないフィールドは、編集できません。

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. 以下のフィールドを更新します。

   >[!NOTE]
   >
   >Workfront管理者がレイアウトテンプレートを設定する方法によっては、環境によって「プロジェクトの詳細」セクションのフィールドが異なる場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">パフォーマンス インデックス メソッド</td> 
      <td> <p>Workfrontがプロジェクトのパフォーマンス指標の計算に使用する方法を制御します。 これは管理者がシステムレベルで設定しますが、プロジェクトレベルで編集することもできます。 次のオプションの 1 つを選択することを検討してください。</p> 
       <ul> 
        <li><strong>時間ベース：</strong>Workfrontでは、プロジェクトの CPI と EAC の計算に「計画時間」が使用され、プロジェクトの EAC は時間単位の数値で表示されます。 </li> 
        <li><strong>コストベース：</strong>Workfrontは、プロジェクトの CPI と EAC の計算に計画労務費を使用し、EAC は通貨値として表示されます。 このオプションを選択する場合は、タスクの担当者（ジョブの役割またはユーザー）がコスト率に関連付けられていることを確認します。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成時総コスト見積り</td> 
      <td> <p>完了時のプロジェクトまたはタスクの推定総コストを表します。 これは管理者がシステムレベルで設定しますが、プロジェクトレベルで編集することもできます。 次のオプションの 1 つを選択することを検討してください。</p> 
       <ul> 
        <li><strong>プロジェクトレベルで計算</strong>:親タスクおよびプロジェクトの EAC は、EAC 式に実績時間/実績労務費を入力することで決定されます。 この計算には、実績時間数/コストと費用が親タスクまたはプロジェクトに直接追加されます。</li> 
        <li><strong>タスク/サブタスクからのロールアップ</strong>:親タスクとプロジェクトの EAC は、各子タスクの EAC を合計することで決定されます。 この計算では、親タスクまたはプロジェクトに直接追加された実績時間/コストと費用が除外されます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予算</td> 
      <td>このプロジェクトの予算を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定コスト</td> 
      <td>このプロジェクトの固定コストを指定します。 これには、労務費や費用費用は含まれません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定収益</td> 
      <td> <p>このプロジェクトの固定売上高を指定します。 パートナーやサードパーティに対して請求された請求レコードから得られる売上高は含まれません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクトの通貨</td> 
      <td> <p>システム内のデフォルトの通貨と異なる場合は、このプロジェクトの通貨を指定します。 システムのデフォルトの通貨は、Workfront管理者が定義します。 Workfrontでの為替レートの設定について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. 「**変更を保存**」をクリックします。
