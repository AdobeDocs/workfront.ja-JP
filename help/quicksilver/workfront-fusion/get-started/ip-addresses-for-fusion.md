---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion にアクセスするための IP アドレス
description: Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: adb324323330f53108532cc7a7e68466fdb84273
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# アクセス用の IP アドレス [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] にはが必要です [!DNL Adobe Workfront Fusion] に加えてライセンス [!DNL Adobe Workfront license].

ファイアウォールまたはメールサーバーが特定のベンダーへのアクセスのみを許可するように設定されている場合、環境と [!DNL Adobe Workfront Fusion].

次の IP アドレスをに追加して有許可リストに加える効にします [!DNL Workfront Fusion] をクリックして、システムにアクセスします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU データセンター</td> 
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

また、組織がアウトバウンドネットワークフィルタリングを使用している場合は、次のドメインをに追加し許可リストに加えるて、システムがWorkfront Fusion にアクセスできるようにします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU データセンター</td> 
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
>アウトバウンドネットワークフィルタリングはまれです。 ネットワーク管理者に問い合わせて、それに対応するためにネットワークを更新する必要があ許可リストに加えるるかどうかを確認してください。

組織の設定について詳しくは、次を参照してく許可リストに加えるださい。 [ファイアウォールの設定を許可リストに加える行う](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
