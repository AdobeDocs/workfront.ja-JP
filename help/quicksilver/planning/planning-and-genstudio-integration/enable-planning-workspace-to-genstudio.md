---
title: Workfront計画WorkspaceからGenStudio for Performance Marketingを有効にする
description: 両方のアプリケーションにアクセスできる場合は、GenStudio for Performance MarketingでAdobe Workfront計画ワークスペースを使用できます。
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 6%
---
# GenStudio for Performance Marketingに対するWorkfront計画ワークスペースの有効化

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

会社がAdobe GenStudio for Performance Marketingも購入し、Adobe Workfront Planningのユーザーである場合、GenStudio WorkspaceはWorkfront Planningでも使用できます。

Workfront Planningにプランニングワークスペースが既にある場合は、GenStudioで同じデータを再作成する代わりに、GenStudio for Performance Marketingに対して有効にすることができます。

ワークスペースを有効にすると、そのワークスペースがAdobe Could Storage プロジェクトにリンクされ、そのレコードタイプとフィールドがGenStudio ワークスペースにマッピングされます。 設定が完了したら、GenStudioでワークスペースのレコードを開くことができます。

以下が必要です。

* Workfront PlanningとGenStudio for Performance Marketingの両方にアクセスできます。
* Adobe Cloud Storage プロジェクトをワークスペースにリンクします。 組織管理者は、Adobe Admin Consoleで組織管理者を作成できます。

  詳しくは、[Adobe ストレージの管理](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)を参照してください。<!--ensure this site still works-->

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontまたはワークフローとプランニングパッケージ</p> 
または
<p>スタンドアロン製品として購入された場合の任意のプランニング・パッケージ</p>

</td> 
   <tr> 
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Adobe Admin Consoleの設定</p> </td> 
   <td> 
   <p> Adobe Admin ConsoleでAdobe Storage Cloud プロジェクトを作成する必要があります </p>

<p>詳しくは、<a href="https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies"> プロジェクトの管理</a>を参照してください

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>計画標準</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Adobe Workfront アクセスレベルの設定</p></td> 
   <td> <p>ワークフローとプランニングパッケージの両方を持っている場合は、ワークフローとプランニングライセンスタイプの両方をWorkfront アクセスレベルに追加する必要があります</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketingのユーザーロール</p></td> 
   <td><p><ul><li>キャンペーン、製品、ペルソナにアクセスする必要がある場合は、GenStudioのあらゆるユーザーロールを利用できます</li>
   <li>アクティベーションにアクセスする必要がある場合は、GenStudio System Manager <!--and Events--></li></ul>
   詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> ユーザーの役割と権限</a>を参照してください。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  
   <p>Workfront Planningでは、次の操作を行います。 </p>
   <ul>
   <li><p>ワークスペースへの権限の管理 <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>Adobe GenStudio for Performance Marketingで： <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> Adobe GenStudio for Performance Marketingで権限を作成して項目を作成する</p></li></ul>
   </td>  
</tbody> 
</table>

Adobe Workfront計画アクセスについて詳しくは、[Adobe Workfront計画アクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。

Adobe GenStudio for Performance Marketingについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home)を参照してください。

+++ 

## GenStudioに対するWorkfront計画ワークスペースの有効化

1. Workfront Planningで、有効にするワークスペースを開きます。
1. ワークスペース名の右側にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、「**GenStudioを有効にする**」をクリックします。

   「**ワークスペースをGenStudio**&#x200B;有効にする」ボックスが開き、次の手順を実行します。

   1. **ACPC プロジェクト**：このワークスペースと同期する&#x200B;**ACPC プロジェクト** （Adobe Cloud Storage プロジェクト）を選択し、**次へ**&#x200B;をクリックします。 ユーザーは、このプロジェクトを通じてGenStudioのワークスペースにアクセスします。

      ![Workspace GenStudioを有効にする – ACPC プロジェクト手順](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **レコードタイプ**: ワークスペースのレコードタイプを、GenStudioで必要な6つのレコードタイプにマッピングします。

      * キャンペーン
      * 製品
      * ペルソナ
      * チャネル
      * 地域
      * アクティベーション

      それぞれに対して、リストを開いて、一致するプランニング レコード タイプを選択するか、**新しい**&#x200B;を追加を選択して作成し、**次へ**&#x200B;をクリックします。

      ![Workspace GenStudioを有効にする – レコードタイプの手順](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **フィールド**：各レコードタイプのフィールドをマッピングします。 ダイアログの上部にあるタブを使用して、レコードタイプ間を移動します。 各フィールドについて、一致する計画フィールドを選択するか、**新規を追加**&#x200B;を選択してフィールドを作成します。

      すべてのレコードタイプについて、フィールド設定を繰り返します。

      ![ ワークスペース GenStudioを有効にする – フィールド ステップ ](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. 警告を確認して対処します。

      例えば、新しいフィールドをレコードタイプのプライマリフィールドにしたり、既に使用されているフィールドエイリアスの名前を変更したりできます（既に「リージョン」という名前のフィールドがある場合、読み込まれたフィールドは「リージョン 2」になります）。

      **ステータス** フィールドをマッピングすると、必要なオプションが追加されます。

   1. 「**公開**」をクリックします。

      ワークスペースを有効にすると、確認メッセージが表示されます。 マッピングされたレコードタイプは、ワークスペースでマークされます。

      GenStudioからアクセスできるようにマッピングされたレコードタイプには、カードに新しい&#x200B;**Adobe** アイコンが追加されています。

      ![Adobe アイコンを含むキャンペーンのレコードタイプ ](assets/campaigns-record-type-card-with-adobe-icon.png)

1. GenStudioを開き、「**キャンペーン**」を選択し、画面の左下隅にあるこの設定のために設定した&#x200B;**ACPC プロジェクト**&#x200B;をクリックします。 読み込んだレコードタイプとフィールドを確認します。

   >[!TIP]
   >
   >Adobe Cloud Storage プロジェクトメンバーシップが許可するレコードのみが表示されます。
