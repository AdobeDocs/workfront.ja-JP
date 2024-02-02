---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager 拡張コネクタ用の Workfront のアンインストール
description: Adobe Experience Manager 拡張コネクタ付き Workfront（Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合）をアンインストールする必要があります。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: ht
source-wordcount: '259'
ht-degree: 100%

---

# Adobe Experience Manager 拡張コネクタ付き Workfront のアンインストール

Adobe Experience Manager 拡張コネクタ付き Workfront（Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合）をアンインストールする必要があります。

## 前提条件

* （オプション）必要に応じて、Workfront ファイアウォール設定および AEM Dispatcher 設定に加えた変更を元に戻します。

## 拡張コネクタのアンインストール

1. Cloud Manager から AEM as a Cloud Service リポジトリにアクセスしてクローンを作成します。

1. 任意の IDE で、クローン作成した Git リポジトリを開きます。

1. 拡張コネクタがインストールされているブランチをチェックアウトします。

1. 次のパスに移動し、拡張コネクタ zip ファイルを削除します。

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. プロジェクトのルートの pom.xml ファイルから、以下の依存関係を削除します。

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
   >上記のコードブロック（1.8.0）で参照されているバージョンが、コードからアンインストールされているバージョンを反映していることを確認してください。

1. 次の依存関係を、**すべて**&#x200B;という名前のプロジェクトのサブモジュールの pom.xml ファイルから削除します。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. すべてという名前のプロジェクトのサブモジュールの pom.xml ファイルから、以下の埋め込みを削除します。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. （条件付き）プロジェクトのルートの pom.xml ファイルから、リポジトリ設定を削除します。


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. （条件付き）以下のパスにある settings.xml から、サーバー設定を削除します。プロジェクトルートの /cloudmanager/maven/settings.xml

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

1. Cloud Manager パイプラインを実行して、変更を Cloud Service インスタンスにデプロイします
