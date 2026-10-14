---
title: "TemplateTable"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレートテーブルを提供します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

テンプレートテーブルを提供します。

テーブルを定義する方法は2つあります：

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | 大文字の名前で [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | 大文字の名前で [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | 大文字の名前で [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getLayout()](#getLayout--) | テーブルのレイアウトを取得します。 |
|
|  | [getParameters()](#getParameters--) | 自動モードでテーブルを検出するためのパラメータを取得します。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


大文字の名前で [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。

テーブルが自動的に検出できない場合、テンプレートテーブルはテーブルレイアウトで設定されます:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | テーブルレイアウト。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


大文字の名前で [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | テーブルレイアウト。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | テーブルレイアウト。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | テーブルレイアウト。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


大文字の名前で [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。

検出器パラメータでテンプレートテーブルが設定されている場合、テーブルは自動的に検出されます:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 自動モードでテーブルを検出するためのパラメータ。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 自動モードでテーブルを検出するためのパラメータ。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 自動モードでテーブルを検出するためのパラメータ。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | 自動モードでテーブルを検出するためのパラメータ。 |
|
|  | 名前 | java.lang.String | テーブル名。 |
|
|  | pageIndex | java.lang.Integer | テンプレートテーブルが配置されているページのインデックス; テンプレートテーブルが任意のページにある場合は null。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


テーブルのレイアウトを取得します。


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


自動モードでテーブルを検出するためのパラメータを取得します。


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


指定された係数で全座標をスケーリングした、現在の項目のコピーを作成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
