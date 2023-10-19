---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: ファイアウォールの設定を許可リストに加える行う
description: ファイアウォールまたはメールサーバーが特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをそのに追加する必要があ許可リストに加えるります。 これにより、環境とAdobe Workfrontサーバー間の通信が開き、ユーザーはWorkfrontからメッセージを送信し、Active Directory または LDAP で SSO を使用できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: ed5f941690754f631c16c5206faeeeb30d126841
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 13%

---

# ファイアウォールの設定を許可リストに加える行う

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>組織がAdobe Admin Consoleにオ許可リストに加えるンボーディングされている場合のを設定するには、 [ドメインのアプリおよびAdobeサービスで許可するドメイン](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>組織が組織を設定する方法は、許可リストに加える各組織に固有です。 IT チームと協力して、組織の手順を特定し、これらの追加を実装します。

ファイアウォールまたはメールサーバーが特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをそのに追加する必要があ許可リストに加えるります。 これにより、環境とAdobe Workfrontサーバー間の通信が開始され、次のプロセスが可能になります。

* Workfrontアプリケーションからのメッセージの送信

  >[!NOTE]
  >
  >組織のWorkfrontインスタンスで「Adobe IMS」が有効になっている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

* カスタムドキュメント統合を設定する際のドキュメント Web フックの使用
* Workfront Event Subscriptions の使用

  詳しくは、 [イベント購読 API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

また、E メールメッセージが配信されたときに暗号化されるように、特定のポートを開く必要があります。

## Workfront 許可リストに加える

組織が Enterprise プランを保有している場合は、次の 2 つのWorkfront設定も設定でき許可リストに加えるます。

* **電子メールの許可リストに加える**：ユーザーがWorkfrontのどこにデータを電子メールで送信できるかを制御できます。 詳しくは、 [電子メールの設定を行いま許可リストに加えるす。](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP の許可リストに加える**:Workfrontへのアクセスを 45 個の IP アドレスまたは IP アドレス範囲に制限し、Workfrontアプリケーションのセキュリティ層をさらに 1 層提供します。 詳しくは、 [IP アドレスでAdobe Workfrontへのアクセスを制限する](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Workfrontクラスターの場所

ファイアウォール上のに追加する必要がある IP アド許可リストに加えるレスは、実稼動環境が実行されるクラスターによって異なります。

組織のクラスターを検索するには、次の手順に従います。

1. Workfront管理者が、 **メインメニュー** アイコン ![メインメニュー](assets/main-menu-icon.png)を選択し、次に **設定**.
1. 左側のナビゲーションで、 **システム**&#x200B;を選択し、「 **顧客情報**.
1. 次を見つけます。 **クラスターの設定** フィールドを使用して、ページの右上隅に表示されます。 組織のクラスターがここに表示されます。

   CL01 はクラスタ 1 を表し、CL02 はクラスタ 2 を表します。

詳しくは、 [組織のクラスターとWorkfrontプランを表示](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) 記事内 [ファイアウォールの概要](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## に追加する IP アド許可リストに加えるレス

>[!IMPORTANT]
>
>一部のWorkfront統合は、静的 IP アドレ許可リストに加えるスで設定できないので、この統合が有効な場合は機能しません。 次の統合を使用するには、「 」オプションを無効にする必要があり許可リストに加えるます。
>
>* Workfront for G Suite
>* Workfront for Outlook
>* Workfront for Salesforce

* [クラスタ 1、2、3、5、7、8、9 に対して許可する IP アドレス](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [クラスタ 4 に許可する IP アドレス](#ip-addresses-to-allow-for-cluster-4)
* [クラスタ 6 に許可する IP アドレス](#ip-addresses-to-allow-for-cluster-6)
* [テストドライブに使用する IP アドレス](#IP%20Addre2)
* [イベント購読の実装時に許可する IP アドレス](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [拡張認証を可能にする IP アドレス](#ip-addresses-to-allow-for-enhanced-authentication)
* [Workfront Fusion にアクセスするために追加する IP アドレス](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Jira でのWorkfrontの使用に追加する IP アドレス](#ip-addresses-to-add-for-using-workfront-for-jira)
* [Workfront Ascent を使用するために追加する IP アドレス](#ip-addresses-to-add-for-using-workfront-ascent)
* [すべてのクラスターWorkfrontに追加する URL](#urls-to-add-for-all-clusters-workfront)

### クラスタ 1、2、3、5、7、8、9 に対して許可する IP アドレス {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

実稼動環境がクラスタ 1、2、3、5、または 7 上にある場合は、次の IP アドレスを許可する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">SSO、ドキュメントの Web フック、またはその他の機能</td> 
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
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfrontアプリケーションから電子メールを受信するには</td> 
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
    </ul> <p>次の IP アドレスについて詳しくは、 <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md" class="MCXref xref">21.1 リリースでのAdobe Workfront E メールの新しい IP アドレス</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### クラスタ 4 に許可する IP アドレス {#ip-addresses-to-allow-for-cluster-4}

実稼動環境がクラスター 4 上にある場合、SSO、ドキュメント Webhook 統合用に次の IP アドレスを追加し、Workfrontアプリケーションから E メールを受信します。

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

次の IP アドレスについて詳しくは、 [21.1 リリースでのAdobe Workfront E メールの新しい IP アドレス](../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md)

* 23.251.239.98
* 23.251.239.99

### クラスタ 6 に許可する IP アドレス {#ip-addresses-to-allow-for-cluster-6}

実稼動環境がクラスター 6 上にある場合は、次の IP アドレスを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfrontアプリケーションから電子メールを受信するには</td> 
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
   <td role="rowheader">AWS E メールサービスを使用するには</td> 
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
 </tbody> 
</table>

### テストドライブに使用する IP アドレス

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">テストドライブを使用する際にWorkfrontアプリケーションから電子メールを受け取るには</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Test Drive を使用する際の SSO およびドキュメント Webhook 統合の場合</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>ユーザーがWorkfrontから電子メールを受信するに許可リストに加えるは、このアドレスをに追加する必要もあります。</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### イベント購読の実装時に許可する IP アドレス  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

すべての環境で、Workfrontイベント購読からペイロードを受け取るには、次の IP アドレスを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> ヨーロッパのお客様向け</td> 
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
   <td role="rowheader">ヨーロッパ以外の場所の顧客</td> 
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

### 拡張認証を可能にする IP アドレス {#ip-addresses-to-allow-for-enhanced-authentication}

プレビューまたは実稼動用の拡張認証を使用するには、次の IP アドレスを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">環境がクラスタ 1、2、3、5、7、8、9 の場合</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">環境がクラスター 4 上にある場合</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Workfront Fusion にアクセスするために追加する IP アドレス  {#ip-addresses-to-add-for-accessing-workfront-fusion}

次の IP アドレスをに追加し許可リストに加えるて、Workfront Fusion がシステムにアクセスできるようにします。

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
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

また、組織がアウトバウンドネットワークフィルタリングを使用している場合は、次のドメインをに追加し許可リストに加えるて、システムがWorkfront Fusion にアクセスできるようにします。

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
 </tbody> 
</table>

>[!NOTE]
>
>アウトバウンドネットワークフィルタリングはまれです。 ネットワーク管理者に問い合わせて、それに対応するためにネットワークを更新する必要があ許可リストに加えるるかどうかを確認してください。

### Jira でのWorkfrontの使用に追加する IP アドレス {#ip-addresses-to-add-for-using-workfront-for-jira}

Workfront for Jira 統合を使用するに許可リストに加えるは、次の IP アドレスをに追加します。

また、 jira.workfront.comドメインは、会社のサーバーからアクセスできる必要があります。 このドメインは、Workfrontと Jira の間のミドルウェアとして機能するので、必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> ヨーロッパのお客様向け</td> 
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
   <td role="rowheader">ヨーロッパ以外の場所の顧客</td> 
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

### Workfront Ascent を使用するために追加する IP アドレス {#ip-addresses-to-add-for-using-workfront-ascent}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront Ascent を使用してWorkfrontのトレーニングリソースにアクセスするには</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Ascent から電子メール通知を受け取るには</td> 
   <td> 
    <ul> 
     <li>23.251.227.75</li> 
     <li>23.251.227.76</li> 
     <li>23.251.227.77</li> 
     <li>23.251.227.78</li> 
     <li>23.251.227.79</li> 
     <li>23.251.227.80</li> 
     <li>23.251.227.81</li> 
     <li>23.251.227.82</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfrontにアクセスするために追加するドメイン

組織でアウトバウンドネットワークフィルタリングを使用している場合、次のドメインをに追加し許可リストに加えるて、システムがWorkfrontにアクセスできるようにします。

>[!NOTE]
>
>アウトバウンドネットワークフィルタリングはまれです。 ネットワーク管理者に問い合わせて、それに対応するためにネットワークを更新する必要があ許可リストに加えるるかどうかを確認してください。

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## すべてのクラスターWorkfrontに追加する URL {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ヘルプコンテンツをWorkfront環境に表示できるようにするには</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof が任意のクラスター上のWorkfrontにアクセスできるようにするには、これらをすべての環境に追加します</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Workfrontで配達確認を表示するために必要</li> 
     <li>*.proofhq.com - Workfront Proof で配達確認を表示する場合に必要です</li> 
     <li>*.proofhq.eu - Workfrontの配達確認で配達確認を表示するために必要</li> 
    </ul> <p><b>メモ</b>:  <p>Workfront配達確認用にへの IP アドレスの追加はサ許可リストに加えるポートされていません。 これらは、WorkfrontがAWSに移行した後、動的になりました。 代わりに、Workfront Proof ドメインのみを許可することをお勧めします。</p> <p>これらのドメインの追加に問題があり、代わりに IP アドレスが必要許可リストに加えるな場合は、Workfrontカスタマーサポートにお問い合わせください。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Proof にアクセスするために追加する IP アドレスと URL

様々な機能を使用するには、次の IP アドレ許可リストに加えるスをに追加する必要があります。

* [コールバックおよび Web キャプチャの配達確認の場合](#for-callbacks-and-webcapture-proofs)
* [送信メールの場合](#for-outgoing-email)

### コールバックおよび Web キャプチャの配達確認の場合 {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US(Clusters 1、2、3、5、7)</td> 
   <td> 
    <ul> 
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
   <td role="rowheader">Prod-EU（クラスタ 4）</td> 
   <td> 
    <ul> 
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
    </ul> <p><b>注意</b>:DNS サーバーオプションはサポートされなくなりました。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 送信メールの場合 {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US(Clusters 1、2、3、5、7)</p> </td> 
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
   <td role="rowheader">Prod-EU（クラスタ 4）</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 最高のWorkfront Proof パフォーマンスを得るために開くポート

配達確認の読み込みで問題が発生した場合や、Workfront Proof で動作しない場合は、次のポートを開きます。

* 5671
* 5672
* 15671

## 暗号化された E メール用に開くポート

Workfrontアプリケーションからの E メールは、ポート 465 および 587 を使用して暗号化されて送信されます。 メールサーバーが暗号化された電子メールをサポートしていない場合、電子メールはポート 25 を使用して暗号化されずに配信されます。

## Workfront Support からの電子メール通知

Workfrontサポートからのメールを受け取っていない場合は、必要な Salesforce IP アドレスとドメインを必ず追加してください。 詳細は、Salesforce のヘルプ記事で許可する Salesforce IP アドレスとドメインに関する記事を参照してください。
