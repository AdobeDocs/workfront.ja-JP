---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: でのロックされたシナリオの管理 [!DNL Adobe Workfront Fusion]
description: でのロックされたシナリオの管理 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 014434dc-7548-42d1-bacd-89ddf627b647
source-git-commit: 9050684504f2335f5631f63978a9f65c25fd8d5f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# でのロックされたシナリオの管理 [!DNL Adobe Workfront Fusion]

場合によっては、シナリオが一時的にロックされることがあります [!DNL Workfront Fusion]. ロックされた実行は、2 ～ 4 時間以内に自動的にロック解除されます。 シナリオのロックを手動で解除することもできます。

>[!IMPORTANT]
>
>シナリオを手動でロック解除すると、シナリオの実行でエラーが発生する場合があります。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA) </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## ロックされたシナリオについて

シナリオは、様々な理由でロックされる場合があります。

Workfront Fusion は、スケジュールされたシナリオの並列処理をサポートしていません。 これらのシナリオは、シナリオの実行の開始時にロックされ、完了時にロックが解除されます。 実行が中断された場合、シナリオはロックを解除できない可能性があります。 これは、ユーザーが手動でシナリオを強制的に停止した場合や、システムの問題が発生した場合に発生する可能性があります。

また、Workfront Fusion のエンジニアリングチームは、パフォーマンスやその他の問題を引き起こしているので、シナリオをロックする場合があります。

ロックされたシナリオの原因に関係なく、ロックされた後、シナリオは自動的に 2～4 時間でロック解除されます。

## ロックされたシナリオのロック解除

ロックされたシナリオは、ロックされた時点から 2 ～ 4 時間ロック解除されます。 シナリオのロックを手動で解除してから、自動的にロックを解除するようスケジュールを設定できます。

シナリオを手動でロック解除すると、シナリオの実行でエラーが発生する場合があります。 シナリオの設計の一環として実行の実行と停止が原因でシナリオがロックされている場合にのみ、シナリオを手動でロック解除することをお勧めします。 その他の状況では、シナリオのロックが自動的に解除されるのを待つことをお勧めします。

>[!IMPORTANT]
>
>シナリオを手動でロック解除すると、シナリオの実行でエラーが発生する場合があります。

1. ロックされたシナリオのシナリオの詳細ページに移動します。
1. クリック **[!UICONTROL オプション]** をクリックします。
1. 選択 **[!UICONTROL 実行のロックを解除]**.
1. クリック **[!UICONTROL ロック解除]**.
