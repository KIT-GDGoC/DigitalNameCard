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

1. クローンしたリポジトリのディレクトリに移動します。

   ```bash
    cd DigitalNameCard
    ```  

2. 以下のコマンドを実行して、リモートリポジトリを自分のGitHubアカウントに変更します。

    ```bash
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
3. 選んだテンプレートフォルダ内の `index.html` や `index.css` を開き、AI（ChatGPTやGitHub Copilotなど）に以下のように指示を出してみましょう。
   - 「名前を『〇〇 太郎』に変えて」
   - 「背景色をパステルブルーにして」
   - 「自己紹介のセクションを追加して」
4. AIが提案したコードを貼り付けて、サイトがどう変わるか確認します。
   - Cloud Shellの「ウェブでプレビュー」機能（右上の四角いアイコン）を使うと、編集中のサイトをブラウザで確認できます。

### 5. 変更のコミットとプッシュ

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
