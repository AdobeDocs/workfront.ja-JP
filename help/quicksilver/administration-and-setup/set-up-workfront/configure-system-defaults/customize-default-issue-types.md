---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: デフォルトのイシュータイプのカスタマイズ
description: デフォルトのイシュータイプごとにラベルをカスタマイズして、組織で使用される用語に合わせることができます。イシュータイプは、イシューステータスのカスタマイズやリクエストキューの作成に役立ちます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 87%

---

# デフォルトのイシュータイプをカスタマイズ

イシュータイプは、次の状況で役立ちます。

* イシューステータスをカスタマイズする場合（[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照）
* リクエストキューを作成する場合（[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照）

デフォルトのイシュータイプごとにラベルをカスタマイズして、組織で使用される用語に合わせることができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## デフォルトのイシュータイプ

[!DNL Adobe Workfront] [!UICONTROL 管理者]アクセス権を持つ場合、4 つのデフォルトのイシュータイプを設定して名前変更できます。

* **[!UICONTROL バグレポート]**：システムで報告されたバグをトラックするために使用されます。
* **[!UICONTROL 変更依頼]**：更新または修正が必要な問題をトラックするために使用します。
* **[!UICONTROL イシュー]**：計画外の作業、発生した問題、またはタスクを続行するために解決する必要があるものを伝達する [!DNL Workfront] 内のオブジェクト。
* **[!UICONTROL リクエスト]**： Workfront でユーザーがリクエストを行うリクエストキューに適用されるイシュータイプ。

![&#x200B; デフォルトのイシュータイプ &#x200B;](assets/default-issue-types.png)

## イシュータイプのカスタマイズ

イシュータイプのカスタマイズについて、次の点を考慮してください。

* イシュータイプのラベルは変更できますが、関数は変更できません。
* これ以上のイシュータイプは作成できません。
* イシュータイプの名前に対してフィルター値を変更することはできません。したがって、イシューレポートでフィルターを作成した場合、フィルター（キー）の値はイシュータイプのカスタム名を反映しません。
* 各イシュータイプには、3 つのデフォルトのステータス（[!UICONTROL 新規]、[!UICONTROL 処理中]、[!UICONTROL 閉じる]）が関連付けられています。これらのステータスは、イシュータイプから削除することはできませんが、名前を変更することはできます。
* 各イシュータイプのドロップダウンメニューに表示されるオプションの順序を変更できます。

イシュータイプをカスタマイズするには：

{{step-1-to-setup}}

1. **[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL ステータス]**&#x200B;をクリックします。

1. 「**[!UICONTROL イシュー]**」タブを選択します。
1. 次のいずれかの操作を行います。

   * カスタマイズするイシュータイプにポインタを合わせ、右端に表示される [!UICONTROL &#x200B; 編集 &#x200B;] アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックして、イシュータイプの新しい名前を入力します。

     ![&#x200B; イシュータイプのカスタマイズ &#x200B;](assets/customize-issue-type.png)

   * [!UICONTROL イシューの種類]をクリックして関連するステータスをリストし、ポインタを合わせると表示されるハンドルをドラッグし、ユーザーのイシュー&#x200B;**[!UICONTROL ステータス]**&#x200B;ドロップダウンメニューに表示する順序でドロップします。
