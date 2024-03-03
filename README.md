# PHP(laravel)を用いたプロジェクト ~how to~

## レポジトリの作り方とファイルへの接続法

### コマンド

まず初めにレポジトリを GitHub で作る。  
そしたら以下のコマンドを実行する。  
`git init`  
"README.md"を作った後に、  
`git add README.md`  
`git commit -m "first commit"`  
`git branch -M main`  
`git remote add origin gitのリンク`  
`git push -u origin main` (なんか`-u`入れなくてもできちゃった...)  
そしたら GitHub 上のレポジトリのページの画面が変わる。

## Laravel のインストール手順

samuraiengineer のサイト：  
[https://www.sejuku.net/blog/106106#index_id2]  
vscode でプロジェクトを始めるには：  
[https://blog-shima-haxtuti.com/vscode-laravel/]  
laravel 関係のおすすめの拡張機能：  
[https://papagram.com/?p=267]

### PHP 環境の導入

### Composer のインストール

### Laravel のインストール

## clone を作ろーん

文献：[https://qiita.com/samurai_runner/items/7442521bce2d6ac9330b]

### ターミナルから clone を実行

`$ git clone gitのリンク`  
C:\Usser\sakka> の状態から行うと  
C:\Usser\sakka\git のリンクのレポジトリ名>にフォルダが現れる。  
だから次にはそこに移動する。

### Pull Request 用の Branch を作成する

`$ cd レポジトリ名`  
`$ git checkout -b develop`

### さて編集

さて編集といったときに忘れてはいけないのがレポジトリ(プロジェクト)名のフォルダを開くこと

#### C:\Usser\sakka\git のリンクのレポジトリ名>

↑ こういった形でフォルダが追加されたことを思い出そう。

#### ......あとはいつもの動作

...ブランチを作成し、そこに移動。  
`$ git checkout -b ブランチ名`  
...ステージング。  
`$ git add .`  
...本番へコミット。  
`$ git commit -m "コメント"`  
...リモートレポジトリにプッシュ。  
`$ git push origin ブランチ名`  
GitHub でプルリクエストをマージ。  
コマンドに戻る。  
...main ブランチに戻る。  
`$ git checkout main`  
...最新化（？）。  
`$ git fetch`  
...リモートレポジトリのモノを main ブランチにマージ。  
`$ git merge origin/main`
