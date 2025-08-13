# CSSプロパティ集

## ress リセットCSS（自分のCSSより上に書く）
`<link rel="stylesheet" href="https://unpkg.com/ress/dist/ress.min.css"/>`


## color	文字色

## font-size	文字の大きさ

## font-weight	文字の太さ
太字

`font-weight: bold;`

## background-color	背景色

## background-image	背景に画像を設置

## width	幅

## height	高さ

## max-width	最大幅

## background-repeat	背景画像の繰り返し

## background-size	背景画像の大きさ
背景画像を縦横比を保持したまま全表示

`background-size: cover;`

背景画像を縦横比を保持したまま空白あり表示

`background-size: contain;`

## background-position	画像の中心点
背景画像の中心点を真ん中にする

`background-position: center center;`

## margin	外側余白

## padding	内側余白

## border-radius	角の丸み

## text-align	文章に位置
文章を中央揃え

`text-align: center;`

## text-decoration: none;	下線を無くす

## box-sizing: border-box;	余白計算を含み計算にする

## display 要素の並ぶ型
- inline 平べったく横並び
- block 横いっぱいに広がる縦並び
- inline-block block型を横並び
- flex 大雑把に整列
- grid 細かく整列（数値入力必要）

## flex-direction flex型での並び方
- colums 縦並び
- rows 横並び

## grid-template-colums grid型での横並びの比率
- 1fr 1fr 1fr 「1:1:1」
- repeat(3, 1fr) 「1:1:1」
- 1/5 「区切りの1から5まで広げる」

## grid-template-rows grid型での縦並びの比率

## justify-content 要素の進行方向に対して要素を揃える
- center 中央揃え
- space-between 両端と均等配置
- space-around 均等配置

## aline-item 要素の進行方向に対して垂直に要素を揃える

## list-style-type: none; リストのマークを消す

## gap 子要素の隙間を作る（内側）

## object-fit 大きさによって比率は崩さない（初期値中央のまま）
- contain 余りは切り取る
- cover 不足は伸ばす

## border 線を引く
以下を指定
- 太さ
- 種類
- 色

## aspect-ratio 比率を変える

## border-collapse: collapse; 表の枠を一本の直線にする

## sursor: pointer; マウスオーバーを指カーソルに変更

## box-shadow boxに影をつける
box-shadow: 右 下 ぼかし 色;

## line-height 行間

## @media(max-width: ) レスポンシブ対応
