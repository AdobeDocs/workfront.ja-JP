---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: ユーザーの共有設定を構成します
description: Adobe Workfrontの管理者またはWorkfrontの配達確認管理者は、配達確認を共有できるユーザーアカウント、配達確認のすべてのバージョンを表示できるかどうか、およびユーザーが共有項目にアクセスできるタイミングを設定できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# ユーザーの共有設定を構成します

Adobe Workfrontの管理者またはWorkfrontの配達確認管理者は、配達確認を共有できるユーザーアカウント、配達確認のすべてのバージョンを表示できるかどうか、およびユーザーが共有項目にアクセスできるタイミングを設定できます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：Premium または Select</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>配達確認権限プロファイルで管理者が選択されている必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">ユーザーの校正アクセスを設定する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 他のアカウントとの共有を設定する

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定**」、「 **設定** タブをクリックします。

1. 内 **共有** セクション（の右） **との共有を許可**&#x200B;をクリックし、 **設定**.

1. 表示されるドロップダウンリストで、配達確認を誰でも使用できるようにするか、配達確認の共有を自分のアカウントのみに制限するか、自分のアカウントと共同作業中の任意のパートナーアカウントに制限するかを指定するオプションを選択します。
1. クリック **保存します。**

## 共有配達確認のすべてのバージョンを表示する設定

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定**」、「 **設定** タブをクリックします。

1. 内 **共有** セクション（の右） **受信者はすべてのバージョンを表示できます**&#x200B;を選択します。 **有効にする** または **無効にする** ：配達確認 URL が有効な場合に、受信者が校正ビューア内のすべてのバージョンの配達確認を表示するかどうかを指定します。

## ワークフローステージアクティビティに基づく配達確認の表示を設定

自動ワークフローを使用した配達確認を、特定のステージに関連付けられたユーザーにいつ表示するかを指定できます。

>[!NOTE]
>
>* このオプションは、スタンドアロンのWorkfront Proof アプリケーションを使用する場合にのみ使用できます。Workfrontと統合されているWorkfront Proof インスタンスを使用している場合や、Workfront内での校正時には使用できません。
>* この設定に関係なく、ユーザーが関連付けられたステージに入った後にのみ、配達確認に関する電子メール通知がユーザーに送信されます。
>


自動ワークフローを使用した配達確認をユーザーに表示するタイミングを設定するには：

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定**」、「 **設定** タブをクリックします。

1. 内 **共有** セクション、有効または無効 **ステージのアクティベーションに基づく配達確認の表示**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>無効</strong> （デフォルト）</td> 
      <td>配達確認は、配達確認の作成時にユーザーに表示されます。<br><p>配達確認のワークフローのステージに関連付けられたユーザーは、配達確認の作成直後に検索結果に配達確認を表示できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>有効</strong> </td> 
      <td> <p>配達確認は、関連付けられたステージが <strong>アクティブ。</strong></p> <p><b>メモ</b>:   
        <ul> 
         <li><em style="font-style: normal;">このオプションを有効にした後も、作成時に表示可能なユーザーには、既存の配達確認が表示されます。</em> </li> 
         <li>ユーザーが配達確認のバージョンにアクセスできるようになった後（ユーザーが関連付けられているステージがアクティブになるため）、ユーザーはステージがアクティブになっているバージョンのみを表示できます。 以前のバージョンが、ユーザーが関連付けられているステージに到達しなかった場合、ユーザーは配達確認のそのバージョンを表示できません。</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
