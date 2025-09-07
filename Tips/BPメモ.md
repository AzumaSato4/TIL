# BPメモ

## アクタ

### Get Actor Location

- 現在のアクタ位置を取得する

### Set Actor Location

- アクタの現在位置をセット
- Sweepにチェックを入れると移動した間に障害物があるかどうかの当たり判定を実施する

## ベクトル

### Negate Vector

逆ベクトル（-1でスカラー倍）

### Vector Length

ベクトルの大きさ（長さ）を取得

### Normalize

ベクトルを正規化（単位ベクトル＝向きを取得）

### Dot Product

ドット積（内積）

### Cross Product

クロス積（外積）

## コンポーネント

### Projectile Movement

弾丸や手榴弾、ホーミングミサイルなどの動きを実現する飛翔体コンポーネント

### Rotating Movement

アクタを指定速度で自転させる回転コンポーネント。風車や水車、ファンなどを簡単に動かせる。

### Interp To Movement

指定された2点以上の地点を移動するコンポーネント。ゲーム中の動く床や遠景を移動する車や飛行機に利用できる。

### Character Movement

ゲームキャラクターの移動制御をテーマにした高機能コンポーネント。歩行、しゃがみ、ジャンプ、登坂など、基本的なキャラクターの運動をパラメーターを調整するだけで実現できる。

### New Updated Component

アクタの中の特定のコンポーネントを動かす。

- ターゲットピンに移動コンポーネント
- New Updated Componentピンに運動させたいコンポーネント

## その他

### 四則演算

- 直接入力することで定数を入力可能

### Get a reference to self

自分自身を参照する

### Add Movement Input

移動値を送り込む
