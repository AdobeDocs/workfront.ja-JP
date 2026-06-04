---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: ユーザー名は既に使用されています
description: ユーザー名が既に使用されているというエラーが表示された場合は、次のヒントをご確認ください。
author: Becky
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
TQID: https://experienceleague.adobe.com/uGrOaZZzbE6CkodhE1TlCtW4rRJkfqljWGJbNSzxODc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 100%

---

# ユーザー名は既に使用されています

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>システム管理者</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 質問

新しいユーザーを作成すると、ユーザー名が既に使用されていることを示す [!UICONTROL Whoops] エラーが表示されます。 システム内にこのメールが他に存在することはありません。 これが表示されるのはなぜですか?

## ソリューション

これは、ユーザー名またはメールアドレスが現在の [!DNL Adobe Workfront] インスタンス内で一意ではないために発生する可能性があります。 ユーザーは、別のインスタンスで同じユーザー名またはメールアドレスを持つことができます。 例えば、ユーザー A は、[!DNL Workfront] アカウントに関連付けられたメールアドレス usera@company1.com および usera@company2.com を持つことができます。

>[!NOTE]
>
>プライマリ [!DNL Workfront] 管理者は、同じクラスター上の別の Workfront インスタンスに存在する場合、同じユーザー名またはメールアドレスを持つことはできません。
>
>インスタンスが異なるクラスター上にある場合、プライマリ管理者は同じユーザー名またはメールアドレスを持つことができます。 インスタンスが存在するクラスターは、[!UICONTROL 設定]／[!UICONTROL システム]／[!UICONTROL 顧客情報]で確認できます。

### ユーザー名がインスタンス内で一意であるかどうかを確認

ユーザー名とメールアドレスが現在の [!DNL Workfront] インスタンス内で一意であることを確認します。

{{step-1-to-users}}

1. ユーザーのリストで、**[!UICONTROL メール]**&#x200B;列を調べて、重複したメールがないことを確認します。
1. ユーザー名の列をビューに追加します。

   1. **[!UICONTROL ビュー]**&#x200B;ドロップダウンメニューで、「**[!UICONTROL ビューをカスタマイズ]**」をクリックします。
   1. 「**[!UICONTROL 列を追加]**」をクリックします。
   1. 検索フィールドに&#x200B;*[!UICONTROL ユーザー名]*&#x200B;と入力します。
   1. **[!UICONTROL ユーザー]**／**[!UICONTROL ユーザー名]**&#x200B;を選択します。
   1. ビューを保存します。\
      これにより、重複を検索できるユーザー名が表示されるビューが表示されます。

1. ユーザーのリストで、**[!UICONTROL ユーザー名]**&#x200B;列を調べて、重複するユーザー名がないことを確認します。
