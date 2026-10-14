---
title: "DocumentData"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar dokumentets data."
type: docs
weight: 11
url: /sv/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Representerar data för dokumentet. Det består av [FieldData](../../com.groupdocs.parser.data/fielddata) objekt som innehåller fältdata från dokumentet. En instans av klassen [DocumentData](../../com.groupdocs.parser.data/documentdata) används som returvärde för metoderna [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) och [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . Se användningsexemplen där.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Hämtar mallen som producerade dessa dokumentdata. |
|
|  | [getCount()](#getCount--) | Hämtar det totala antalet fältdata. |
|
|  | [get(int index)](#get-int-) | Hämtar fältdata efter ett index. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Returnerar samlingen av fältdata där namnet är lika med fieldName. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator över elementen i denna lista i korrekt ordning. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Hämtar mallen som producerade dessa dokumentdata.

När data producerades av ett automatiskt urval av mallsamling (se
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
detta är den valda mallen.
null
när data inte producerades av en mall.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Hämtar det totala antalet fältdata.


**Returns:**
int - Ett heltalsvärde som representerar det totala antalet fältdata.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Hämtar fältdata efter ett index.

Iteration över alla fält:

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
av ärvda klasser till [PageArea](../../com.groupdocs.parser.data/pagearea). Till exempel extraherar metoden [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) endast textfält:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Det nollbaserade indexet för fältet. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Returnerar samlingen av fältdata där namnet är lika med fieldName.

Hitta fält efter ett fältnamn:

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
vilken som helst av ärvda klasser till [PageArea](../../com.groupdocs.parser.data/pagearea). Till exempel extraherar metoden [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) endast textfält.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fieldName | java.lang.String | Namnet på fältet. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - En samling av [FieldData](../../com.groupdocs.parser.data/fielddata)-objekt; tom samling om ingen fältdata hittas.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Returnerar en iterator över elementen i denna lista i korrekt ordning.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - en iterator över elementen i denna lista i korrekt ordning.

