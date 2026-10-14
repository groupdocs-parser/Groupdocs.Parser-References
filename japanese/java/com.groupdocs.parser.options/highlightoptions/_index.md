---
title: "HighlightOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "検索シナリオで見つかったテキストの周囲のテキストブロックをハイライト抽出するために使用されるオプションを提供します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

検索シナリオで見つかったテキストの周囲のテキストブロック（ハイライト）を抽出するために使用されるオプションを提供します。

[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスのインスタンスは、[Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) メソッドのパラメーターとして使用されます。
そこにある使用例をご覧ください。

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | 制限が設定されていない状態で、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | 固定長のハイライトを抽出するために使用される、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | 行制限付きハイライトを抽出するために使用される、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | 固定語数のハイライトを抽出するために使用される、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | 最大テキスト長を取得します。 |
|
|  | [getWordCount()](#getWordCount--) | 最大語数を取得します。 |
|
|  | [isLineLimited()](#isLineLimited--) | ハイライト抽出がテキスト行の開始（または終了）で制限されているかどうかを示す値を取得します。 |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | 最大テキスト長を設定します。 |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | 最大単語数を設定します。 |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | ハイライト抽出がテキスト行の開始（または終了）で制限されるかどうかを示す値を設定します。 |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


制限が設定されていない状態で、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。パーサーに渡す前に、#setMaxLength(Integer).setMaxLength(Integer)、#setWordCount(Integer).setWordCount(Integer)、#setLineLimited(boolean).setLineLimited(boolean) のいずれかを少なくとも一つ設定してください。


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


固定長のハイライトを抽出するために使用される、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | maxLength | int | 最大テキスト長。 |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


行制限付きハイライトを抽出するために使用される、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 最大テキスト長。 |
|
|  | isLineLimited | boolean | ハイライト抽出がテキスト行の開始（または終了）で制限されるかどうかを示す値。 |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


固定語数のハイライトを抽出するために使用される、[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 最大テキスト長。 |
|
|  | wordCount | int | 最大単語数。 |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 最大テキスト長。 |
|
|  | wordCount | java.lang.Integer | 最大単語数。 |
|
|  | isLineLimited | boolean | ハイライト抽出がテキスト行の開始（または終了）で制限されるかどうかを示す値。 |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


最大テキスト長を取得します。


**Returns:**
java.lang.Integer - 最大テキスト長を表す正の整数値;  null  はテキスト長が制限されていない場合です。

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


最大語数を取得します。


**Returns:**
java.lang.Integer - 最大単語数を表す正の整数値;  null  は単語数が制限されていない場合です。

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


ハイライト抽出がテキスト行の開始（または終了）で制限されているかどうかを示す値を取得します。


**Returns:**
boolean -  true  はハイライト抽出がテキスト行の開始（または終了）で制限される場合;  false  はそれ以外の場合です。

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


最大テキスト長を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 負の値を取らない整数;  null  は長さの制限を解除するためです。 |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


最大単語数を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | 負の値を取らない整数;  null  は単語数の制限を解除するためです。 |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


ハイライト抽出がテキスト行の開始（または終了）で制限されるかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | lineLimited | boolean | true  は行の境界で制限することを意味します。 |
|

