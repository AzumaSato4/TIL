# C#文法集

## Console.WriteLine();

コンソールに文字を表示する

## 型

- int -> 整数
- string -> 文字列
- float -> 単精度浮動小数点（処理速度優先、数字の後ろに必ず「f」）
- double -> 倍制度浮動小数点（精度優先、扱える範囲が広い）
- bool -> 真偽のみ

## 型変更

- 数字型 -> 別の数字型 変数の前に「(変換後の型名)」
- 文字列 -> 整数 「x = int.Parse();」

## 条件分岐

- if文

```c#
if (条件)
{
    処理
}
else if (条件)
{
    処理
}
else
{
    処理
}
```

-switch文  
条件に変数名書く必要なし

```c#
switch (変数)
{
    case 条件1:
        処理
        break;
    case 条件2:
        処理
        break;
    default:
        処理
        break;
}
```

## 配列

```c#
型[] 変数名 = new 型[];
変数名[0] = 値;
変数名[1] = 値;
変数名[2] = 値;
変数名[3] = 値;
```

```c#
変数名.Length
```

配列の長さを値として出力


## 乱数

```c#
Random 変数名 = new Random();
変数名.Next(a,b)
a以上b未満
```

## 繰り返し

- for文 -> 条件回まで繰り返す

```c#
for (int i = 0; i < 10; i++)
{
    処理
}
```

- foreach -> 変数の要素をすべて取り出す

```c#
foreach(int n in 変数名)
{
    処理
}
```

- while文 -> 条件の間ずっと繰り返す

```c#
while (条件)
{
    処理
}
```

## アクセス修飾子

- public すべてのクラスからアクセス可能
- protected 自分or派生のクラスのみアクセス可能
- private 自分のクラス以外からアクセス不可

## プロパティから変数に干渉

```c#
public string 変数名（頭は大文字）
{
    get { return 変数名; } 読み取り機能
    set { 変数名 = 代入する変数名; } 書き込み機能
}
```

## オーバーライド

- 継承元に「virtual」宣言
- 継承先に「override」宣言

## リスト

```c#
List<型名> 変数名 = new List<型名>();
変数名.Add(値);
```

```c#
変数名.Count
```

リストの長さを値として出力

## ディクショナリー

```c#
Dictionary<キー型名, 型名> 変数名 = new Dictionary<キー
型名, 型名>();
```

## ラムダ式

```c#
int Add(int n)
{
    return n + 5;
}
```

↓ラムダ式

```c#
n => n+ 5
```

***

```c#
int Add(int a, int b)
{
    return a + b;
}
```

↓ラムダ式

```c#
(a, b) => a + b
```

***

```c#
bool InPositive(int n)
{
    return n >= 0;
}
```

↓ラムダ式

```c#
n => n >= 0
```

