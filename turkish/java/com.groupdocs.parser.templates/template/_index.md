---
title: "Şablon"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Belge sayfa şablonunu sağlar."
type: docs
weight: 10
url: /tr/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Belge sayfa şablonunu sağlar. Şablonun metin alanı ve tablo tanımları gibi öğelerini temsil eden [TemplateItem](../../com.groupdocs.parser.templates/templateitem) nesnelerinden oluşur.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Yeni bir [Template](../../com.groupdocs.parser.templates/template) sınıfı örneği başlatır. |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Yeni bir [Template](../../com.groupdocs.parser.templates/template) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | Şablon öğelerinin toplam sayısını alır. |
|
|  | [get(int index)](#get-int-) | Şablon öğesini bir dizine göre alır. |
|
|  | [getOptions()](#getOptions--) | Şablon seçeneklerini alır. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Bir dosyadan şablon yükler. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Bir akıştan şablon yükler. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Şablonu bir dosyaya kaydeder. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Şablonu bir akışa kaydeder. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Yeni bir [Template](../../com.groupdocs.parser.templates/template) sınıfı örneği başlatır.

Kullanım:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) nesnelerinin koleksiyonu. |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Yeni bir [Template](../../com.groupdocs.parser.templates/template) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) nesnelerinin koleksiyonu. |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Şablon seçenekleri. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Şablon öğelerinin toplam sayısını alır.


**Returns:**
int - Şablon öğelerinin toplam sayısını temsil eden bir tamsayı.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Şablon öğesini bir dizine göre alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Şablon öğesinin sıfır tabanlı indeksi. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Şablon seçeneklerini alır.


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


Bir dosyadan şablon yükler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Bir akıştan şablon yükler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.InputStream | Girdi akışı. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Şablonu bir dosyaya kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Şablonu bir akışa kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Çıktı akışı. |
|

