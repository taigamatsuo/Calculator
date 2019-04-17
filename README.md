# Calculator

基本的な変数を理解するための良い課題だったと思う。
扱うデータ型の値が多いため中高生の中には戸惑ってしまう子もいそう。
特に型変換に気をつけたい。


<h3>変数</h3>

再代入を許可する場合は var、許可しない場合(=定数)は let を使用する

```a.swift
var a = 1
a = 2
```

```a.swift
let a = 1
a = 2 // エラー
```

データ型を指定して宣言することもできる

```a.swift
var a: Int
var a: String = "Hello"
```

Swift のデータ型には以下のものがある

**データ型	内容**
String	文字列

Int	

Float	浮動小数点(32bit長)

Double	浮動小数点(64bit長)

Bool	真偽値

Dictionary	辞書型

Array	配列

Any	総称型(何でも入る)

何も指定せずに小数を宣言すると Double 型になる


```a.swift
var a = 100.5 // Double
```


注意点として、計算処理をする時に、Int + Double のような異なる型との計算はエラーになる

```a.swift
var a: Int = 10
var b: Double = 10.5
a + b // エラー
```

こういう場合は、どちらかの型を変換して同じ型同士にする必要があります。以下、よく使用する型変換のパターン


**Int -> Double**

```a.swift
var a: Int = 100
Double(a) // 100
```

**Int -> String**


```a.swift
var a: Int = 100
String(a) // "100"
```

**Double -> Int**

```a.swift
var a: Double = 100.5
Int(a) // 100
```

**Double -> String**

```a.swift
var a: Double = 100.5
String(a)
```

**String -> Int**

```a.swift
var a: String = "100"
Int(a) // 100
```

**String -> Double**

```a.swift
var a: String = "100.5"
Double(a) // 100.5
```

**出力**
コンソールに出力する場合は print を使用する

```a.swift
var a = "Hello"
print(a) // "Hello"
```

文字列の中で出力する場合は \(変数) を使用する

```a.swift
var a = "Hello"
print("aの値は\(a)です") // "aの値はHelloです"
```
