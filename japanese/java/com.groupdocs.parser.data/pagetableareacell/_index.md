---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "クラスで使用されるテーブルセルを表します。"
type: docs
weight: 23
url: /ja/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

クラス [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) で使用されるテーブルセルを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | 行インデックスを取得します。 |
|
|  | [getColumnIndex()](#getColumnIndex--) | 列インデックスを取得します。 |
|
|  | [getRowSpan()](#getRowSpan--) | テーブルセルを含む行の総数を取得します。 |
|
|  | [getColumnSpan()](#getColumnSpan--) | テーブルセルを含む列の総数を取得します。 |
|
|  | [getPageArea()](#getPageArea--) | テーブルセルの値を取得します。 |
|
|  | [getText()](#getText--) | テーブルセルのテキスト値を取得します。 |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rowIndex | int | 行のゼロベースインデックスです。 |
|
|  | columnIndex | int | 列のゼロベースインデックスです。 |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | テーブルセルの値です。 |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rowIndex | int | 行のゼロベースインデックスです。 |
|
|  | columnIndex | int | 列のゼロベースインデックスです。 |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | テーブルセルの値です。 |
|
|  | rowSpan | int | テーブルセルを含む行の総数です。 |
|
|  | columnSpan | int | テーブルセルを含む列の総数です。 |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


行インデックスを取得します。


**Returns:**
int - テーブルセルを含む最初の行のゼロベースインデックスです。

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


列インデックスを取得します。


**Returns:**
int - テーブルセルを含む最初の列のゼロベースインデックスです。

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


テーブルセルを含む行の総数を取得します。


**Returns:**
int - テーブルセルを含む行の総数を表す正の整数値です。

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


テーブルセルを含む列の総数を取得します。


**Returns:**
int - テーブルセルを含む列の総数を表す正の整数値です。

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


テーブルセルの値を取得します。


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


テーブルセルのテキスト値を取得します。


**Returns:**
java.lang.String - セルのテキスト値を表す文字列です。セルがテキスト値を含まない場合は null です。

