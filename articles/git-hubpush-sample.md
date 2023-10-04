---
title: "pushの仕方" # 記事のタイトル
emoji: "👶" # アイキャッチとして使われる絵文字（1文字だけ）
type: "tech" # tech: 技術記事 / idea: アイデア記事
topics: ["aws", "iam", "初心者向け"] # タグ。["markdown", "rust", "aws"]のように指定する
published: false # 公開設定（falseにすると下書き）
---
## はじめに
読む対象者・前提条件など

## 手順
1.  リポジトリの状態を確認　
``````
git status
``````
確認する場所
- changes not staged for commit:
　コミットのため、ステージングされていない変更が表示される
　modified 変更したファイル
　deleted　削除したファイル
- untracked files:
　ローカルで操作したファイルが表示される
![お試し](/images/sample.png)



2. ステージングエリアに作成・変更したファイルを追加
``````
git add ファイル名
``````
3. リポジトリの状態を再確認
``````
git status
``````

-下記の場所を確認
changes to be committed:
new file: 手順2でステージング環境にしたファイル名がここにあるか確認

4. ステージングエリアの変更内容をコミットする
``````
git commit -m “コミットメッセージ”
``````

5. リポジトリの状態を再確認
``````
    git status
``````

6. ローカルリポジトリの変更内容をリモートリポジトリにプッシュする
``````
git push 
``````



