---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflake用のリーダーアカウントの作成
description: Data Connect データにアクセスするには、まずSnowflake リーダーアカウントを作成する必要があります。
author: Courtney
feature: Reports and Dashboards
hide: true
hidefromtoc: true
source-git-commit: a42c13804b0463af27bac6f9166bc6e3c41d3fda
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 8%

---


# テスト

## アクセスレベル

<table>
  <thead>
    <tr>
        <th>Workfront エンティティ名</th>
        <th>インターフェイス参照</th>
        <th>API リファレンス | ラベル</th>
        <th>データレイクの表示</th>
    </tr>
  </thead>
 <tr>
        <td>アクセスレベル</td>
         <td>アクセスレベル</td>
        <td>ACSLVL | アクセス レベル</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong> 関係フィールド </strong> <br>
         ACCESSLEVELID （self）: セルフ <br>
         APPGLOBALID：関係ではありません。内部アプリケーション目的で使用されます <br>
         LASTUPDATEDBYID: USER_CURRENT | ユーザー ID<br>
         LEGACYACCESSLEVELID：関係ではありません。内部適用のために使用されます <br>
         OBJID: OBJCODE フィールドで識別されるオブジェクトの ID <br>
         SYSID：関係ではありません。内部アプリケーション目的で使用されます</td>
    </tr>
</table>

## アクセスレベル

<table>
  <thead>
    <tr>
        <th>Workfront エンティティ名</th>
        <th>インターフェイス参照</th>
        <th>API リファレンス | ラベル</th>
        <th>データレイクの表示</th>
    </tr>
  </thead>
 <tr>
        <td>アクセスレベル</td>
         <td>アクセスレベル</td>
        <td>ACSLVL | アクセス レベル</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong> 関係フィールド </strong> <br>
         <ul>
            <li>ACCESSLEVELID （self）: セルフ</li>
            <li>APPGLOBALID：関係ではありません。内部アプリケーション目的で使用されます</li>
            <li>LASTUPDATEDBYID: USER_CURRENT | ユーザー ID</li>
            <li>LEGACYACCESSLEVELID：関係ではありません。内部適用目的で使用されます</li>
            <li>OBJID: OBJCODE フィールドで識別されたオブジェクトの ID</li>
            <li>SYSID：関係ではありません。内部アプリケーション目的で使用されます</li>
        </ul>
    </tr>
</table>