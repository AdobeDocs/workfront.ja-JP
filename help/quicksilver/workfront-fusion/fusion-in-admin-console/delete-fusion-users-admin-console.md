---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Admin Console を使用したユーザーの削除
description: ユーザーを Adobe Workfront Fusion からのみ削除して、その他のアドビ製品プロファイルへのアクセスは残しておくことも、またはそのユーザーを Adobe Admin Console から完全に削除することもできます。
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: ht
source-wordcount: '288'
ht-degree: 100%

---

# [!DNL Adobe Admin Console] を使用したユーザーの削除

>[!IMPORTANT]
>
>この記事に記載される機能は、組織の [!DNL Adobe Workfront Fusion] のインスタンスが [!DNL Adobe Business Platform] にオンボーディングされている場合にのみ使用できます。
>
>組織が [!DNL Adobe Business Platform] にオンボーディングされているかどうかによって手順は異なります。手順のリストについて詳しくは、[プラットフォームベースの管理上の違い（[!DNL Adobe Workfront Fusion]／[!DNL Adobe Business Platform]）](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md)を参照してください。

ユーザーを [!DNL Adobe Workfront Fusion] からのみ削除して、その他の [!DNL Adobe] プロファイルへのアクセスは残しておくことも、またはそのユーザーを [!DNL Adobe Admin Console] から完全に削除することもできます。

## [!DNL Adobe Workfront Fusion] でのユーザーの削除

[!DNL Adobe Workfront Fusion] でユーザーを削除するには、[!DNL Adobe Admin Console] を使用してユーザーを非アクティブ化する必要があります。

次のいずれかに該当する場合、ユーザーは [!DNL Adobe Admin Console] から非アクティブ化されます。

* ユーザーは製品または製品プロファイルから移動され、他の製品または製品プロファイルに割り当てられません。
* ユーザーは製品プロファイルにリンクされているグループから削除され、製品プロファイルにリンクされている他のグループには含まれません。
* ユーザーは製品プロファイルから削除され、別の製品プロファイルに割り当てられません。
* Workfront Fusion を含む組織でユーザーが削除または非アクティブ化されます。

  手順について詳しくは、[ユーザーの個別管理](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html)の「ユーザーの削除」の節を参照してください。

[!DNL Workfront Fusion] で非アクティブ化をすると、次のようにユーザーに影響を与えます。

* ユーザーが 1 つの組織にのみ存在する場合、そのユーザーは非アクティブ化されます。
* ユーザーが複数の組織に属している場合、[!DNL Adobe Admin Console] でユーザーが変更された組織から削除されます。
* [!DNL Workfront Fusion] でのユーザーの削除におけるその他の考慮事項について詳しくは、[ [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider) でユーザーを削除する際の考慮事項を参照してください。
