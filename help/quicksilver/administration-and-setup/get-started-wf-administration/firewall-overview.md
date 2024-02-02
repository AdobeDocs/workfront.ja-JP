---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: ファイアウォールの概要
description: Adobe Workfront は組織のネットワークと通信するので、組織のファイアウォールがその通信を許可するように設定されている必要があります。ファイアウォールは、組織のネットワークをインターネットから分離することによって機能する、非常に効果的なセキュリティ対策です。これにより、選択したデータとネットワークトラフィックのみが組織のネットワークに出入りできるようになります。ファイアウォールは、データの送受信を行うサイトに基づいて、データを許可またはブロックします。Adobe Workfront 管理者は、Workfront との間で送信されるデータが組織のファイアウォールを通過できることを確認する必要があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d74b0aa22644b7c79d3c6c3c3bbd5e67efdff732
workflow-type: ht
source-wordcount: '742'
ht-degree: 100%

---

# ファイアウォールの概要

Adobe Workfront は組織のネットワークと通信するので、組織のファイアウォールがその通信を許可するように設定されている必要があります。ファイアウォールは、組織のネットワークをインターネットから分離することによって機能する、非常に効果的なセキュリティ対策です。これにより、選択したデータとネットワークトラフィックのみが組織のネットワークに出入りできるようになります。ファイアウォールは、データの送受信を行うサイトに基づいて、データを許可またはブロックします。Adobe Workfront 管理者は、Workfront との間で送信されるデータが組織のファイアウォールを通過できることを確認する必要があります。

これは、基本的に、ファイアウォールを介したデータの送受信が「許可」されているサイトの「リスト」である許可リストを通じて実現されます。サイトは、次の 2 つの方法のいずれかで識別できます。

* **IP アドレス**：52.31.132.175 などの一連の数値
* **ドメイン**：URL の一部（www.thisdomain.com の「thisdomain」など）

Workfront は、web 通信に特定の IP アドレスおよびドメインを使用します。組織で Workfront を使用するには、これらを組織の許可リストに追加する必要があります。

通常、許可リストはネットワーク管理者によって設定されます。組織のネットワーク管理者と協力して、ファイアウォールでこれらの IP アドレスが許可されていることを確認します。ネットワーク管理者が誰であるかわからない場合は、組織の IT 部門が正しい方向を示してくれます。

>[!IMPORTANT]
>
>Workfront 管理者は、これらの IP アドレスとドメインが組織の許可リストに追加されていることを確認する必要があります。これは、自分で追加しない場合でも当てはまります。Workfront は組織の許可リストを設定できません。

## ファイアウォールを設定するための情報を収集する

Workfront 用のファイアウォールを設定するには、追加する IP アドレスとドメインをネットワーク管理者が知っておく必要があります。この情報の一部は、Workfront 管理者のみが使用できます。Workfront 管理者は、この情報を探してネットワーク管理者に提供する必要があります。

>[!NOTE]
>
>セキュリティのベストプラクティスは、組織が積極的に使用している機能に接続する IP アドレスとドメインのみを追加することです。この情報を提供することで、このベストプラクティスに確実に従うことができます。

ネットワーク管理者に次の情報を提供してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">許可する特定の IP アドレスおよびドメイン</td> 
   <td> <p><a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">ファイアウォールの許可リストを設定</a>の記事には、組織が許可リストに追加する必要がある IP アドレスとドメインのリストが含まれています。 </p> <p>ネットワーク管理者が「ファイアウォールを設定」の記事にアクセスできない可能性があります。その場合は、それを提供する必要があります。ハード（紙）コピーは印刷しないことをお勧めします。デジタルコピーを使用すると、ネットワーク管理者はアドレスをコピーして貼り付けることができます。これは、ハードコピーから入力するよりも迅速かつ正確です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">クラスター</td> 
   <td>組織のクラスターを検索するには、<a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">組織のクラスターと Workfront プランを表示</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront プラン</td> 
   <td> <p>組織のプランを検索するには、<a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">組織のクラスターと Workfront プランを表示</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ドメイン</td> 
   <td> <p>ドメインを見つけるには、Workfront に接続するために使用する web アドレスを確認します。</p> <p>例：web アドレス <code>greatcompany.my.workfront.com</code> では、ドメインは「greatcompany」です</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">その他の Adobe Workfront 製品</td> 
   <td> <p>次のいずれかのライセンスを持っている場合は、ネットワーク管理者に通知します。</p> 
    <ul> 
     <li> <p>Adobe Workfront Proof</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 統合</td> 
   <td>次のいずれかを使用する場合は、ネットワーク管理者に通知します。
    <ul>
     <li><p><p>Workfront for Jira</p></p></li>
     <li><p>Workfront for G Suite</p></li>
     <li><p>Workfront for Microsoft Teams</p></li>
     <li><p>Workfront for Outlook</p></li>
     <li><p>Workfront for Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">その他の機能</td> 
   <td> <p>次のいずれかを使用する場合は、ネットワーク管理者に通知します。</p> 
    <ul> 
     <li> <p>Workfront 体験版</p> </li> 
     <li> <p>Workfront Ascent</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>後日、これらの製品、統合、または機能のいずれかを追加する場合は、ネットワーク管理者に連絡して許可リストを調整してもらう必要があります。

### 組織のクラスターと Workfront プランを表示する {#view-your-organization-s-cluster-and-workfront-plan}

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**システム**」をクリックします。
1. クラスターを表示するには、「**顧客情報**」を選択します。

   クラスターは、「**基本情報**」セクションの右上隅近くに表示されます。

   ![](assets/locate-cluster.png)

1. Workfront プランを表示するには、「**ライセンス**」を選択します。

   プランがページの下部近くに表示されます。

   ![](assets/locate-plan.png)
