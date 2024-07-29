---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Admin Console を使用してAdobe Workfront Fusion にユーザーを追加する
description: ユーザーを Adobe Admin Console に追加して Adobe Workfront Fusion に割り当てたり、Adobe Admin Console の既存のユーザーを Workfront Fusion に割り当てたりすることができます。
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: b7ceec2750ded516cae20d12b991b8fec94c6029
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 93%

---

# [!DNL Adobe Admin Console] を通じて [!DNL Adobe Workfront Fusion] にユーザーを追加

>[!IMPORTANT]
>
>このページで説明する手順は、[!DNL Adobe Admin Console] に登録されている組織にのみ適用されます。
>
>組織がまだ[!DNL Adobe Admin Console]に登録されていない場合には、[ [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md) 組織にユーザーを追加を参照してください。
>
>組織が[!DNL Adobe Admin Console]に登録されているかどうかに基づいて異なる手順のリストについて詳しくは、[プラットフォームベースの管理の違い（[!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform]）](../fusion-in-admin-console/fusion-adobe-admin-console.md)を参照してください。

ユーザーを [!DNL Adobe Admin Console] に追加して、[!DNL Adobe Workfront Fusion] に割り当てるか、[!DNL Adobe Admin Console] に既存のユーザーを [!DNL Workfront Fusion] に割り当てます。

ユーザーの追加方法などを含む、[!DNL Adobe Admin Console] の [!DNL Workfront Fusion] を説明するビデオについて詳しくは、Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank} の [[!DNL Fusion]  を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] 管理者権限</td> 
   <td>組織の [!DNL Adobe] 製品の [!UICONTROL Product Configuration Administrator] 管理者である必要があります。</td> 
  </tr>
  </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。



## 前提条件

[!DNL Workfront] に [!DNL Admin Console] を使用する前に、コンソールへの招待メールが届くはずです。

1. [!DNL Adobe] を初めて使用する場合で、組織の [!DNL Adobe] ソフトウェアとサービスを管理する管理者権限があることを知らせるメールを受け取った場合には、メール内のボタンをクリックして [!DNL Adobe] アカウントを作成して、[!DNL Admin Console] を開きます。

   または

   既に Adobeアカウント がある場合は、[[!DNL Adobe Admin Console] ページ](https://adminconsole.adobe.com/)に移動します。


## [!DNL Adobe Admin Console] および [!DNL Workfront Fusion] に新しいユーザーを追加

1. [[!DNL Adobe Admin Console] ページ](https://adminconsole.adobe.com/)から、上部ナビゲーションバーの「**[!UICONTROL 製品]**」タブを選択し、**[!DNL Workfront Fusion]**&#x200B;製品タイルを選択します。

   ![Admin Console 内の Fusion](assets/fusion-product-admin-console.png)

1. 表示されるリストで、ユーザーを追加する組織を選択します。

   ![Admin Console 内の Fusion インスタンス](assets/fusion-instances-admin-console.png)

1. 表示されるリストで、「**[!UICONTROL 製品プロファイル]**」タブが選択されている場合、[!DNL Workfront Fusion] [!UICONTROL 製品プロファイル]リンクの名前をクリックします。

   ![Workfront Fusion 製品プロファイル](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > [!UICONTROL 製品プロファイル]自体には、変更を加えないでください。

1. リストの上で「**[!UICONTROL ユーザー]**」タブを選択し、「**[!UICONTROL ユーザーを追加]**」をクリックします。

1. **[!UICONTROL この製品プロファイルにユーザーを追加]**&#x200B;ボックスに、追加するユーザーのメールアドレスまたは名前を入力し、表示されるリストからそのユーザーを選択します。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ユーザーが [!DNL Workfront Fusion] に作成されました。

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. （オプション）[ [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion) でのユーザーのアクセスレベルの変更に進みます。

## Workfront Fusion でのユーザーのアクセスレベルを変更

### ユーザーの役割を管理者に変更

ユーザーに管理者の役割を割り当てる場合は、[!DNL Adobe Admin Console] で実行する必要があります。

1. [!DNL Workfront Fusion] のユーザーを追加した[!UICONTROL 製品プロファイル]ページで、「**[!UICONTROL 管理者]**」タブを選択します。

1. 「**[!UICONTROL 管理者を追加]**」をクリックします。

1. 「**[!UICONTROL 製品プロファイル管理者の追加]**」ボックスで、追加するユーザーのメールアドレスまたは名前を入力し、表示されるリストからそのユーザーを選択します。

1. 「**[!UICONTROL 保存]**」をクリックします。

   このユーザーが [!DNL Workfront Fusion] の管理者になりました。

### ユーザーの役割を[!UICONTROL メンバー]、[!UICONTROL 経理担当者]、または[!UICONTROL アプリ開発者]に変更します。

[!UICONTROL メンバー]、[!UICONTROL 経理担当者]、および[!UICONTROL アプリ開発者]の役割は、[!DNL Workfront Fusion] の内部で処理されます。

手順については、[組織の  [!DNL Adobe Workfront Fusion]  ユーザーの管理](../organizations/manage-fusion-users.md)の記事にある[ユーザーの役割の表示または編集](../organizations/manage-fusion-users.md#view-or-edit-user-roles)を参照してください。

## [!DNL Adobe Admin Console] の既存ユーザーの [!DNL Workfront Fusion] への割り当て

Fusion で既存のユーザーをチームに追加できます。 これは Fusion 内で処理されます。

手順については、Adobe Workfront Fusion での組織またはチームへのユーザーの追加の記事の [ チームにユーザーを追加する ](/help/quicksilver/workfront-fusion/organizations/add-user-to-an-organization.md#add-a-user-to-a-team) を参照してください。
