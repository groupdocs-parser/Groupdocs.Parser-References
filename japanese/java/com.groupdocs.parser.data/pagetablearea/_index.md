---
title: "PageTableArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート解析機能でテーブルを表すために使用されるテーブルページ領域を表します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

テンプレート解析機能でテーブルを表すために使用されるテーブルページ領域を表します。

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 新しい [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCells()](#getCells--) | セルのコレクションを取得します。 |
|
|  | [getRowCount()](#getRowCount--) | テーブル行の総数を取得します。 |
|
|  | [getColumnCount()](#getColumnCount--) | テーブル列の総数を取得します。 |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | 行の高さを返します。 |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | 列の幅を返します。 |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | 行と列のインデックスでテーブルセルを取得します。 |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


新しい [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) クラスのインスタンスを初期化します。

注: C# プロジェクトではこのコンストラクタを次のようにマークしています
internal
(commit 954951f)。Java では "internal-to-the-assembly"
パッケージプライベートにきれいに翻訳できません。なぜならプロデューサー（
WordProcessingParser
,
TableAreaParser
,
etc.) にあります
com.groupdocs.parser
, ない
com.groupdocs.parser.data
. コンストラクタはそのため保持されます

public
そのため、クロスパッケージの構築がまだ機能します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 行 | java.lang.Iterable<java.lang.Double> | 行の高さのコレクションです。 |
|
|  | 列 | java.lang.Iterable<java.lang.Double> | 列の幅のコレクションです。 |
|
|  | セル | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | セルのコレクションです。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | テーブルを含むページです。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テーブルを含む矩形領域。 |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


セルのコレクションを取得します。テーブルセルの単純な読み取り専用コレクションです。


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - テーブルセルのコレクション

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


テーブル行の総数を取得します。


**Returns:**
int - テーブル行の総数を含む整数値です。

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


テーブル列の総数を取得します。


**Returns:**
int - テーブル列の総数を含む整数値です。

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


行の高さを返します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rowIndex | int | 行のゼロベースインデックスです。 |
|

**Returns:**
double - 行の高さを表す倍精度浮動小数点数です。

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


列の幅を返します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | columnIndex | int | 列のゼロベースインデックスです。 |
|

**Returns:**
double - 列の幅を表す倍精度浮動小数点数です。

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


行と列のインデックスでテーブルセルを取得します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rowIndex | int | セル行のゼロベースインデックスです。 |
|
|  | columnIndex | int | セル列のゼロベースインデックスです。 |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

