## STEP 2：変数とデータ

このSTEPでは、Pythonでプログラムを書くうえで非常に重要な「変数」と「データ」について学びます。

プログラムでは、数字を計算したり、文字を表示したり、条件によって処理を変えたりします。

そのためには、コンピューターの中でデータを扱う方法を理解する必要があります。

このSTEPでは、次の内容を順番に学びます。

- 10 変数
- 11 数値
- 12 文字列
- 13 True / False
- 14 None
- 15 型とtype()

---

# 10 変数

## 変数とは

変数とは、データを入れておくための名前付きの箱のようなものです。

例えば、次のコードを見てください。

```python
name = "太郎"

このコードでは、name という変数に "太郎" という文字列を入れています。

イメージすると、

name
 ↓
┌─────────┐
│  太郎   │
└─────────┘

という状態です。

その後、

print(name)

と書くと、

太郎

と表示されます。


---

変数を作る

Pythonでは、次のように変数を作ります。

変数名 = データ

例えば、

name = "太郎"
age = 15

と書けます。

ここでは、

name に "太郎"

age に 15


を入れています。


---

変数を表示する

変数に入れたデータは、print()で表示できます。

name = "太郎"

print(name)

実行結果：

太郎

数字も同じです。

age = 15

print(age)

実行結果：

15


---

変数の値を変更する

変数に入っているデータは変更できます。

age = 15

print(age)

age = 16

print(age)

実行結果：

15
16

最初は15でしたが、その後16を入れ直したので、値が変わりました。


---

変数を使って計算する

変数に数字を入れて計算することもできます。

a = 10
b = 20

print(a + b)

実行結果：

30

変数に入っている値を使って計算しています。


---

変数同士の計算

例えば、

price = 100
count = 3

total = price * count

print(total)

実行結果：

300

この場合、

price → 100
count → 3

なので、

100 × 3 = 300

となります。


---

変数名

変数には名前を付けます。

例えば、

name = "太郎"
age = 15
score = 80

のようにします。

変数名は、その変数に何が入っているのか分かりやすい名前にすると便利です。

例えば、

x = 15

よりも、

age = 15

のほうが意味が分かりやすくなります。


---

変数名の基本ルール

変数名にはいくつかルールがあります。

英字、数字、アンダースコアなどを使えます。

name = "太郎"
age = 15
user_name = "太郎"

ただし、数字から始めることはできません。

これは使えません。

1name = "太郎"

また、Pythonで特別な意味を持つ予約語を変数名として使うこともできません。


---

大文字と小文字

Pythonでは、大文字と小文字は区別されます。

例えば、

name = "太郎"
Name = "次郎"

この2つは別の変数です。

print(name)
print(Name)

実行結果：

太郎
次郎


---

変数のまとめ

変数は、データを名前を付けて保存しておくために使います。

name = "太郎"
age = 15

print(name)
print(age)

変数を使うことで、プログラムの中でデータを簡単に扱えるようになります。


---

11 数値

数値とは

Pythonでは、数字を使って計算できます。

例えば、

10

や、

3.14

などです。

Pythonでは、数値には主に次の種類があります。

整数

小数



---

整数

小数点がない数字を整数といいます。

例えば、

1
10
100
-5
0

などです。

Pythonでは整数をそのまま書けます。

age = 15

print(age)

実行結果：

15


---

小数

小数点を含む数字も扱えます。

price = 120.5

print(price)

実行結果：

120.5

例えば、

height = 170.5

のように使えます。


---

足し算

Pythonでは+を使って足し算ができます。

print(10 + 5)

実行結果：

15

変数も使えます。

a = 10
b = 5

print(a + b)

実行結果：

15


---

引き算

-を使うと引き算ができます。

print(10 - 5)

実行結果：

5


---

掛け算

*を使うと掛け算ができます。

print(10 * 5)

実行結果：

50


---

割り算

/を使うと割り算ができます。

print(10 / 2)

実行結果：

5.0

Pythonでは/を使った割り算の結果は、基本的に小数として扱われます。


---

整数の割り算

//を使うと、整数部分だけを求めることができます。

print(10 // 3)

実行結果：

3


---

余り

%を使うと、割り算の余りを求められます。

print(10 % 3)

実行結果：

1

10を3で割ると、

3 × 3 = 9

なので、余りは1です。


---

べき乗

**を使うと、べき乗を計算できます。

print(2 ** 3)

実行結果：

8

これは、

2 × 2 × 2

と同じです。


---

数値と変数

数値は変数に保存できます。

price = 100
count = 5

total = price * count

print(total)

実行結果：

500


---

数値のまとめ

Pythonでは、数値を使ってさまざまな計算ができます。

print(10 + 3)
print(10 - 3)
print(10 * 3)
print(10 / 3)
print(10 // 3)
print(10 % 3)
print(10 ** 3)


---

12 文字列

文字列とは

文字列とは、文字や文章を扱うためのデータです。

Pythonでは、文字列を"または'で囲みます。

"こんにちは"

または、

'こんにちは'

と書けます。


---

文字列を表示する

print("こんにちは")

実行結果：

こんにちは


---

文字列を変数に入れる

文字列を変数に保存できます。

name = "太郎"

print(name)

実行結果：

太郎


---

文字列をつなげる

文字列は+を使ってつなげられます。

first_name = "太郎"
message = "こんにちは、" + first_name

print(message)

実行結果：

こんにちは、太郎


---

文字列と文字列

a = "Hello"
b = "World"

print(a + b)

実行結果：

HelloWorld

間に空白を入れたい場合は、

print(a + " " + b)

とします。

実行結果：

Hello World


---

文字列と数値

文字列と数値は、そのまま+でつなぐことはできません。

例えば、

age = 15

print("年齢は" + age)

これはエラーになります。

数値を文字列に変換するにはstr()を使います。

age = 15

print("年齢は" + str(age))

実行結果：

年齢は15


---

f文字列

Pythonでは、変数を文章の中に入れる方法としてf文字列があります。

name = "太郎"
age = 15

print(f"{name}さんは{age}歳です")

実行結果：

太郎さんは15歳です

初心者のうちは、この書き方も覚えておくと便利です。


---

文字列の長さ

len()を使うと、文字列の長さを調べられます。

text = "Hello"

print(len(text))

実行結果：

5

日本語も文字数として数えられます。

text = "こんにちは"

print(len(text))

実行結果：

5


---

文字列のまとめ

文字列は、文字や文章を扱うためのデータです。

name = "太郎"
message = f"こんにちは、{name}さん"

print(message)

文字列は、名前や文章、メッセージなどを扱うときに使います。


---

13 True / False

TrueとFalseとは

Pythonには、TrueとFalseという特別な値があります。

これは、

True → 正しい・はい

False → 正しくない・いいえ


という意味で使われます。


---

True

print(True)

実行結果：

True


---

False

print(False)

実行結果：

False


---

変数に入れる

TrueやFalseも変数に保存できます。

is_student = True

print(is_student)

実行結果：

True

例えば、

is_login = False

のように、「ログインしているかどうか」を表すこともできます。


---

比較するとTrue / Falseになる

数字を比較すると、結果としてTrueまたはFalseが返ってきます。

print(10 > 5)

実行結果：

True

10は5より大きいのでTrueです。


---

print(10 < 5)

実行結果：

False

10は5より小さくないのでFalseです。


---

等しいか調べる

==を使うと、2つの値が等しいか調べられます。

print(10 == 10)

実行結果：

True


---

print(10 == 5)

実行結果：

False


---

等しくない

!=を使うと、等しくないかを調べられます。

print(10 != 5)

実行結果：

True


---

True / Falseを変数にする

age = 20

is_adult = age >= 18

print(is_adult)

実行結果：

True

このように、条件を調べた結果を変数に保存できます。


---

True / Falseのまとめ

TrueとFalseは、プログラムで「はい・いいえ」や「正しい・正しくない」を表すために使います。

is_login = True
is_admin = False

このデータは、後のif文などで非常に重要になります。


---

14 None

Noneとは

Noneは、「何もない」「値が存在しない」という状態を表す特別な値です。

x = None

print(x)

実行結果：

None


---

0とは違う

Noneは0とは違います。

x = 0

の場合は、

0という数値が入っている

という意味です。

一方、

x = None

の場合は、

値がない

という意味です。


---

空文字とも違う

Noneは空文字""とも違います。

x = ""

これは、

空の文字列

です。

一方、

x = None

は、

値が存在しない

という意味です。


---

Noneを使う例

例えば、まだ名前が決まっていない状態を表すことができます。

name = None

print(name)

実行結果：

None

後から値を入れることもできます。

name = None

name = "太郎"

print(name)

実行結果：

太郎


---

Noneを確認する

Noneかどうかを確認するときは、is Noneを使う書き方が一般的です。

name = None

print(name is None)

実行結果：

True

値が入っている場合は、

name = "太郎"

print(name is None)

実行結果：

False


---

Noneのまとめ

Noneは「値がない」という状態を表します。

data = None

0や""とは意味が違うことを覚えておきましょう。


---

15 型とtype()

データには型がある

Pythonで扱うデータには「型」があります。

型とは、

このデータは何の種類なのか

を表すものです。

例えば、

10

は数値です。

"Hello"

は文字列です。

True

はTrue / Falseを扱う型です。


---

type()とは

type()を使うと、データの型を確認できます。

print(type(10))

実行結果：

<class 'int'>

intは整数を表します。


---

文字列の型

print(type("Hello"))

実行結果：

<class 'str'>

strは文字列を表します。


---

小数の型

print(type(3.14))

実行結果：

<class 'float'>

floatは小数を表します。


---

Trueの型

print(type(True))

実行結果：

<class 'bool'>

boolはTrue / Falseを扱う型です。


---

Noneの型

print(type(None))

実行結果：

<class 'NoneType'>

Noneの型はNoneTypeです。


---

変数の型を調べる

変数に入っているデータの型も調べられます。

name = "太郎"

print(type(name))

実行結果：

<class 'str'>


---

age = 15

print(type(age))

実行結果：

<class 'int'>


---

height = 170.5

print(type(height))

実行結果：

<class 'float'>


---

is_student = True

print(type(is_student))

実行結果：

<class 'bool'>


---

主な型

このSTEPでは、まず次の型を覚えましょう。

型	意味	例

int	整数	10
float	小数	3.14
str	文字列	"Hello"
bool	True / False	True
NoneType	None	None



---

型を変換する

Pythonでは、データの型を変えることもできます。

例えば、文字列を整数に変換するにはint()を使います。

age = "15"

age = int(age)

print(age)

実行結果：

15

このとき、

print(type(age))

とすると、

<class 'int'>

になります。


---

数値を文字列に変換する

str()を使うと文字列に変換できます。

age = 15

text = str(age)

print(text)

実行結果：

15

型を確認すると、

print(type(text))

実行結果：

<class 'str'>


---

小数に変換する

float()を使うと、小数に変換できます。

number = "3.14"

number = float(number)

print(number)

実行結果：

3.14


---

型変換のまとめ

Pythonでは、次のような型変換ができます。

int("10")

整数になります。

float("3.14")

小数になります。

str(10)

文字列になります。


---

STEP 2 総まとめ

このSTEPでは、Pythonでデータを扱うための基本を学びました。

変数

データを名前を付けて保存できます。

name = "太郎"
age = 15


---

数値

整数や小数を扱えます。

age = 15
height = 170.5

計算もできます。

print(10 + 5)
print(10 - 5)
print(10 * 5)
print(10 / 5)


---

文字列

文字や文章を扱えます。

name = "太郎"

print(name)


---

True / False

正しい・間違っている、はい・いいえなどを表せます。

is_student = True
is_adult = False


---

None

「値がない」という状態を表します。

data = None


---

型

データには種類があります。

print(type(10))
print(type(3.14))
print(type("Hello"))
print(type(True))
print(type(None))


---

STEP 2で覚えておきたいこと

まずは次の内容を覚えられれば十分です。

name = "太郎"
age = 15
height = 170.5
is_student = True
data = None

それぞれ、

name       → 文字列
age        → 整数
height     → 小数
is_student → True / False
data       → None

というデータを持っています。

そして、type()を使えば、そのデータが何の型なのか確認できます。

print(type(name))
print(type(age))
print(type(height))
print(type(is_student))
print(type(data))

ここまで理解できれば、Pythonでデータを扱うための基本的な土台ができています。

次のSTEPでは、これらのデータを使って、さらにプログラムらしい処理を作っていきます。
