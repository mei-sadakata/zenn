---
title: "gitコマンドでのpushの仕方" # 記事のタイトル
emoji: "👶" # アイキャッチとして使われる絵文字（1文字だけ）
type: "tech" # tech: 技術記事 / idea: アイデア記事
topics: ["github", "iam", "初心者向け"] # タグ。["markdown", "rust", "aws"]のように指定する
published: false # 公開設定（falseにすると下書き）
---
## はじめに
読む対象者・前提条件など

## 手順
1. 対象のディレクトリに入っているか確認

2.  リポジトリの状態を確認　
``````bash
git status
``````
確認する場所
- changes not staged for commit:
　コミットのため、ステージングされていない変更が表示される
　modified 変更したファイル
　deleted　削除したファイル
- untracked files:
　ローカルで操作したファイルが表示される
![お試し](/images/sample00.png)



3. ステージングエリアに作成・変更したファイルを追加
``````bash
git add ファイルのパス
``````
4. リポジトリの状態を再確認
``````bash
git status
``````

-下記の場所を確認
changes to be committed:
new file: 手順2でステージング環境にしたファイル名がここにあるか確認
![お試し](/images/sample01.png)

5. ステージングエリアの変更内容をコミットする
``````bash
git commit -m “コミットメッセージ”
``````
![お試し](/images/sample03.png)
6. リポジトリの状態を再確認
``````bash
 git status
``````
![お試し](/images/sample04.png)
new filesがなくなっていることを確認

7. ローカルリポジトリの変更内容をリモートリポジトリにプッシュする
``````bash
git push 
``````
commit履歴をみて反映されているか確認
![お試し](/images/sample02.png)



