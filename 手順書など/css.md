# CSSの基本 (初心者向け)

CSS（Cascading Style Sheets）は、Webサイトの**見た目**を整えるための言語です。
HTMLで作った骨組みに、色やフォント、レイアウトなどのデザインを付け加えます。

## 1. 基本的な書き方

CSSは、「どこに（セレクタ）」「何を（プロパティ）」「どうする（値）」という形式で書きます。

```css
/* セレクタ { プロパティ: 値; } */
h1 {
  color: blue; /* 文字の色を青にする */
  font-size: 24px; /* 文字の大きさを24ピクセルにする */
}
```

## 2. よく使うプロパティ一覧

| プロパティ | 説明 | 例 |
| :--- | :--- | :--- |
| `color` | 文字の色 | `red`, `#ff0000`, `rgb(255,0,0)` |
| `background-color` | 背景の色 | `white`, `skyblue` |
| `font-family` | フォントの種類 | `'Arial', sans-serif` |
| `margin` | 要素の外側の余白 | `10px`, `auto` |
| `padding` | 要素の内側の余白 | `20px` |
| `border` | 枠線 | `1px solid black` |
| `text-align` | 文字の配置 | `center`, `right` |

## 3. クラス（Class）とID

特定の要素だけにスタイルを適用したいときは、HTMLで「クラス名」を付けます。

```html
<!-- HTML -->
<p class="highlight">この文章だけ目立たせたい！</p>
```

```css
/* CSS (クラス名の前には . を付ける) */
.highlight {
  background-color: yellow;
  font-weight: bold;
}
```

## 4. ハンズオンでのポイント

今回のハンズオンでは、テンプレートの `index.css` を開いて、以下の部分を探してみましょう。

- `body` の `background-color` を変えて、全体の雰囲気を変える
- `.profile-name` などのクラスを探して、文字の色や大きさを変える
- `margin` や `padding` の数字を変えて、余白を調整する

AIに「このCSSを、もっとモダンでスタイリッシュなデザインにして」と頼むと、一気にプロっぽい見た目に変えてくれます！

※このファイルは、ハンズオン担当者である須藤が作成した[プログラム](https://github.com/s-taku0502/markdown_converter)によって、Markdown ファイルをPDF 化したものです。
