---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Adobe Workfront Fusion の接続メタデータ
description: Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
source-git-commit: 3a7983279a38c30cb58078d129ea22dee137d9a5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Adobe Workfront Fusion の接続メタデータ

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] にはが必要です [!DNL Adobe Workfront Fusion] に加えてライセンス [!DNL Adobe Workfront] ライセンス。

すべての接続が同じではありません。 接続間の違いを理解することは、ビジネスコンテキストを知る上で非常に重要です。 Fusion では、メタデータを使用して、接続の重要な属性を識別します。

新しい接続を作成する際に、接続メタデータを設定できます。 これらの属性は、接続の設定に使用するのと同じダイアログボックスに表示されます。

![接続メタデータ](assets/connection-metadata-setup.png)

Fusion ユーザーは、[ 接続 ] 領域から接続を表示および編集できます。

![「接続」領域の接続メタデータ](assets/connections-area-metadata.png)

## 環境タイプ

統合接続は、実稼働システムと非実稼働システムの両方で使用できます。 この違いを知ることは、本番環境を保護する上で非常に重要です。 環境タイプは、他の接続メタデータと同様に、情報提供の目的でのみ使用されます。 ユーザーは、引き続きこの属性を正確に設定する必要があります。

## 認証タイプ

統合接続は、サービスアカウントと個人アカウントの両方に使用できます。 Fusion としてシナリオが自動化される場合、サービスアカウントは認証に使用されます。 個人アカウントは、特定の人物に基づく認証です。 どの認証タイプを使用するかは、シナリオの要件によって異なります。 個人アカウントは、自動化されたユーザーアクションに使用する必要があります。 たとえば、Fusion シナリオが特定の人物による承認を自動化する場合、その人物の認証タイプを使用する必要があります。 それ以外の場合、Fusion は Fusion として機能し、型は&quot;Service Account&quot;にする必要があります。

タイプは、他の接続メタデータと同様に、情報提供の目的でのみ使用されます。 ユーザーは、引き続き、この属性を手動で正確に設定する必要があります。

認証タイプについて詳しくは、 [認証](https://developer.adobe.com/developer-console/docs/guides/authentication/) (Adobe認証ガイド )。



