---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: ファイアウォールの許可リスト
description: ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをその許可リストに追加する必要があります。これにより、環境と Adobe Workfront サーバー間の通信が開き、ユーザーは Workfront からメッセージを送信し、Active Directory または LDAP で SSO を使用することが可能になります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: ee4cf80bc69416e3224c895c1f04628432ce2f4c
workflow-type: tm+mt
source-wordcount: '1646'
ht-degree: 88%

---

# ファイアウォールの許可リストの設定

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>このページで説明する手順は、Admin Console にまだ登録されていない組織にのみ適用されます。組織が Adobe Admin Console に登録されている場合は、Adobe Admin Console でこのアクションを実行してください。
>
>組織が Adobe Admin Console にオンボーディングされている場合に許可リストを設定するには、[アドビアプリおよびサービスで許可するドメイン](https://helpx.adobe.com/jp/enterprise/kb/network-endpoints.html)を参照してください。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront／Adobe Business Platform）](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

>[!NOTE]
>
>組織が許可リストを設定する方法は、各組織に一意です。IT チームと協力して、組織の手順を特定し、これらの追加を実装してください。

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをその許可リストに追加する必要があります。これにより、環境と Adobe Workfront サーバー間の通信が開始され、次のプロセスが可能になります。

* Workfront アプリケーションからのメッセージの送信

  >[!NOTE]
  >
  >組織の Workfront インスタンスが Adobe IMS によって有効化されている場合は使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

* カスタムドキュメント統合を設定する際のドキュメント web フックの使用
* Workfront イベント登録の使用

  詳しくは、[Event Subscription API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680) を参照してください。

また、メールメッセージが配信されたときに暗号化されるように、特定のポートを開く必要があります。

## 使用可能な Workfront 許可リスト

組織がエンタープライズプランを保有している場合は、次の 2 つの Workfront 許可リストも設定できます。

* **メールの許可リスト**：ユーザーが Workfront に保存されているデータをどこにメールで送信できるかを制御できます。詳しくは、[メールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)を参照してください。
* **IP の許可リスト**：Workfront へのアクセスを指定した 75 個の IP アドレスまたは IP アドレス範囲に制限し、Workfront アプリケーションのセキュリティ層をさらに 1 層追加します。詳しくは、[IP アドレスで Adobe Workfront へのアクセスの制限](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)を参照してください。

## Workfront クラスターの場所を特定

ファイアウォール上で許可リストに追加する必要がある IP アドレスは、実稼働環境が実行されるクラスターによって異なります。

組織のクラスターを検索するには、次の手順に従います。

{{step-1-to-setup}}

1. 左側のナビゲーションで、**システム**&#x200B;をクリックし、次に&#x200B;**顧客情報**&#x200B;を選択します。
1. ページの右上隅の「**クラスターの設定**」フィールドの場所を特定します。組織のクラスターがここに一覧表示されます。

   CL01 はクラスター 1 を参照し、CL02 はクラスター 2 を、と続きます。

詳しくは、[ファイアウォールの概要](../../administration-and-setup/get-started-wf-administration/firewall-overview.md)の記事内の、「[組織のクラスターと Workfront プランの表示](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan)」の節を参照してください。

## 許可リストに追加する IP アドレス

>[!IMPORTANT]
>
>一部の Workfront 統合は、静的 IP アドレスで設定できないため、許可リストが有効な場合は機能しません。次の統合を使用するには、許可リストを無効にする必要があります。
>
>* Google WorkspaceのWorkfront
>* Workfront for Outlook
>* Workfront for Salesforce

* [クラスター 1、2、3、5、7、8、9 に対して許可する IP アドレス](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [クラスター 4 に許可する IP アドレス](#ip-addresses-to-allow-for-cluster-4)
* [クラスター 6 に許可する IP アドレス](#ip-addresses-to-allow-for-cluster-6)
* [クラスター 10 に許可する IP アドレス](#ip-addresses-to-allow-for-cluster-10)
* [体験版に許可する IP アドレス](#IP%20Addre2)
* [イベント登録の実装時に許可する IP アドレス](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Workfront Fusion にアクセスするために追加する IP アドレス](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Jira での Workfront を使用するため追加する IP アドレス](#ip-addresses-to-add-for-using-workfront-for-jira)
* [すべてのクラスターの Workfront に追加する URL](#urls-to-add-for-all-clusters-workfront)

### クラスター 1、2、3、5、7、8、9 に対して許可する IP アドレス {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

実稼動環境がクラスター 1、2、3、5、7、8、9 にある場合、次の IP アドレスを許可する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">SSO、ドキュメントの web フック、またはその他の機能</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront アプリケーションからのメールの受信</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>次の IP アドレスについて詳しくは、<a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">21.1 リリースでの Adobe Workfront メールの新規 IP アドレス</a>を参照してください。</p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### クラスター 4 に許可する IP アドレス {#ip-addresses-to-allow-for-cluster-4}

実稼動環境がクラスター 4 上にある場合、SSO、ドキュメント web フック統合用に次の IP アドレスを追加し、Workfront アプリケーションからメールを受信します。

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

次の IP アドレスについて詳しくは、[21.1 リリースでの Adobe Workfront メールの新規 IP アドレス](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)を参照してください。

* 23.251.239.98
* 23.251.239.99

### クラスター 6 に許可する IP アドレス {#ip-addresses-to-allow-for-cluster-6}

実稼動環境がクラスター 6 上にある場合は、次の IP アドレスを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront アプリケーションからのメールの受信</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">メールサービスを使用するには</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Mailgun メールサービスを使用するには</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### クラスター 10 に許可する IP アドレス

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

### 体験版に使用する IP アドレス

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">体験版を使用する際に Workfront アプリケーションからメールを受け取るには</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">体験版を使用する際の SSO およびドキュメント web フック統合の場合</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>ユーザーが Workfront からメールを受信するに許可リストに加えるは、このアドレスをに追加する必要もあります。</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### イベント登録の実装時に許可する IP アドレス  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

すべての環境で、Workfront イベント登録からペイロードを受け取るには、次の IP アドレスを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> ヨーロッパの顧客の場合</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ヨーロッパ以外の場所の顧客の場合</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Workfront Fusion にアクセスするために追加する IP アドレス  {#ip-addresses-to-add-for-accessing-workfront-fusion}

次の IP アドレスをに追加し許可リストに加えて、Workfront Fusion がシステムにアクセスできるようにします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Microsoft Azure クラスター上</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

また、組織でアウトバウンドネットワークフィルタリングを使用している場合は、次のドメインを許可リストに追加して、システムからWorkfront Fusion にアクセスできるようにします。 これらの URL は、Fusion の Webhook に使用されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] Microsoft Azure クラスター上</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>アウトバウンドネットワークフィルタリングはまれです。対応するために許可リストを更新する必要があるかどうかをネットワーク管理者に確認してください。

### Workfront for Jira を使用するために追加する IP アドレス {#ip-addresses-to-add-for-using-workfront-for-jira}

Workfront for Jira 統合を使用するためには、次の IP アドレスを許可リストに追加します。

また、jira.workfront.comドメインは、会社のサーバーからアクセスできる必要があります。このドメインは、Workfront と Jira の間のミドルウェアとして機能するので必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> ヨーロッパの顧客の場合</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ヨーロッパ以外の場所の顧客の場合</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront にアクセスするために追加するドメイン

組織がアウトバウンドネットワークフィルタリングを使用している場合は、許可リストに次のドメインを追加して、システムから Workfront にアクセスできるようにします。

>[!NOTE]
>
>アウトバウンドネットワークフィルタリングはまれです。対応するために許可リストを更新する必要があるかどうかをネットワーク管理者に確認してください。

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* *.aptrinsic.com
* *.static.workfront.com


  これは、次のすべてのドメインを組み込んだ静的ドメインです。 必要に応じて、個々のドメインを追加できます。

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

組織がAdobeの統合エクスペリエンス上にある場合は、次のドメインを使用します。 これらのドメインについては `*.adobe.com` で説明していますが、必要に応じて追加できます。

* &lt;your domain>.my.workfront.adobe.com
* &lt;your domain>.preview.workfront.adobe.com
* &lt;your domain>.sb01.workfront.adobe.com
* &lt;your domain>.sb02.workfront.adobe.com


Workfront Fusion の場合、次のドメインを追加します。

* Adobeの統合エクスペリエンス以外の組織の場合：
   * app.workfrontfusion.com （米国AWS）
   * app-eu.workfrontfusion.com （EU AWS）
   * app-az.workfrontfusion.com （米国 Azure）

* Adobeの統合エクスペリエンスの組織の場合
（これらのドメインについては `*.adobe.com` で説明していますが、必要に応じて追加できます。）

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## すべてのクラスターの Workfront に追加する URL {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ヘルプコンテンツを Workfront 環境に表示できるようにするには：</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof から任意のクラスター上の Workfront にアクセスできるようにするには：</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Workfront でプルーフを表示するために必要</li> 
     <li>*.proofhq.com - Workfront Proof でプルーフを表示するために必要</li> 
     <li>*.proofhq.eu - Workfront Proof でプルーフを表示するために必要</li> 
    </ul> <p><b>メモ</b>:  <p>Workfront Proof の許可リストに IP アドレスを追加することはサポートしていません。これらは、Workfront が AWS に移行した後、動的なアドレスになりました。代わりに、Workfront Proof ドメインのみを許可することをお勧めします。</p> <p>これらのドメインを許可リストに追加することに問題があり、代わりに IP アドレスが必要な場合は、Workfront カスタマーサポートにお問い合わせください。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Proof にアクセスするために追加する IP アドレスと URL

様々な機能を使用するには、次の IP アドレスを許可リストに追加する必要があります。

* [コールバックおよび web キャプチャプルーフの場合](#for-callbacks-and-webcapture-proofs)
* [送信メールの場合](#for-outgoing-email)

### コールバックおよび web キャプチャプルーフの場合 {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US（クラスター 1、2、3、5、7）</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU（クラスター 4）</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>メモ</b>：DNS サーバーオプションはサポートされなくなりました。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 送信メールの場合 {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US（クラスター 1、2、3、5、7）</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU（クラスター 4）</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 最高の Workfront Proof パフォーマンスを得るために開くポート

Workfront Proof でプルーフの読み込みや動作に問題が発生した場合は、次のポートを開きます。

* 5671
* 5672
* 15671

## 暗号化されたメール用に開くポート

Workfront アプリケーションからのメールは、ポート 465 および 587 を使用して暗号化されて送信されます。メールサーバーが暗号化されたメールをサポートしていない場合、メールはポート 25 を使用すると暗号化されずに配信されます。

## Workfront サポートからのメール通知

Workfront サポートからのメールを受け取っていない場合は、必要な Salesforce IP アドレスとドメインを必ず追加してください。詳しくは、許可する Salesforce IP アドレスとドメインに関する Salesforce のヘルプ記事を参照してください。
