---
content-type: api
navigation-topic: general-api
title: API サンプルスクリプト
description: FAPI サンプルスクリプト
author: John
feature: Workfront API
exl-id: 76c5eca6-be82-4331-9da9-9943e0bda669
source-git-commit: e6bad8cbe84d0f116e9679ecaba5178973a2604f
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# API サンプルスクリプト

## Adobe Workfront API の例

以下は、Workfront RESTful API とのやり取りに使用される様々なプログラミング言語の例です。 各例では、次の操作を実行します。

* 接続を確立します
* ログインしているユーザーの情報を取得します
* プロジェクトのクエリ
* プロジェクトを作成
* プロジェクトを取得します
* プロジェクトを更新します
* プロジェクトを削除
* ログアウト

次の例は、Workfrontの GitHub ページからダウンロードできます。  [https://github.com/Workfront](https://github.com/Workfront)

リポジトリ内で例を検索するには、 `example` に **リポジトリを検索…** ボックス

>[!NOTE]
>
>API の使用は、実稼動環境で実行する前に、Workfrontのベータ環境でテストする必要があります。 お客様が On-Demand Software に負担があると合理的に考えるプロセス（つまり、そのプロセスが他のお客様に対するソフトウェアの実行に重大な悪影響を与える）で API を使用している場合、Workfrontはお客様にそのプロセスの中止を求める権利を留保します。

>[!IMPORTANT]
>
>本ソフトウェアは「現状のまま」で提供され、明示的または黙示的のいかなる種類の保証も付与されません。商品性、特定目的に対する適合性、非侵害に関する保証も含みますが、これに限定されません。 いかなる場合でも、作成者または著作権者は、契約の訴え、不法行為、その他の行為がソフトウェアの使用または他の取引に起因するかにかかわらず、いかなる権利、損害、その他の責任も負いません。
