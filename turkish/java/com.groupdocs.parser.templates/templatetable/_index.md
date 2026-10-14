---
title: "TemplateTable"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon tablosunu sağlar."
type: docs
weight: 20
url: /tr/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Şablon tablosunu sağlar.

Bir tablo tanımlamanın iki yolu vardır:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | UPPER CASE adıyla [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | UPPER CASE adıyla [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | UPPER CASE adıyla [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getLayout()](#getLayout--) | Tablonun düzenini alır. |
|
|  | [getParameters()](#getParameters--) | Tabloyu otomatik modda tespit etmek için parametreleri alır. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


UPPER CASE adıyla [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.

Tablo otomatik olarak tespit edilemezse, şablon tablo tablo düzeniyle ayarlanır:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tablo düzeni. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


UPPER CASE adıyla [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tablo düzeni. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tablo düzeni. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tablo düzeni. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


UPPER CASE adıyla [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.

Bir şablon tablo algılayıcı parametreleriyle ayarlanmışsa, tablo otomatik olarak tespit edilir:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Tabloyu otomatik modda tespit etmek için parametreler. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Tabloyu otomatik modda tespit etmek için parametreler. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Tabloyu otomatik modda tespit etmek için parametreler. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


[TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Tabloyu otomatik modda tespit etmek için parametreler. |
|
|  | ad | java.lang.String | Tablo adı. |
|
|  | pageIndex | java.lang.Integer | Şablon tablonun bulunduğu sayfanın indeksi; şablon tablo herhangi bir sayfada bulunuyorsa  null  olur. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Tablonun düzenini alır.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Tabloyu otomatik modda tespit etmek için parametreleri alır.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Mevcut öğenin bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirerek oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| faktör | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
