---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion アクセス用の IP アドレス
description: Adobe Workfront Fusion を使用するには、Adobe Workfront ライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 800cf889ff2729fca0c9d75d0ace0ecc1ee53a79
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 55%

---

# [!DNL Adobe Workfront Fusion] にアクセスするための IP アドレス

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] には、[!DNL Adobe Workfront license] に加えて [!DNL Adobe Workfront Fusion] ライセンスが必要です。

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合には、環境と [!DNL Adobe Workfront Fusion] の間でオープンな通信を許可するために、特定の IP アドレスを許可リストに追加する必要があります。

すべての Fusion IP アドレスとドメインを許可リストに追加することも、Fusion クラスターを見つけて、そのクラスターの IP アドレスとドメインのみを追加することもできます。

## すべての Fusion IP アドレスとドメインの追加

次の IP アドレスを許可リストに追加します。

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

また、組織でアウトバウンドネットワークフィルタリングを使用している場合は、次のドメインを許可リストに追加して、システムからWorkfront Fusion にアクセスできるようにします。 これらは Webhook に使用されます。

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## クラスターにのみ Fusion の IP アドレスとドメインを追加

### データセンターの特定

IP アドレスは、データが格納されている場所によって異なります。

URL を使用して Fusion にアクセスすると、URL を調べてデータセンターを見つけることができます。

| URL | データセンター |
| --- | --- |
| `https://app.workfrontfusion.com/` | US データセンター |
| `https://app-eu.workfrontfusion.com/` | EU データセンター |
| `https://app-az.workfrontfusion.com/` | Azure データセンター |

experience.adobe.comから Fusion にアクセスする場合は、ブラウザーの「ネットワーク」タブを確認して、データセンターを特定できます。

| URL | データセンター |
| --- | --- |
| `https://fusion.adobe.com` への呼び出し | US データセンター |
| `https://eu.fusion.adobe.com` への呼び出し | EU データセンター |
| `https://az.fusion.adobe.com` への呼び出し | Azure データセンター |

### データセンターの IP アドレスとドメインの追加

以下の IP アドレスを許可リストに追加して、[!DNL Workfront Fusion] がシステムにアクセスできるようにします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
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

また、組織がアウトバウンドネットワークフィルタリングを使用している場合は、次のドメインを許可リストに追加して、システムが Workfront Fusion にアクセスできるようにします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
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

組織の許可リストの設定について詳しくは、[ファイアウォールの許可リストを設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。
