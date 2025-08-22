---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS ログアウト URL が機能しない
description: このページで説明する手順は、まだ Adobe Admin Console にオンボーディングされていない組織にのみ適用されます。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 5a2df341a54d305807a1c9f175baf60b9007ffa2
workflow-type: tm+mt
source-wordcount: '67'
ht-degree: 37%

---

# ADFS ログアウト URL が機能しません

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>このページで説明されている手順は、Adobe Admin Consoleにまだオンボーディングされていない組織にのみ適用されるので、削除されました。
>
>すべてのWorkfront組織がAdobe Admin Consoleにオンボーディングされました。

<!--DELETE ME MARCH 2026-->

<!--

## Problem

When using the ADFS logout URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), you receive a message page with the error: "There was a problem accessing the site. Try to browse to the site again."

If the problem persists, contact the administrator of this site and provide the following reference number to identify the problem: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] license</td> 
   <td> 
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

1. In your ADFS manager server, go to **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** > `<your party trust>` properties.

1. Under the **[!UICONTROL Endpoints]** tab, click **[!UICONTROL Add]**.

1. **[!UICONTROL Endpoint Type]** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   You can set a response URL if you want it to redirect to another page. But we recommend the ADFS site because it warns that you are logged off, but you should still close your browser.
-->