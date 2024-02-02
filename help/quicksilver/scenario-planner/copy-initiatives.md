---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのイニシアチブをコピーする
description: 既存のイニシアチブをコピーして、イニシアチブを作成できます。自分が作成したプランや、誰かが自分と共有するプランのイニシアチブをコピーできます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: ht
source-wordcount: '504'
ht-degree: 100%

---

# [!DNL Scenario Planner] 内のイニシアチブをコピーする

既存のイニシアチブをコピーして、イニシアチブを作成できます。自分が作成したプランや、誰かが自分と共有するプランのイニシアチブをコピーできます。

## アクセス要件

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> プラン*</b> </p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> ライセンス</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>この記事で説明する機能にアクセスするためには、[!DNL Adobe Workfront Scenario Planner] 用の追加ライセンスを購入する必要があります。</p> <p>[!DNL Workfront Scenario Planner]の取得については、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a>の使用に必要なアクセス権を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>次に対する[!UICONTROL Edit]以上のアクセス権： [!DNL Scenario Planner]</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>プランに対する[!UICONTROL Manage]権限</p> <p>計画への追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a> の計画へのアクセスをリクエストを参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イニシアチブをコピーする

イニシアチブをコピーする際は、次の点に注意してください。

* イニシアチブをコピーすると、コピーは元のイニシアチブと同じプランに配置されます。
* イニシアチブをコピーして、元のイニシアチブから次の情報を新しいイニシアチブに追加します。

   * [!UICONTROL 期間]
   * [!UICONTROL 担当業務]
   * [!UICONTROL ユーザー]および[!UICONTROL 固定コスト]
   * [!UICONTROL 予定便益]

* イニシアチブをコピーすると、元のイニシアチブに情報が存在する場合に、プランの次の情報を変更できます。

   * 必要な担当業務数
   * [!UICONTROL コスト]
   * [!UICONTROL プランの稼動率]
   * 担当業務の稼動率
   * [!UICONTROL 純価]

* プロジェクトを読み込んで作成されたイニシアチブ、または少なくとも 1 回プロジェクトに公開されたイニシアチブをコピーすると、次のような影響があります。

   * イニシアチブに関連付けられたプロジェクトは複製されません。
   * コピーしたイニシアチブはプロジェクトに接続されません。
   * 1 回以上公開されているプロジェクトの場合、プロジェクトの [!DNL Scenario Planner] セクションは変更されません。

  プロジェクトへのイニシアチブの公開について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトのアップデートまたは作成を参照してください。

  プロジェクトの読み込みによるイニシアチブの作成について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) のプランにプロジェクトを読み込むを参照してください。

## イニシアチブをコピーする

1. **[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「[!UICONTROL シナリオ]」の順にクリックします。

   計画のリストが表示されます。

1. プランの名前をクリックして開き、コピーするイニシアチブを確認します。
1. コピーするイニシアチブの左側にあるボックスを選択し、プランの下部に表示されるメニューから、「**[!UICONTROL コピー]**」をクリックします。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] はイニシアチブをすぐにコピーし、最後に選択したイニシアチブの下に配置します。

   コピーされたイニシアチブの名前は、* のコピー`<Name of original initiative>`*&#x200B;です。

   >[!NOTE]
   >
   >新しいイニシアチブの挿入場所に応じて、既存のイニシアチブの数が変わる場合があります。

1. コピーしたイニシアチブの名前を更新します。

   >[!TIP]
   >
   >イニシアチブを再度コピーする場合に混乱を避けるために、必ずイニシアチブの名前を更新することをお勧めします。

1. （オプション）新しく作成したイニシアチブの優先度を更新します。

   イニシアチブの優先順位について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md) のイニシアチブ優先度を更新を参照してください。

1. 「**[!UICONTROL プランを保存]**」をクリックして、変更を保存します。
