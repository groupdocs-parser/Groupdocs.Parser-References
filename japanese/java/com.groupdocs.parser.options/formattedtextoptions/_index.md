---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "書式付きテキスト抽出に使用されるオプションを提供します。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

書式付きテキスト抽出に使用されるオプションを提供します。

インスタンス [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) クラスは、[Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-) のパラメータとして使用されます。
および [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) メソッド。使用例はそちらをご覧ください。

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | モードが設定されていない状態で、[FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getMode()](#getMode--) | 書式付きテキスト抽出モードを取得します。 |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | 書式付きテキスト抽出モードを設定します。 |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


モードが設定されていない状態で、[FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) クラスの新しいインスタンスを初期化します。


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


[FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | 書式化テキスト抽出のモードです。 |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


書式付きテキスト抽出モードを取得します。


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


書式付きテキスト抽出モードを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) 列挙体は、書式化テキスト抽出モードを含みます。 |
|

