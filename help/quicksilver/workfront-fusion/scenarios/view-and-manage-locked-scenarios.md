---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] でのロックされたシナリオの管理'
description: ' [!DNL Adobe Workfront Fusion] でのロックされたシナリオの管理'
author: Becky
feature: Workfront Fusion
exl-id: 014434dc-7548-42d1-bacd-89ddf627b647
source-git-commit: 9050684504f2335f5631f63978a9f65c25fd8d5f
workflow-type: ht
source-wordcount: '333'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのロックされたシナリオの管理 

場合によっては、[!DNL Workfront Fusion] でシナリオが一時的にロックされることがあります。ロックされた実行は、2～4 時間以内に自動的にロック解除されます。シナリオのロックを手動で解除することもできます。

>[!IMPORTANT]
>
>シナリオを手動でロック解除すると、シナリオの実行でエラーが発生する場合があります。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## ロックされたシナリオについて

シナリオは、様々な理由でロックされる場合があります。

Workfront Fusion では、スケジュールされたシナリオの並列処理をサポートしていません。これらのシナリオは、シナリオ実行の開始時にロックされ、完了時にロックが解除されます。実行が中断された場合は、シナリオのロックが解除されない可能性があります。これは、ユーザーが手動で強制的にシナリオを停止した場合や、システムの問題が発生した場合に起こる可能性があります。

また、Workfront Fusion でパフォーマンスなどの問題が発生しているので、エンジニアリングチームがシナリオをロックする場合があります。

ロックされたシナリオの原因に関係なく、シナリオはロックされた後 2～4 時間で自動的にロック解除されます。

## ロックされたシナリオのロックを解除

ロックされたシナリオは、ロックされた時点から 2～4 時間後にロック解除されます。シナリオの自動ロック解除がスケジュールされている時点より前に、手動でロック解除することもできます。

シナリオを手動でロック解除すると、シナリオの実行でエラーが発生する場合があります。シナリオの設計の一環として、シナリオを手動でロック解除するのは、実行の開始と停止が原因でシナリオがロックされる場合に限ることをお勧めします。その他の状況では、シナリオのロックが自動的に解除されるのを待つことをお勧めします。

>[!IMPORTANT]
>
>シナリオを手動でロック解除すると、シナリオの実行でエラーが発生する場合があります。

1. ロックされたシナリオのシナリオの詳細ページに移動します。
1. 画面の右上隅にある「**[!UICONTROL オプション]**」をクリックします。
1. 「**[!UICONTROL 実行のロックを解除]**」を選択します。
1. 「**[!UICONTROL ロックを解除]**」をクリックします。
