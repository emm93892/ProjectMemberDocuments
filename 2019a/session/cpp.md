# C++勉強会資料

## C++とは

## namespace

名前空間のこと。JavaでいうところのPackage。<br/>
複数人で開発を行うとき、同じクラス名の衝突を避けるためにある。

### std名前空間

C++で提供されるクラスライブラリは全てstd名前空間に属する。<br/>
そのため、単純にincludeしただけでは使用することができず、下で説明する`using句`を使用するか、使用するクラスがstdに属することを明示しなければいけない。

### using句

`using namespace [名前空間名]`を使用することで、宣言されたブロック内で、その名前空間に属するクラスを使用することができるようになる。<br/>
ただし、ここで注意しなければならないのは、`using namespace`によって、そのブロックが名前空間に汚染されるという事である。<br/>
入門書/入門サイトなどでは、コードブロック外(グローバル名前空間と呼ぶ)で`using namespace`が宣言されており、このソースファイルをincludeすると、`using namespace`をしなくてもその名前空間に属するクラスを使用することができるようになってしまう。

## ポインタと参照

```cpp
int number = 100;
int *pnumber = &number;   // ポインタ
int &rnumber = number;    // 参照
```

## template

## STL

STL(Standard Template Library)とは、C++で標準で用意されている、テンプレートを用いて様々な型に対応したコンテナのことである。

* std::vector\<T>
* std::map\<K,V>

### std::vector\<T>

可変長配列。

### std::map\<K,V>

辞書。

## 継承

## 仮想関数

## 純粋仮想関数

## constとconstexpr

## Lambda

