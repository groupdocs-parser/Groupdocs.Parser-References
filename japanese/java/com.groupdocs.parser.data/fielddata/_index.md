---
title: "FieldData"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "名前、ページインデックス、フィールド値などのフィールドデータを表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

名前、ページインデックス、フィールド値などのフィールドデータを表します。フィールドによっては、値がテキスト、画像、テーブルなどになることがあります。

[FieldData](../../com.groupdocs.parser.data/fielddata) クラスのインスタンスは、[DocumentData](../../com.groupdocs.parser.data/documentdata) コレクションで使用されます。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getName()](#getName--) | フィールド名を取得します。 |
|
|  | [getPageIndex()](#getPageIndex--) | ページインデックスを取得します。 |
|
|  | [getPageArea()](#getPageArea--) | フィールドの値を取得します。 |
|
|  | [getLinkedField()](#getLinkedField--) | リンクされたフィールドを取得します。 |
|
|  | [getText()](#getText--) | テキストを取得します。 |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | 名前が大文字に変換されたかどうかを示す値を取得します。 |
|
### getName() {#getName--}
```
public String getName()
```


フィールド名を取得します。


**Returns:**
java.lang.String - フィールド名を表す大文字の文字列値です。

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


ページインデックスを取得します。


**Returns:**
int - フィールドが含まれるページのゼロベースインデックスです。

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


フィールドの値を取得します。

フィールドの PageArea プロパティは、[PageArea](../../com.groupdocs.parser.data/pagearea) クラスの継承クラスのいずれかを含む場合があります。
例えば、[Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) メソッドはテキストフィールドのみを抽出します。

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


リンクされたフィールドを取得します。


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


テキストを取得します。


**Returns:**
java.lang.String - フィールドテキストの値を表す文字列です。 [PageArea](../../com.groupdocs.parser.data/pagearea) プロパティが [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) でない場合は null です。

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


名前が大文字に変換されたかどうかを示す値を取得します。


**Returns:**
boolean - 名前が大文字に変換されたかどうかを示すブール値です。

