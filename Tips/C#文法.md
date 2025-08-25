# C#文法集

## Console.WriteLine();
コンソールに文字を表示する

## 型
- int -> 整数
- string -> 文字列
- float -> 単精度浮動小数点（処理速度優先、数字の後ろに必ず「f」）
- doble -> 倍制度浮動小数点（精度優先、扱える範囲が広い）
- bool -> 真偽のみ

## 型変更
- 数字型 -> 別の数字型 変数の前に「(変換後の型名)」
- 文字列 -> 整数 「x = int.Parse();」

## Console.WriteLine()
入力待ち

## 条件分岐
- if文
```
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

```
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