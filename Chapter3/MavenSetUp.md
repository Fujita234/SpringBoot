# Mavenのセットアップ方法

1, https://maven.apache.org/download.cgi　のサイトに飛ぶ

2, FilesのLinkにファイルがまとめてある

3, 以下に該当するファイルをダウンロードする

* WindowsならBinary zip archiveのzipファイル
* MacならBinary tar.gz archiveのtar.gzファイル

4, Windowsの場合、「システム -> 詳細設定 -> 環境変数 -> システム環境設定のリストにあるPathを選択し編集ボタンをクリック」

5, そこにダウンロードし、解凍したapache-mavenフォルダにあるbinファイルにパスを設定する(Pathの最後は/binになるぞ)

6, Mavenでプロジェクトを生成する(ことを今からやります)

7, プロジェクトを作成したい場所へ移動する

8, 「mvn archetype:generate」コマンドを実行

9, 「case sensitive contains): 整数: 」みたいなところで止まったらEnterを押す

10, 「Choose a number: 数字:」が出たらEnter

11, 「Define value for property 'groupId': :」と出てきたらグループIdを記入

書き方は「com.名前.なんの目的で作るプロジェクトなのか」みたいな感じ

12, 「Define value for property 'artifactId': :」と出てきたらアーティファクトIDを記入

書き方は「アプリケーション名」みたいな感じ

13, 「Define value for property 'version': バージョン:」が出てきたらデフォルトのままでいいのでEnter

14, 「Define value for property 'package':」と出てきたらデフォルトのままでいいのでEnter

15, 「Y」と出てきたら実行するという意味なのでEnter

16, 「BUILD SUCCESS」と出たら成功

17, 本当成功が確かめてみよう

18, 出来たファイルに移動

19, 「mvn compile」コマンドを実行

20, 「mvn package」コマンドを実行

21, 「mvn spring-boot:run」コマンドを実行

22, ただし、今このコマンドを実行するとErrorになる。それはGradleの設定がまだだから、なので次はGradleの設定をしよう


-------------------Macの場合---------------------------

4, ホームディレクトリ内にある「.bash_profile」ファイルにパスを記入する
