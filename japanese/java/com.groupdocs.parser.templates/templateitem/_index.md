---
title: "TemplateItem"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート項目の基底抽象クラスを提供します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

テンプレート項目の基底抽象クラスを提供します。

継承クラスである [TemplateItem](../../com.groupdocs.parser.templates/templateitem) は、[Template](../../com.groupdocs.parser.templates/template) コレクションで使用されます。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | 指定された係数で全座標をスケーリングした、現在の項目のコピーを作成します。 |
|
|  | [getName()](#getName--) | テンプレート項目の名前を取得します。 |
|
|  | [getPageIndex()](#getPageIndex--) | テンプレート項目のページインデックスを取得します。 |
|
|  | [getPageWidth()](#getPageWidth--) | テンプレート項目の作成に使用されたページの幅を取得します。 |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | 名前が大文字に変換されたかどうかを示す値を取得します。 |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


指定された係数で全座標をスケーリングした、現在の項目のコピーを作成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | factor | double | スケーリング係数です。 |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


テンプレート項目の名前を取得します。


**Returns:**
java.lang.String - テンプレート項目の名前を表す大文字の文字列です。

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


テンプレート項目のページインデックスを取得します。


**Returns:**
java.lang.Integer - テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページに配置されている場合は  null  です。

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


テンプレート項目の作成に使用されたページの幅を取得します。


**Returns:**
java.lang.Double - ページの幅（ピクセル単位）です。ページ幅が不明な場合は  null  です。

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


名前が大文字に変換されたかどうかを示す値を取得します。


**Returns:**
boolean - 名前が大文字に変換されたかどうかを示すブール値です。

