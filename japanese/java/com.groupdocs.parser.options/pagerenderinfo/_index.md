---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ページがどのようにレンダリングされるかの情報を表します。"
type: docs
weight: 30
url: /ja/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

ページがどのようにレンダリングされるかの情報を表します。

一部のドキュメント（例としてスプレッドシート）は、ページをレンダリングできません。
単一の画像としてです。これらのドキュメントでは、ページがタイルの集合としてレンダリングされます。
これらのタイルは矩形テーブルに配置されます。


RowCount
と
ColumnCount
行と列の総数を表します
このテーブルのものです。ドキュメントページが単一画像にレンダリングされる場合、これらのプロパティは 1 になります。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | 新しい [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | ページ番号を取得します。 |
|
|  | [getRowCount()](#getRowCount--) | タイル行の総数を取得します。 |
|
|  | [getColumnCount()](#getColumnCount--) | タイル列の総数を取得します。 |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | tileIndex を持つタイルが配置されている列のインデックスを返します。 |
|
|  | [getRow(int tileIndex)](#getRow-int-) | tileIndex を持つタイルが配置されている行のインデックスを返します。 |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


新しい [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageNumber | int | ページ番号 (1 から開始) です。 |
|
|  | rowCount | int | タイル行の総数です。 |
|
|  | columnCount | int | タイル列の総数です。 |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


ページ番号を取得します。


**Returns:**
int - ページ番号を表す整数値です (1 から開始)。

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


タイル行の総数を取得します。


**Returns:**
int - タイル行の総数を表す整数値です。

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


タイル列の総数を取得します。


**Returns:**
int - タイル列の総数を表す整数値です。

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


tileIndex を持つタイルが配置されている列のインデックスを返します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | tileIndex | int | タイルのゼロベースインデックスです。 |
|

**Returns:**
int - 列インデックスを表すゼロベースの整数値です。

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


tileIndex を持つタイルが配置されている行のインデックスを返します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | tileIndex | int | タイルのゼロベースインデックスです。 |
|

**Returns:**
int - 行インデックスを表すゼロベースの整数値です。

