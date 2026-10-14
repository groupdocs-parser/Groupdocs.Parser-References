---
title: "DocumentData"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Belgenin verilerini temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Belgenin verilerini temsil eder. Belgeden alan verilerini içeren [FieldData](../../com.groupdocs.parser.data/fielddata) nesnelerinden oluşur. [DocumentData](../../com.groupdocs.parser.data/documentdata) sınıfının bir örneği, [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) ve [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) yöntemlerinin dönüş değeri olarak kullanılır. Oradaki kullanım örneklerine bakın.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Bu belge verisini üreten şablonu alır. |
|
|  | [getCount()](#getCount--) | Alan verilerinin toplam sayısını alır. |
|
|  | [get(int index)](#get-int-) | Alan verisini bir indeksle alır. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Adı fieldName'e eşit olan alan verileri koleksiyonunu döndürür. |
|
|  | [iterator()](#iterator--) | Bu listedeki öğeler üzerinde doğru sırada bir yineleyici döndürür. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Bu belge verisini üreten şablonu alır.

Veri otomatik şablon-koleksiyon seçimiyle üretildiğinde (bkz
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
bu seçilen şablondur.
null
veri bir şablon tarafından üretilmediğinde.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Alan verilerinin toplam sayısını alır.


**Returns:**
int - Alan verilerinin toplam sayısını temsil eden bir tam sayı değeri.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Alan verisini bir indeksle alır.

Tüm alanlar üzerinden yineleme:

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
[PageArea](../../com.groupdocs.parser.data/pagearea) sınıfının türevleri. Örneğin, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) yöntemi yalnızca metin alanlarını çıkarır:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Alanının sıfır tabanlı indeksi. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Adı fieldName'e eşit olan alan verileri koleksiyonunu döndürür.

Alanları bir alan adıyla bulun:

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
[PageArea](../../com.groupdocs.parser.data/pagearea) sınıfının herhangi bir türevi. Örneğin, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) yöntemi yalnızca metin alanlarını çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fieldName | java.lang.String | Alanının adı. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - [FieldData](../../com.groupdocs.parser.data/fielddata) nesnelerinin bir koleksiyonu; alan verisi bulunamazsa boş koleksiyon.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Bu listedeki öğeler üzerinde doğru sırada bir yineleyici döndürür.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - bu listedeki öğeler üzerinde doğru sırada bir yineleyici.

