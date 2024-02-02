---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのイニシアチブを削除
description: 自分が作成した計画や、誰かが自分と共有した計画のイニシアチブを削除できます。削除したイニシアチブを復元することはできません。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: ht
source-wordcount: '529'
ht-degree: 100%

---

# [!DNL Scenario Planner]内のイニシアチブを削除

自分が作成した計画や、誰かが自分と共有した計画のイニシアチブを削除できます。削除したイニシアチブを復元することはできません。

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
   <td> <p>[!DNL Adobe Workfront]<b>ライセンス*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>この記事で説明する機能にアクセスするためには、[!DNL Adobe Workfront Scenario Planner] 用の追加ライセンスを購入する必要があります。 </p> <p>[!DNL Workfront Scenario Planner]の取得について詳しくは、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!UICONTROL Scenario Planner] を使用するために必要なアクセス権</a>の記事を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>次に対する[!UICONTROL Edit]以上のアクセス権： [!DNL Scenario Planner]</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>プランに対する[!UICONTROL Manage]権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a>でのプランへの利用申請を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イニシアチブを削除

イニシアチブを削除する際は、以下の点を考慮してください。

* イニシアチブを削除すると、そのイニシアチブに関連付けられている必要な担当業務数とコスト情報がプランから削除されます。
* プロジェクトを読み込んで作成したイニシアチブを削除しても、イニシアチブに関連付けられたプロジェクトは削除されません。
* 1 回以上プロジェクトに公開されたイニシアチブを削除すると、結果として以下のようになります。

   * イニシアチブはシナリオから削除されますが、[!DNL Scenario Planner]エリアは「[!UICONTROL プロジェクトの詳細]」セクションに残ります。
   * 削除したイニシアチブがシナリオで唯一の公開イニシアチブである場合は、プランが公開されたことを示す指標も削除されます。

     プロジェクトへのイニシアチブの公開について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトのアップデートまたは作成を参照してください。

     プロジェクトの読み込みによるイニシアチブの作成について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) のプランにプロジェクトを読み込むを参照してください。

1 度に 1 つのイニシアチブを削除することも、複数のイニシアチブを一括で削除することもできます。

* [イニシアチブを 1 つ削除](#delete-one-initiative)
* [イニシアチブを一括削除](#delete-initiatives-in-bulk)

### イニシアチブを 1 つ削除 {#delete-one-initiative}

1. **[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「[!UICONTROL シナリオ]」の順にクリックします。

   計画のリストが表示されます。

1. 計画の名前をクリックして開き、削除するイニシアチブを確認します。
1. 次のいずれかの操作を行います。

   * イニシアチブ名の右側にある&#x200B;**[!UICONTROL その他のメニュー]** ![](assets/more-menu.png)、**[!UICONTROL 削除]**／**[!UICONTROL はい、削除します]**&#x200B;の順にクリックします。

   * イニシアチブの左側にあるボックスを選択し、計画の下部に表示されるフローティングメニューで「**[!UICONTROL 削除]**」、「**[!UICONTROL はい、削除します]**」の順にクリックします。

   イニシアチブとその担当業務およびコスト情報は、プランから削除されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。

### イニシアチブを一括削除 {#delete-initiatives-in-bulk}

1. **[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「[!UICONTROL シナリオ]」の順にクリックします。

   計画のリストが表示されます。

1. 計画の名前をクリックして開き、削除するイニシアチブを確認します。
1. 削除するイニシアチブの左側にあるボックスを選択し、計画の下部に表示されるメニューから、「**[!UICONTROL 削除]**」、「**[!UICONTROL はい、削除します]**」の順にクリックします。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   イニシアチブとその担当業務およびコスト情報は、プランから削除されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。
