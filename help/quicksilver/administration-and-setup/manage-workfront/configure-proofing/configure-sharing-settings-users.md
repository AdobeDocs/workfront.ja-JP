---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: ユーザーの共有設定の指定
description: Adobe Workfront 管理者または Workfront Proof 管理者は、プルーフを共有できるユーザーアカウント、ユーザーがプルーフのすべてのバージョンを表示できるかどうか、およびユーザーが共有アイテムにアクセスできるタイミングを設定できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '607'
ht-degree: 100%

---

# ユーザーの共有設定の指定

Adobe Workfront 管理者または Workfront Proof 管理者は、プルーフを共有できるユーザーアカウント、ユーザーがプルーフのすべてのバージョンを表示できるかどうか、およびユーザーが共有アイテムにアクセスできるタイミングを設定できます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Premium または選択</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プルーフ権限プロファイルで管理者を選択しておく必要があります。詳細については、<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">ユーザーのプルーフアクセスの設定</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 他のアカウントとの共有の設定

1. Workfront で、メインメニュー ![](assets/main-menu-icon.png) をクリックし、プルーフ ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. **設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブをクリックします。

1. 「**共有**」セクションで、「**共有を許可**」の右側にある「**設定**」をクリックします。

1. 表示されるドロップダウンリストで、プルーフを誰でも使用できるようにするか、プルーフの共有を自分のアカウントのみに制限するか、プルーフを自分のアカウントと共同作業中の任意のパートナーアカウントに制限するかを指定するオプションを選択します。
1. 「**保存**」をクリックします。

## 共有プルーフのすべてのバージョンの表示の設定

1. Workfront で、メインメニュー ![](assets/main-menu-icon.png) をクリックし、プルーフ ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. **設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブをクリックします。

1. 「**共有**」セクションで、「**受信者はすべてのバージョンを表示可能**」の右側にある「**有効にする**」または「**無効にする**」を選択して、プルーフ URL が有効になっている場合に、受信者がプルーフビューア内でプルーフのすべてのバージョンを表示できるようにするかどうかを指定します。

## ワークフローステージアクティビティに基づいたプルーフの表示の設定

自動ワークフローを使用したプルーフを、特定のステージに関連付けられたユーザーにいつ表示するかを指定できます。

>[!NOTE]
>
>* このオプションは、スタンドアロンの Workfront Proof アプリケーションを使用する場合にのみ使用できます。Workfront と統合された Workfront Proof インスタンスを使用する場合や、Workfront 内でのプルーフを行う場合は使用できません。
>* この設定に関係なく、ユーザーが関連付けられているステージにプルーフが入った後にのみ、プルーフに関するメール通知がユーザーに送信されます。
>

自動ワークフローを使用したプルーフをユーザーに表示するタイミングを設定するには：

1. Workfront で、メインメニュー ![](assets/main-menu-icon.png) をクリックし、プルーフ ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. **設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブをクリックします。

1. 「**共有**」セクションで、「**ステージアクティベーションに基づいたプルーフの表示**」を有効または無効にします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>無効</strong>（デフォルト）</td> 
      <td>プルーフは、プルーフが作成された時点でユーザーに表示されます。<br><p>プルーフのワークフローのステージに関連付けられているユーザーは、プルーフの作成直後に検索結果でプルーフを表示できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>有効</strong> </td> 
      <td> <p>プルーフは、ユーザーが関連付けられているステージが<strong>アクティブ</strong>になった後でのみユーザーに表示されます。</p> <p><b>メモ</b>:   
        <ul> 
         <li><em style="font-style: normal;">このオプションを有効にした後も、既存のプルーフは、そのプルーフが作成されたときに表示できたユーザーには引き続き表示されます。</em> </li> 
         <li>ユーザーがプルーフのバージョンにアクセスできるようになった後（ユーザーが関連付けられているステージがアクティブになったため）、ユーザーはステージがアクティブになっているバージョンのみを表示できます。以前のバージョンが、ユーザーが関連付けられているステージに到達していない場合、ユーザーはプルーフのそのバージョンを表示できません。</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
