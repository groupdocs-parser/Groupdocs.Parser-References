---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "OCRイベント用ハンドラを提供します。"
type: docs
weight: 26
url: /ja/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

OCRイベント用ハンドラを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | 警告メッセージのリストを取得します。 |
|
|  | [hasWarnings()](#hasWarnings--) | 警告リストが空でないかどうかを示す値を取得します。 |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | pageIndex を持つページの警告メッセージのリストを返します。 |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | ページの警告メッセージを設定します。 |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) クラスの新しいインスタンスを初期化します。


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


警告メッセージのリストを取得します。


**Returns:**
java.util.List<java.lang.String> - すべてのページの警告メッセージのリストです。

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


警告リストが空でないかどうかを示す値を取得します。


**Returns:**
boolean - 警告リストが空でない場合は true、そうでない場合は false。

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


pageIndex を持つページの警告メッセージのリストを返します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.util.List<java.lang.String> - ページの警告メッセージのリスト。警告メッセージがない場合は空のリストです。

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


ページの警告メッセージを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | warnings | java.lang.Iterable<java.lang.String> | ページの警告メッセージのリストです。 |
|

