---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目標の目標ステータスの概要
description: 目標ステータスは、目標がアクティブで進行状況を記録しているか、非アクティブ、下書き、または既に達成済みかを示します。
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Adobe Workfront目標の目標ステータスの概要

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>この記事で説明する機能を使用するには、以下が必要です。
>
>* プロ以上 [Adobe Workfrontプラン](https://www.workfront.com/plans).
>* Workfrontライセンスに加えて、Adobe Workfront Goals ライセンスが必要です。
>
>Workfront Goals ライセンスについて詳しくは、Workfrontのアカウントマネージャーにお問い合わせください。

Workfront Goals へのアクセスについて詳しくは、 [Workfront目標の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


目標ステータスは、目標がアクティブで進行状況を記録しているか、非アクティブ、下書き、または既に達成済みかを示します。

## Workfront目標の目標ステータスを更新する際の考慮事項

* 自分が作成した目標や自分が共有していた目標のステータスを手動で更新することはできません。 目標のステータスは、目標に対して実行したアクションに応じて更新されます。 例えば、目標をアクティブ化すると、ドラフトステータスがアクティブに変わります。
* 一部の制限が存在し、次のルールに従って目標のステータスを別のステータスに変更できない場合があります。

   | 開始/終了 | 下書き | アクティブ | 非アクティブ | クローズ |
   |---|---|---|---|---|
   | 下書き | - | はい | いいえ | いいえ |
   | アクティブ | いいえ | - | はい | はい |
   | 非アクティブ | いいえ | はい | - | いいえ |
   | クローズ | いいえ | はい | いいえ | - |

* クローズした目標を開くと、目標の進行状況も更新されます。
* 目標に対して実行する特定のアクションのステータスも更新されます。 目標ステータスを更新する方法については、次の記事を参照してください。

   * [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md)
   * [Adobe Workfront目標で目標を有効化](../../workfront-goals/goal-management/activate-goals.md)
   * [Adobe Workfront目標の目標の削除と無効化](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Adobe Workfront目標の目標を閉じて再度開く](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront目標の目標ステータスの概要

Workfront目標の作成について詳しくは、 [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md).

目標のアクティブ化について詳しくは、 [Adobe Workfront目標で目標を有効化](../../workfront-goals/goal-management/activate-goals.md).

目標は、Workfront目標に次のいずれかのステータスを持つことができます。

* [下書き](#draft)
* [アクティブ](#active)
* [非アクティブ](#inactive)
* [クローズ](#closed)

### 下書き {#draft}

* これは、新しく作成された目標のデフォルトのステータスです。 目標の作成について詳しくは、 [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md).
* Workfront目標は、下書き目標に関する進捗を記録しません。
* 下書きの目標の進捗状況を更新することはできません。
* 下書き目標に進捗情報がないため、下書き目標を閉じたり非アクティブにしたりすることはできません。
* 下書きの目標は、他の目標の進捗計算には影響せず、グラフでは考慮されません。
* 下書きの目標は、Workfront目標の以下の領域に表示されます。

   * 目標リスト
   * [ 目標の位置合わせ ] セクション（位置合わせされた目標としてのみ）


>[!IMPORTANT]
>
>目標のステータスを他のステータスに変更した後は、目標をドラフトステータスにすることはできません。

### アクティブ {#active}

* 下書き目標は、結果、アクティビティに関連付ける場合、または目標に別の目標を整列する場合にのみ有効化できます。 目標をアクティブ化すると、そのステータスが「アクティブ」に変わります。 目標のアクティブ化について詳しくは、 [Adobe Workfront目標で目標を有効化](../../workfront-goals/goal-management/activate-goals.md).
* Workfront目標は、アクティブな目標の進捗を記録します。
* アクティブな目標は、他の目標の進捗状況の計算に役立ち、グラフで考慮されます。
* アクティブな目標は、Workfront目標の次の領域に表示されます。

   * 目標リスト
   * [ 目標の位置合わせ ] セクション
   * アクティブな目標の進行状況がグラフに表示されます

* クローズ済みまたは非アクティブな目標を再アクティブ化できます。

### 非アクティブ {#inactive}

* 所有者が一時的または恒久的に作業を停止した場合に、アクティブな目標を非アクティブ化できます。 履歴情報用に保存できます。 これにより、目標のステータスが非アクティブに更新されます。

   目標の無効化について詳しくは、この記事の「目標の無効化」の節を参照してください。 [Adobe Workfront目標の目標の削除と無効化](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* 下書きまたは終了した目標は無効にできません。
* 非アクティブな目標を再アクティブ化して、引き続き作業を行うことができます。
* Workfront目標は、非アクティブな目標の進捗を計算しません。
* 非アクティブな目標の進行状況は更新できません。
* 非アクティブな目標は、他の目標の進捗状況の計算には影響せず、グラフでは考慮されません。
* 非アクティブな目標は、下書きの目標とは異なり、かつてアクティブだったので、進捗履歴があります。
* 非アクティブな目標は、Workfront目標の次の領域に表示されます。

   * 目標リスト
   * 「目標の整列」セクション（整列された目標としてのみ）

### クローズ {#closed}

* 目標を達成したこと、または今後その目標に取り組んでいないこと、または将来その目標に取り組まないことを示す場合は、目標をクローズできます。 終了目標について詳しくは、 [Adobe Workfront目標の目標を閉じて再度開く](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >まだ達成していない目標を後から作業する予定がある場合は、ステータスを「クローズ」ではなく「非アクティブ」に変更することをお勧めします。

* 下書き目標のように、有効化されていない目標を閉じることはできません。
* 閉じた目標を再度開き、その目標に関する作業を続行できます。
* Workfront目標は、終了した目標の進捗の記録を停止します。
* 終了した目標の進捗状況を更新することはできません。
* 閉じた目標は、Workfront目標の次の領域に表示されます。

   * 目標リスト
   * 「目標の整列」セクション（整列された目標としてのみ）
   * 閉じた目標の情報は、グラフセクションでも考慮されます。
