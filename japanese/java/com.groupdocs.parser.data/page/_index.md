---
title: "Page"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ページインデックスやページサイズなどのドキュメントページ情報を表します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

ページインデックスやページサイズなど、ドキュメントページ情報を表します。テンプレートによる解析機能で、[PageArea](../../com.groupdocs.parser.data/pagearea) クラスの継承者を含むページを表すために使用されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | [Page](../../com.groupdocs.parser.data/page) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getIndex()](#getIndex--) | ページインデックスを取得します。 |
|
|  | [getSize()](#getSize--) | ページサイズを取得します。 |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


[Page](../../com.groupdocs.parser.data/page) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | インデックス | int | ページインデックスです。 |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | ページサイズです。 |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


ページインデックスを取得します。


**Returns:**
int - ページのゼロベースインデックスです。

### getSize() {#getSize--}
```
public Size getSize()
```


ページサイズを取得します。


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

