# JavaScript授業用ファイル

JavaScriptの授業で使うための、最低限のHTML/CSS/JavaScriptファイル一式です。

学生はこのリポジトリを自分のGitHubアカウントにforkして使います。

## ファイル構成

```text
.
|-- index.html
|-- css/
|   `-- style.css
`-- js/
    `-- app.js
```

## 作業の流れ

1. このリポジトリをforkします。
2. forkした自分のリポジトリで、授業用ブランチを作成します。
3. VS Codeの準備をします。
4. VS Codeでプログラムを記述します。
5. GitHub Pagesで、授業用ブランチを公開対象に設定します。
6. ブラウザで表示を確認します。

## 1. このリポジトリをforkする

1. GitHubでこのリポジトリを開きます。
2. 画面右上の `Fork` を押します。
3. `Owner` が自分のGitHubアカウントになっていることを確認します。
4. `Repository name` は、基本的に `OIC2026-FRONT2` のままにします。
5. `Create fork` を押します。

forkが完了すると、自分のアカウントに次のようなリポジトリが作成されます。

```text
https://github.com/自分のGitHubユーザー名/OIC2026-FRONT2
```

以降の作業は、forkした自分のリポジトリで行います。

## 2. GitHubのサイトで授業用ブランチを作成する

授業ごとにブランチを分けると、回ごとの内容を管理しやすくなります。

例として、`lesson/01` という名前の授業用ブランチを作成します。

1. forkした自分のリポジトリを開きます。
2. 画面上部の `Code` を開きます。
3. ブランチ名が表示されているボタンを押します。
   - 最初は `main` と表示されています。
4. 検索欄に `lesson/01` と入力します。
5. `Create branch: lesson/01 from main` を押します。

別の授業用ブランチを作る場合は、`lesson/01` の部分を変更します。

```text
lesson/02
lesson/03
```

## 3. VS Codeの準備をする

授業ではVS CodeでHTML/CSS/JavaScriptを編集します。

この授業で必須の拡張機能はありません。

### 任意でインストールする拡張機能

| 拡張機能 | 用途 |
| --- | --- |
| Prettier - Code formatter | HTML/CSS/JavaScriptのコードを見やすく整形します。 |
| Japanese Language Pack for Visual Studio Code | VS Codeの画面を日本語で表示します。 |

### インストール方法

1. VS Codeを開きます。
2. 左側の `Extensions` アイコンを押します。
   - 四角形が並んだアイコンです。
3. 検索欄にインストールしたい拡張機能名を入力します。
   - 例: `Prettier - Code formatter`
4. 対象の拡張機能を選びます。
5. `Install` を押します。

`Prettier - Code formatter` を使う場合は、保存時に自動整形する設定にしておくと便利です。

1. VS Code左下の歯車アイコンを押します。
2. `Settings` を開きます。
3. 検索欄に `Format On Save` と入力します。
4. `Editor: Format On Save` にチェックを入れます。
5. 検索欄に `Default Formatter` と入力します。
6. `Editor: Default Formatter` で `Prettier - Code formatter` を選びます。

## 4. VS Codeでプログラムを記述する

授業では、forkした自分のリポジトリをVS Codeで開いて作業します。

### リポジトリをVS Codeで開く

1. forkした自分のリポジトリをGitHubで開きます。
2. `Code` を押します。
3. `Local` の `HTTPS` を選びます。
4. 表示されたURLをコピーします。
5. VS Codeを開きます。
6. `View` > `Command Palette` を開きます。
7. `Git: Clone` を選びます。
8. コピーしたURLを貼り付けます。
9. 保存先のフォルダを選びます。
10. cloneが終わったら、`Open` を押してフォルダを開きます。

### 授業用ブランチに切り替える

1. VS Code左下のブランチ名を押します。
2. 作成した授業用ブランチを選びます。
   - 例: `lesson/01`

ブランチが表示されない場合は、VS Codeのソース管理画面で同期してから、もう一度ブランチを確認します。

### 編集するファイル

主に次のファイルを編集します。

| ファイル | 内容 |
| --- | --- |
| `index.html` | ページの構造を書きます。 |
| `css/style.css` | 文字色、余白、配置などの見た目を書きます。 |
| `js/app.js` | JavaScriptの処理を書きます。 |

### ローカルで確認する

1. VS Codeでファイルを編集します。
2. ファイルを保存します。
3. エクスプローラーで `index.html` を開きます。
4. ブラウザに表示されたページを確認します。
5. 変更後は、ブラウザの再読み込みボタンを押して確認します。

### 変更内容をGitHubに反映する

1. VS Code左側の `Source Control` アイコンを押します。
2. 変更されたファイルを確認します。
3. メッセージ欄に変更内容を入力します。
   - 例: `JavaScriptの練習問題を追加`
4. `Commit` を押します。
5. `Sync Changes` または `Push` を押します。

GitHub Pagesで公開するには、変更内容をGitHubにpushしておく必要があります。

## 5. GitHub Pagesで授業用ブランチを表示させる

GitHub Pagesでは、選んだブランチの内容をWebページとして公開できます。

1. forkした自分のリポジトリを開きます。
2. 画面上部の `Settings` を開きます。
3. 左側メニューの `Pages` を開きます。
4. `Build and deployment` の `Source` で `Deploy from a branch` を選びます。
5. `Branch` で表示したい授業用ブランチを選びます。
   - 例: `lesson/01`
6. フォルダは `/(root)` を選びます。
7. `Save` を押します。

設定後、数分待つとGitHub Pagesに反映されます。

GitHub Pagesの公開URLは次の形式です。

```text
https://自分のGitHubユーザー名.github.io/OIC2026-FRONT2/
```

リポジトリ名を変更した場合は、URLの `OIC2026-FRONT2` の部分も変更後のリポジトリ名になります。

```text
https://自分のGitHubユーザー名.github.io/リポジトリ名/
```

GitHub Pagesでは、URLにブランチ名は入りません。`Settings` の `Pages` で選んだブランチの内容が、上記URLに表示されます。

参考: [Configuring a publishing source for your GitHub Pages site - GitHub Docs](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 6. 確認用の表示方法

### GitHub Pagesで確認する

GitHub Pagesの設定後、次のURLをブラウザで開きます。

```text
https://自分のGitHubユーザー名.github.io/OIC2026-FRONT2/
```

表示が更新されない場合は、次の点を確認します。

- forkした自分のリポジトリを開いているか
- `Settings` > `Pages` で正しい授業用ブランチを選んでいるか
- フォルダに `/(root)` を選んでいるか
- VS Codeで変更内容をcommitしてpushしているか
- 数分待ってからブラウザを再読み込みしたか

### ローカルで確認する

VS Codeで編集したファイルは、`index.html` をブラウザで直接開いて確認します。

1. VS Codeでファイルを保存します。
2. エクスプローラーで `index.html` を開きます。
3. ブラウザに表示されたページを確認します。
4. 変更後は、ブラウザを再読み込みします。

ローカルで見えていても、GitHub Pagesに反映するにはcommitとpushが必要です。

## コマンドで作業する場合の補足

授業ではGitHubのサイトとVS Codeの画面操作を基本とします。コマンドで作業する場合は、forkした自分のリポジトリを使います。

GitHubのサイトで授業用ブランチを作成済みの場合は、次のようにcloneしてブランチを切り替えます。

```bash
git clone https://github.com/自分のGitHubユーザー名/OIC2026-FRONT2.git
cd OIC2026-FRONT2
git switch lesson/01
```

コマンドで授業用ブランチを作成する場合は、次のように実行します。

```bash
git switch main
git pull origin main
git switch -c lesson/01
git push -u origin lesson/01
```

作成したブランチでファイルを編集したら、次のように保存します。

```bash
git add .
git commit -m "授業用ファイルを更新"
git push
```
