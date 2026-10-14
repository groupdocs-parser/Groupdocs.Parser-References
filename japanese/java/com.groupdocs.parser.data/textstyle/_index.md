---
title: "TextStyle"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "フォント名やフォントサイズなど、テキストのスタイルを表します。"
type: docs
weight: 30
url: /ja/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

フォント名やフォントサイズなど、テキストのスタイルを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | [TextStyle](../../com.groupdocs.parser.data/textstyle) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getName()](#getName--) | スタイル名を取得します。 |
|
|  | [getFontName()](#getFontName--) | フォント名を取得します。 |
|
|  | [getFontSize()](#getFontSize--) | フォントサイズを取得します。 |
|
|  | [isBold()](#isBold--) | フォントが太字かどうかを示す値を取得します。 |
|
|  | [isItalic()](#isItalic--) | フォントが斜体かどうかを示す値を取得します。 |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


[TextStyle](../../com.groupdocs.parser.data/textstyle) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 名前 | java.lang.String | スタイルの名前です。 |
|
|  | fontName | java.lang.String | フォントの名前です。 |
|
|  | fontSize | double | フォントのサイズです。 |
|
|  | bold | boolean | フォントが太字かどうかを示す値です。 |
|
|  | italic | boolean | フォントが斜体かどうかを示す値です。 |
|

### getName() {#getName--}
```
public String getName()
```


スタイル名を取得します。


**Returns:**
java.lang.String - スタイル名を表す文字列値です。

### getFontName() {#getFontName--}
```
public String getFontName()
```


フォント名を取得します。


**Returns:**
java.lang.String - フォント名を表す文字列値です。

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


フォントサイズを取得します。


**Returns:**
double - フォントサイズを表す double 値です。

### isBold() {#isBold--}
```
public boolean isBold()
```


フォントが太字かどうかを示す値を取得します。


**Returns:**
boolean - フォントが太字の場合は true、そうでない場合は false です。

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


フォントが斜体かどうかを示す値を取得します。


**Returns:**
boolean - フォントが斜体の場合は true、そうでない場合は false です。

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
