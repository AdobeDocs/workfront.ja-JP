---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront for Adobe Experience Manager拡張コネクタのアンインストール
description: WorkfrontとAdobe Experience Manager Assetsas a Cloud Serviceを接続する最新のネイティブ統合に対して、Adobe Experience Manager拡張コネクタ付きWorkfrontをアンインストールする必要があります。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Adobe Experience Manager拡張コネクタ付きWorkfrontのアンインストール

WorkfrontとAdobe Experience Manager Assetsas a Cloud Serviceを接続する最新のネイティブ統合に対して、Adobe Experience Manager拡張コネクタ付きWorkfrontをアンインストールする必要があります。

## 前提条件

* （オプション）必要に応じて、Workfrontファイアウォール設定およびAEM Dispatcher 設定に加えた変更を元に戻します。

## 拡張コネクタのアンインストール

1. Cloud Manager からAEM as a Cloud Serviceリポジトリにアクセスしてクローンを作成します。

1. 任意の IDE で、クローン Git リポジトリを開きます。

1. 拡張コネクタがインストールされているブランチをチェックアウトします。

1. 次のパスに移動し、拡張コネクタ zip ファイルを削除します。

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. プロジェクトのルートの pom.xml ファイルから次の依存関係を削除します。

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >上記のコードブロック (1.8.0) で参照されているバージョンが、コードからアンインストールされているバージョンを反映していることを確認してください。

1. 次の依存関係を、という名前のプロジェクトのサブモジュールの pom.xml ファイルから削除します。 **すべて**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```
1. 次の埋め込みを、プロジェクトのサブモジュール (all) の pom.xml ファイルから削除します。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. （条件付き）プロジェクトのルートの pom.xml ファイルからリポジトリ設定を削除します。


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. （条件付き）次のパスにある settings.xml からサーバー設定を削除します。/cloudmanager/maven/settings.xmlをプロジェクトルートに追加します。

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. 変更をコミットし、コードを Cloud Manager リポジトリにプッシュします。

1. Cloud Manager パイプラインを実行して、変更をCloud Servicesインスタンスにデプロイします
