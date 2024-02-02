---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals の目標ステータスの概要
description: 目標ステータスは、目標がアクティブで現在の進行状況を記録しているか、非アクティブ、ドラフトまたは達成済みかを示します。
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: ht
source-wordcount: '825'
ht-degree: 100%

---

# Adobe Workfront Goals の目標ステータスの概要

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
>この記事で説明している機能を使用するには、組織に以下が必要です。
>
>* Pro 以上の [Adobe Workfront プラン](https://www.workfront.com/plans)。
>* Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。
>
>Workfront Goals ライセンスについては、Workfront のアカウントマネージャーにお問い合わせください。

Workfront Goals へのアクセス権について詳しくは、[Workfront Goals の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md)を参照してください。


目標ステータスは、目標がアクティブで現在の進行状況を記録しているか、非アクティブ、ドラフトまたは達成済みかを示します。

## Workfront Goals の目標ステータスを更新する際の考慮事項

* 自分が作成した目標や、自分に共有された目標のステータスを手動で更新することはできません。目標のステータスは、目標に対して実行したアクションに応じて更新されます。例えば、目標をアクティブ化すると、「ドラフト」のステータスが「アクティブ」に変わります。
* いくつか制限が存在し、次のルールに従って目標のステータスを別のステータスに変更できない場合があります。

  | 変更元／変更先 | ドラフト | アクティブ | 非アクティブ | クローズ |
  |---|---|---|---|---|
  | ドラフト | - | はい | いいえ | いいえ |
  | アクティブ | いいえ | - | はい | はい |
  | 非アクティブ | いいえ | はい | - | いいえ |
  | クローズ | いいえ | はい | いいえ | - |

* クローズした目標を開くと、目標の進行状況も更新されます。
* 目標に対して実行する特定のアクションのステータスも更新されます。目標ステータスを更新する方法について詳しくは、次の記事を参照してください。

   * [Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)
   * [Adobe Workfront Goals での目標のアクティブ化](../../workfront-goals/goal-management/activate-goals.md)
   * [Adobe Workfront Goals での目標の削除と非アクティブ化](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Adobe Workfront Goals での目標のクローズと再オープン](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront Goals の目標ステータスの概要

Workfront Goals の目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

目標のアクティブ化については、[Adobe Workfront Goals での目標のアクティブ化](../../workfront-goals/goal-management/activate-goals.md)を参照してください。

Workfront Goals では、目標は次のいずれかのステータスを持つことができます。

* [ドラフト](#draft)
* [アクティブ](#active)
* [非アクティブ](#inactive)
* [クローズ](#closed)

### ドラフト {#draft}

* これは、新しく作成された目標のデフォルトのステータスです。目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。
* Workfront Goals は、ドラフトの目標に関する進捗を記録しません。
* ドラフトの目標の進捗状況を更新することはできません。
* ドラフトの目標に進捗情報がないため、ドラフトの目標を閉じたり非アクティブ化したりすることはできません。
* ドラフトの目標は、他の目標の進捗計算には影響せず、グラフでは考慮されません。
* ドラフトの目標は、Workfront Goals の以下のエリアに表示されます。

   * 目標リスト
   * 「目標の整合性」セクション（調整された目標としてのみ）


>[!IMPORTANT]
>
>目標のステータスをドラフトから他のステータスに変更した後は、目標を「ドラフト」のステータスに戻すことはできません。

### アクティブ {#active}

* ドラフトの目標は、結果やアクティビティに関連付けたり、別の目標関連付けることで初めてアクティブ化できます。目標をアクティブ化すると、そのステータスが「アクティブ」に変わります。目標のアクティブ化について詳しいは、[Adobe Workfront Goals での目標のアクティブ化](../../workfront-goals/goal-management/activate-goals.md)を参照してください。
* Workfront Goals は、アクティブな目標の進捗を記録します。
* アクティブな目標は、他の目標の進捗状況の計算に影響し、グラフで考慮されます。
* アクティブな目標は、Workfront Goals の以下のエリアに表示されます。

   * 目標リスト
   * 「目標の整合性」セクション
   * アクティブな目標の進捗状況のグラフ表示

* クローズした目標または非アクティブな目標を再アクティブ化できます。

### 非アクティブ {#inactive}

* 所有者が一時的または恒久的に作業を停止した場合、アクティブな目標を非アクティブ化できます。それを履歴情報に保存できます。これにより、目標のステータスが非アクティブに更新されます。

  目標の非アクティブ化について詳しくは、[Adobe Workfront Goals での目標の削除および非アクティブ化](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)の記事の「目標を非アクティブ化」セクションを参照してください。

* ドラフトまたはクローズした目標は非アクティブ化できません。
* 非アクティブな目標を再アクティブ化して、引き続き作業を行うことができます。
* Workfront Goals は、非アクティブな目標の進捗を計算しません。
* 非アクティブな目標の進行状況は更新できません。
* 非アクティブな目標は、他の目標の進捗状況の計算には影響せず、グラフでは考慮されません。
* 非アクティブな目標は、下書きの目標とは異なり、一度はアクティブだったことがあるので、進捗履歴があります。
* 非アクティブな目標は、Workfront Goals の次のエリアに表示されます。

   * 目標リスト
   * 「目標の整合性」セクション（調整された目標としてのみ）

### クローズ {#closed}

* 目標を達成した、目標に取り組んでいない、または将来その目標に取り組むことがない場合は、目標をクローズすることができます。目標のクローズについて詳しくは、[Adobe Workfront Goals での目標のクローズおよび再オープン](../../workfront-goals/goal-management/close-and-reopen-goals.md)を参照してください。

  >[!TIP]
  >
  >未達成の目標に後で取り組む予定がある場合は、ステータスを「クローズ」ではなく「非アクティブ」に変更することをお勧めします。

* ドラフトの目標のように、アクティブ化していない目標をクローズすることはできません。
* クローズした目標を再オープンして、その目標の作業を続行することができます。
* Workfront Goals では、クローズした目標の進捗の記録は停止します。
* クローズした目標の進捗状況を更新することはできません。
* クローズした目標は、Workfront Goals の以下のエリアに表示されます。

   * 目標リスト
   * 「目標の整合性」セクション（調整された目標としてのみ）
   * クローズした目標の情報は、「グラフ」セクションでも考慮されます。
