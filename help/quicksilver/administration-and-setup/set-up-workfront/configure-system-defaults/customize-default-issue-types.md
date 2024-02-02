---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: デフォルトのイシュータイプをカスタマイズ
description: デフォルトのイシュータイプごとにラベルをカスタマイズして、組織で使用される用語に合わせることができます。イシュータイプは、イシューステータスのカスタマイズやリクエストキューの作成に役立ちます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: ht
source-wordcount: '451'
ht-degree: 100%

---

# デフォルトのイシュータイプをカスタマイズ

イシュータイプは、次の状況で役立ちます。

* イシューステータスをカスタマイズする場合（[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照）
* リクエストキューを作成する場合（[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照）

デフォルトのイシュータイプごとにラベルをカスタマイズして、組織で使用される用語に合わせることができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## デフォルトのイシュータイプ

[!DNL Adobe Workfront] [!UICONTROL 管理者]アクセス権を持つ場合、4 つのデフォルトのイシュータイプを設定して名前変更できます。

* **[!UICONTROL バグレポート]**：システムで報告されたバグをトラックするために使用されます。
* **[!UICONTROL 変更依頼]**：更新または修正が必要な問題をトラックするために使用します。
* **[!UICONTROL イシュー]**：計画外の作業、発生した問題、またはタスクを続行するために解決する必要があるものを伝達する [!DNL Workfront] 内のオブジェクト。
* **[!UICONTROL リクエスト]**： Workfront でユーザーがリクエストを行うリクエストキューに適用されるイシュータイプ。

![](assets/default-issue-types.png)

## イシュータイプのカスタマイズ

イシュータイプのカスタマイズについて、次の点を考慮してください。

* イシュータイプのラベルは変更できますが、関数は変更できません。
* これ以上のイシュータイプは作成できません。
* イシュータイプの名前に対してフィルター値を変更することはできません。したがって、イシューレポートでフィルターを作成した場合、フィルター（キー）の値はイシュータイプのカスタム名を反映しません。
* 各イシュータイプには、3 つのデフォルトのステータス（[!UICONTROL 新規]、[!UICONTROL 処理中]、[!UICONTROL 閉じる]）が関連付けられています。これらのステータスは、イシュータイプから削除することはできませんが、名前を変更することはできます。
* 各イシュータイプのドロップダウンメニューに表示されるオプションの順序を変更できます。

イシュータイプをカスタマイズするには：

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. **[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL ステータス]**&#x200B;をクリックします。

1. 「**[!UICONTROL イシュー]**」タブを選択します。
1. 次のいずれかの操作を行います。

   * カスタマイズするイシュータイプにポインタを合わせて、[!UICONTROL 編集]アイコン ![](assets/edit-icon.png) が右端に表示されたら、イシュータイプの新しい名前を入力します。

     ![](assets/customize-issue-type.png)

   * [!UICONTROL イシューの種類]をクリックして関連するステータスをリストし、ポインタを合わせると表示されるハンドルをドラッグし、ユーザーのイシュー&#x200B;**[!UICONTROL ステータス]**&#x200B;ドロップダウンメニューに表示する順序でドロップします。
