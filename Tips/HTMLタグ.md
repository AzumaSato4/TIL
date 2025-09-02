# HTMLタグ集

## nav ナビゲーションメニュー

```html
<nav> </nav>
```

## article 読み物、記事部分

```html
<article> </article>
```

## section テーマを持ったグループ

```html
<section> </section>
```

## aside サイドバー

```html
<aside> </aside>
```

## div 意味を持たないグループ

```html
<div> </div>
```

## span 意味を持たないグループ（改行なし）

```html
<span> </span>
```

## ol 番号付き箇条書き

```html
<ol> </ol>
```

## ul 番号なし箇条書き

```html
<ul> </ul>
```

## li 箇条書きするアイテム

```html
<li> </li>
```

## a リンクを貼る

```html
<a href=""> </a>
```

リンクを貼る（別タブで開く）

```html
<a href="" target="_blank"> </a>
```

ページ内リンク（id名）

```html
<a href="#"> </a>
```

## img 画像を挿入

```html
<img src="" alt="">
```

## table 表を作成

```html
<table>
  <thead>
    <tr>
      <th>種類1</th>
      <th>種類2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>アイテム1</td>
      <td>アイテム2</td>
    </tr>
    <tr>
      <td>アイテム3</td>
      <td>アイテム4</td>
    </tr>
    <tr>
      <td>アイテム5</td>
      <td>アイテム6</td>
    </tr>
  </tbody>
</table>
```

## フォーム作成

```html
<form action="#" method="post" class="contact-form">
  <div>
    <label for="name">お名前:</label>
    <input type="text" id="name" name="user_name">
  </div>
  <div>
    <label for="email">メールアドレス:</label>
    <input type="email" id="email" name="user_email">
  </div>
  <div>
    <label for="message">お問い合わせ内容:</label>
    <textarea id="message" name="user_message"></textarea>
  </div>
  <input type="submit" value="送信する">
</form>
```

## © コピーライト

```html
&copy;
```
