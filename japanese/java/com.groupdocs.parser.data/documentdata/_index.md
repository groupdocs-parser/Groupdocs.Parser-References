---
title: "DocumentData"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ドキュメントのデータを表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

ドキュメントのデータを表します。ドキュメントからフィールドデータを含む [FieldData](../../com.groupdocs.parser.data/fielddata) オブジェクトで構成されています。[DocumentData](../../com.groupdocs.parser.data/documentdata) クラスのインスタンスは、[Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) および [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) メソッドの戻り値として使用されます。使用例をご覧ください。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | このドキュメントデータを生成したテンプレートを取得します。 |
|
|  | [getCount()](#getCount--) | フィールドデータの総数を取得します。 |
|
|  | [get(int index)](#get-int-) | インデックスでフィールドデータを取得します。 |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | 名前が fieldName と等しいフィールドデータのコレクションを返します。 |
|
|  | [iterator()](#iterator--) | このリストの要素を正しい順序で反復するイテレータを返します。 |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


このドキュメントデータを生成したテンプレートを取得します。

データが自動テンプレートコレクション選択によって生成された場合（参照
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
これは選択されたテンプレートです。
null
データがテンプレートによって生成されなかったとき。


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


フィールドデータの総数を取得します。


**Returns:**
int - フィールド データの総数を表す整数値。

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


インデックスでフィールドデータを取得します。

すべてのフィールドを反復処理:

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
[PageArea](../../com.groupdocs.parser.data/pagearea) クラスの継承者です。例えば、[Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) メソッドはテキストフィールドのみを抽出します:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | インデックス | int | フィールドのゼロベースインデックスです。 |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


名前が fieldName と等しいフィールドデータのコレクションを返します。

フィールド名でフィールドを検索:

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
[PageArea](../../com.groupdocs.parser.data/pagearea) クラスの継承者のいずれかです。例えば、[Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) メソッドはテキストフィールドのみを抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fieldName | java.lang.String | フィールドの名前です。 |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - [FieldData](../../com.groupdocs.parser.data/fielddata) オブジェクトのコレクションです。フィールドデータが見つからない場合は空のコレクションになります。

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


このリストの要素を正しい順序で反復するイテレータを返します。


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - このリスト内の要素を正しい順序で反復するイテレータです。

