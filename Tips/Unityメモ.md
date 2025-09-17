# Unityメモ

## コンポーネントの情報（Rigidbody2D）を取得

```c#
変数名 = GetComponent<Rigidbody2D>();
```

## 指定方向キーの入力されたかどうか

```c#
Input.GetAxisRaw(指定方向キー)
```

- 戻り値はfloat型
- 1.0f or 0 or -1.0fで戻ってくる
- Horizontal：水平、Vertical：垂直

## linearVelocityに値を代入

```c#
コンポーネント情報を取得している変数名.linearVelocity = new Vector2(x方向, y方向);
```

## フレームレート制御

```c#
private void FixedUpdate()
{
    処理
}
```

## インスペクターで変数の値を変更

変数前にpublicをつける

## 指定キーが入力されたかどうか

```c#
Input.GetButtonDown("指定キー")
```

## ジャンプ

```c#
AddForce(方向, ForceMode2D.Impulse);
```

## サークルキャスト

```c#
変数名 = Physics2D.CircleCast(
    発射位置,
    円の半径,
    発射方向,
    発射距離,
    対象レイヤー
)
```

## レイヤー変数の宣言

```c#
LayerMask 変数名;
```

## Updateの中でパソコンの性能差に左右されずに機能させる

(Time.deltaTime)を掛け算する

## 当たり判定

- Add Component > Colliderで付与
- is Triggerにチェックを入れるとすり抜けられる

## 簡単に他から読み書きができる

- 変数（型）の前に「static」を入れる

## コンソールに表示する

```c#
Debug.Log("表示");
```

## 時間差でメソッドを実行

メソッドを1秒後に実行

```c#
Invoke("メソッド名", 1.0f);
```

## TextMeshProについて

 - TextMeshProUGUI
 - using TMProを設定すると使える

## 型変更

- int型 -> string型 = 後ろに「.ToString()」をつける

## 切り上げ

Mathf.Ceil(変えたい変数)

## 物体間の距離

物体Aと物体Bの距離

```c#
Distance(物体A, 物体B);
```

## 特定タグのオブジェクトを探す

```c#
GameObject.FindGameObjectWithTag("タグ名")
```

## 生成メソッド

```c#
Instantiate(生成物, 場所, 回転)
```

## 指定移動

```c#
Vector2.Lerp(開始位置, 終了位置, 進捗率)
```

↓times分の時間をかけて移動する

```c#
float distance = Vector2.Distance(startPos, endPos); //移動距離
float ds = distance / times; //1秒の移動距離
float df = ds * Time.deltatime; //1フレームの移動距離
movep += df / distance; //移動補完値（進捗率）
```

## 現在シーン情報の取得

```c#
GetActiveScene();
```

## 完成後のビルド

以下を設定

- Compression Format <- Gzip
- Decompression Fallback <- ON

## コルーチンのメソッド

```c#
IEnumerator メソッド名(){}
```

## 角度を求める

```c#
//第一引数に高さY、第二引数に底辺Xを与えると角度をラジアン形式で算出（演習の長さで表現）
float rad = Mathf.Atan2(dirY, dirX);

//ラジアン値をオイラー値(デグリー)に変換
angle = rad * Mathf.Rad2Deg;
```
