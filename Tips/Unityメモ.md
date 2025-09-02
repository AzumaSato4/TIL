# Unityメモ

## コンポーネントの情報（Rigidbody2D）を取得

変数名 = GetComponent<Rigidbody2D>();

## 指定方向キーの入力されたかどうか

Input.GetAxisRaw(指定方向キー)
- 戻り値はfloat型
- 1.0f or 0 or -1.0fで戻ってくる
- Horizontal：水平、Vertical：垂直

## linearVelocityに値を代入

コンポーネント情報を取得している変数名.linearVelocity = new Vector2(x方向, y方向);

## フレームレート制御

'''c#
private void FixedUpdate()
{
    処理
}
'''

## インスペクターで変数の値を変更

変数前にpublicをつける