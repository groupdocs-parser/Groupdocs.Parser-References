---
title: "Template"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ドキュメントページテンプレートを提供します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

ドキュメントページのテンプレートを提供します。これは、テキストフィールドやテーブル定義など、テンプレートの項目を表す [TemplateItem](../../com.groupdocs.parser.templates/templateitem) オブジェクトで構成されています。

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | 新しい [Template](../../com.groupdocs.parser.templates/template) クラスのインスタンスを初期化します。 |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | 新しい [Template](../../com.groupdocs.parser.templates/template) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | テンプレート項目の総数を取得します。 |
|
|  | [get(int index)](#get-int-) | インデックスでテンプレート項目を取得します。 |
|
|  | [getOptions()](#getOptions--) | テンプレートオプションを取得します。 |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | ファイルからテンプレートをロードします。 |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | ストリームからテンプレートをロードします。 |
|
|  | [save(String filePath)](#save-java.lang.String-) | テンプレートをファイルに保存します。 |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | テンプレートをストリームに保存します。 |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


新しい [Template](../../com.groupdocs.parser.templates/template) クラスのインスタンスを初期化します。

使用方法:

````
// Create an array of template fields
 TemplateItem[] fields = new TemplateItem[]
 {
     new TemplateField(new TemplateRegexPosition("From"), "From", 0),
     new TemplateField(
         new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromCompany",
         0),
     new TemplateField(
         new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromAddress",
         0)
 };
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) オブジェクトのコレクションです。 |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


新しい [Template](../../com.groupdocs.parser.templates/template) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) オブジェクトのコレクションです。 |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | テンプレートオプションです。 |
|

### getCount() {#getCount--}
```
public int getCount()
```


テンプレート項目の総数を取得します。


**Returns:**
int - テンプレート項目の総数を表す整数です。

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


インデックスでテンプレート項目を取得します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | インデックス | int | テンプレート項目のゼロベースインデックスです。 |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


テンプレートオプションを取得します。


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


ファイルからテンプレートをロードします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


ストリームからテンプレートをロードします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 入力ストリームです。 |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


テンプレートをファイルに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


テンプレートをストリームに保存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | stream | java.io.OutputStream | 出力ストリーム。 |
|

