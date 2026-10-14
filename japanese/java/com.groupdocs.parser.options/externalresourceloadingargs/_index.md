---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "メソッドのデータを提供します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

[ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) メソッドのデータを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | 矩形領域で [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getUri()](#getUri--) | 外部リソースの URI を取得します。 |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | 外部リソースの URI を取得します。 |
|
|  | [isSkipped()](#isSkipped--) | 外部リソースの読み込みをスキップすべきかどうかを示す値を取得します。 |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | 外部リソースの読み込みをスキップすべきかどうかを示す値を設定します。 |
|
|  | [getData()](#getData--) | ユーザーデータを取得します。 |
|
|  | [setData(byte[] data)](#setData-byte---) | ユーザーデータを設定します。 |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


矩形領域で [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | uri | java.lang.String | 外部リソースの URI。 |
|

### getUri() {#getUri--}
```
public String getUri()
```


外部リソースの URI を取得します。


**Returns:**
java.lang.String - 外部リソースの URI を表す文字列値。

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


外部リソースの URI を取得します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | uri | java.lang.String | 外部リソースの新しい URI を表す文字列値。 |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


外部リソースの読み込みをスキップすべきかどうかを示す値を取得します。


**Returns:**
boolean - 外部リソースの読み込みをスキップすべき場合は true、そうでない場合は false。

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


外部リソースの読み込みをスキップすべきかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | skipped | boolean | 外部リソースの読み込みをスキップすべき場合は true、そうでない場合は false。 |
|

### getData() {#getData--}
```
public byte[] getData()
```


ユーザーデータを取得します。


**Returns:**
byte[] - 外部リソースのユーザーコンテンツを含むバイト配列。設定されていない場合は null。

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


ユーザーデータを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | データ | byte[] | 外部リソースのユーザーコンテンツを含むバイト配列。設定されていない場合は null。 |
|

