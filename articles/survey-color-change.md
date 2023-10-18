---
title: "gitを使った作業手順" # 記事のタイトル
emoji: "👶" # アイキャッチとして使われる絵文字（1文字だけ）
type: "tech" # tech: 技術記事 / idea: アイデア記事
topics: ["github", "iam", "初心者向け"] # タグ。["markdown", "rust", "aws"]のように指定する
published: false # 公開設定（falseにすると下書き）
---
## はじめに
読む対象者・前提条件など

## 手順
1. 作業するリポジトリを確認

2.  ブランチを切る
リポジトリ内の`branches`を押す
`new branch`を押す
branch名をつける


3. vscodeを開く
branchを切る前に最新の状態にする
``````bash
git fetch upstream
``````
ブランチを切り替える
``````bash
git checkout -b 切り替えたいブランチ名
````````
- 下記コマンドでブランチが切れていることを確認

``````bash
git branch
``````

3. 修正を行う


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

- `#5272F2`
- ![](https://via.placeholder.com/16/c7e7f6/FFFFFF/?text=%20) `#c7e7f6`

- `#FF3B30`
- `#34C759`
- `#007AFF`



