---
title: "TextReader"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "文字のシーケンシャルな系列を読み取ることができるリーダーを表します。"
type: docs
weight: 29
url: /ja/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

文字のシーケンシャルな系列を読み取ることができるリーダーを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | テキストリーダーから文字列の行を読み取り、データを文字列として返します。 |
|
|  | [readToEnd()](#readToEnd--) | 現在位置からテキストリーダーの末尾までのすべての文字を読み取り、1つの文字列として返します。 |
|
|  | [dispose()](#dispose--) | [TextReader](../../com.groupdocs.parser.data/textreader) オブジェクトが使用するすべてのリソースを解放します。 |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


テキストリーダーから文字列の行を読み取り、データを文字列として返します。


**Returns:**
java.lang.String - リーダーからの次の行、またはすべての文字が読み取られた場合は  null  です。

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


現在位置からテキストリーダーの末尾までのすべての文字を読み取り、1つの文字列として返します。


**Returns:**
java.lang.String - 現在位置からテキストリーダーの末尾までのすべての文字を含む文字列です。

### dispose() {#dispose--}
```
public void dispose()
```


[TextReader](../../com.groupdocs.parser.data/textreader) オブジェクトが使用するすべてのリソースを解放します。


