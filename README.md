# 2026 GDGoC KIT welcome event

※このハンズオンでは、既存テンプレートを使用して、自分たち独自の名刺やプロフィールサイトをつくり、AIを用いたコーディングによるプログラミングへの不安解消を目的とする。

---

## 🚀 ハンズオン概要

このハンズオンでは、GitHub上のテンプレートをベースに、自分だけの**デジタル名刺（プロフィールサイト）**を作成します。
プログラミング未経験の方でも、AI（ChatGPTやGitHub Copilotなど）を活用することで、驚くほど簡単にWebサイトをカスタマイズできる体験を提供します。

### 🎯 目的

- プログラミングに対する「難しそう」という不安を解消する
- AIを使った効率的なコーディング手法を体験する
- 自分だけのオリジナルプロフィールサイトを公開する

## 🛠 事前準備

ハンズオンをスムーズに進めるために、以下の準備をお願いします。

1. **GitHubアカウントの作成**
   - [GitHub](https://github.com/)にサインアップしておいてください。
2. **Discordへの参加**
   - GDGoC KITのDiscordサーバーに参加してください。
3. **PCの持参**
   - 学内Wi-Fiに接続可能なノートPCを持参してください。
4. **Googleアカウントの準備**
   - Cloud Shellを利用するため、Googleアカウントにログインできる状態にしておいてください。

## 📝 手順

### 1. テンプレートの準備

1. [DigitalNameCard リポジトリ](https://github.com/KIT-GDGoC/DigitalNameCard)にアクセスします。
2. 右上の「code」をクリックし、画像右側のコピーボタンを押して、リポジトリのURLをコピーします。

### 2. Cloud Shellでのクローン（複製）

1. [Google Cloud Shell](https://shell.cloud.google.com/)にアクセスします。
2. ターミナルで以下のコマンドを実行して、リポジトリをクローンします。

   ```bash
   git clone https://github.com/KIT-GDGoC/DigitalNameCard.git
   ```

### 3. クローン（複製）したリポジトリを、自分のGitHubアカウントにコピーする

1. Google Cloud Shellの画面の左上にある「ファイル」アイコンをクリックし、「Open Folder」を選択して、クローンした `DigitalNameCard` フォルダを開きます。

2. 以下のコマンドを実行して、リモートリポジトリを自分のGitHubアカウントに変更します。

    ```bash
    # 1行ずつ実行してください
    cd DigitalNameCard
    git remote set-url origin https://github.com/あなたのユーザー名/DigitalNameCard.git  
    ```

3. 変更を保存（コミット）し、GitHubにアップロード（プッシュ）します。

    ```bash
    # 1行ずつ実行してください
    git add .  
    git commit -m "Initial commit: Cloned template"  
    git push origin main  
    ```

### 4. AIと一緒にカスタマイズ

1. Cloud Shellの左上にある「ファイル」アイコンをクリックし、エディタを開きます。
2. `DigitalNameCard` フォルダの中から、`one`, `two`, `three`, `portfolio` のいずれか好きなテンプレートを選びます。

※選ぶテンプレートによって、サイトのデザインや構成が異なります。以下は各テンプレートのイメージです。

**テンプレート「One」**

![](https://res.cloudinary.com/dbf2ta8pg/image/upload/v1776247653/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88_2026-04-15_183209_resexb.png)

~~

**テンプレート「Two」**

![](https://res.cloudinary.com/dbf2ta8pg/image/upload/v1776247653/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88_2026-04-15_183503_hhgzyy.png)

~~

**テンプレート「Three」**

![](https://res.cloudinary.com/dbf2ta8pg/image/upload/v1776247653/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88_2026-04-15_183529_ciekvj.png)

~~

**テンプレート「Portfolio」**

![](https://res.cloudinary.com/dbf2ta8pg/image/upload/v1776247653/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88_2026-04-15_184230_tdadjv.png)

~~

3. 選んだテンプレートフォルダ内の `index.html` や `index.css` を開き、AI（画面右のGemini など）に以下のように指示を出してみましょう。
   - 「名前を『〇〇 太郎』に変えて」
   - 「背景色をパステルブルーにして」
   - 「自己紹介のセクションを追加して」

4. プレビューは、次のセッション「ウェブでプレビュー」を確認してください。

5. AIが提案したコードを貼り付けて、サイトがどう変わるか確認します。
   - Cloud Shellの「ウェブでプレビュー」機能（右上の四角いアイコン）を使うと、編集中のサイトをブラウザで確認できます。

### 5. ウェブでプレビュー

画面左側に、画像のようなアイコンが記されていると思います。

![](https://res.cloudinary.com/dbf2ta8pg/image/upload/v1776247652/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88_2026-04-15_185123_bolfk1.png)

1. その中から、四角が積んである「Extension」を選択してください。
2. 「Extension」の中から、「Live Server」を検索し、選択してください。
3. 「Live Server」をインストールしてください。
4. インストールが完了したら、編集している `index.html` を右クリックし、「Open with Live Server」を選択してください。
5. ブラウザが自動で開き、編集した内容が反映されたサイトが表示されます。

### 6. 変更のコミットとプッシュ

1. 編集が終わったら、Cloud Shellのターミナルで以下のコマンドを実行して変更を保存（コミット）し、GitHubにアップロード（プッシュ）します。

   ```bash
   # 1行ずつ実行してください
   git add .
   git commit -m "feat: My profile site customization"
   git push origin main
   ```

### 6. サイトの公開

1. GitHubの自分のリポジトリページに戻ります。
2. 「Settings」タブ > 左側のメニューから「Pages」を選択します。
3. 「Source」で `main` ブランチと `/(root)` フォルダを選択し、「Save」をクリックします。
4. 数分待つと、あなたのプロフィールサイトが世界中に公開されます！

## 📚 学習用資料

- [HTMLの基本 (html.md)](./手順書など/html.md)
- [CSSの基本 (css.md)](./手順書など/css.md)
※このファイルは、ハンズオン担当者である須藤が作成した[プログラム](https://github.com/s-taku0502/markdown_converter)によって、Markdown ファイルをPDF 化したものです。
