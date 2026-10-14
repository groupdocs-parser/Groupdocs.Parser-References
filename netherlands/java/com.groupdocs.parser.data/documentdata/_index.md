---
title: "DocumentData"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de gegevens van het document voor."
type: docs
weight: 11
url: /nl/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Stelt de gegevens van het document voor. Het bestaat uit [FieldData](../../com.groupdocs.parser.data/fielddata) objecten die veldgegevens uit het document bevatten. Een instantie van de [DocumentData](../../com.groupdocs.parser.data/documentdata) klasse wordt gebruikt als retourwaarde van de [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) en [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) methoden. Zie de gebruiksvoorbeelden daar.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Haalt de sjabloon op die deze documentgegevens heeft geproduceerd. |
|
|  | [getCount()](#getCount--) | Haalt het totale aantal veldgegevens op. |
|
|  | [get(int index)](#get-int-) | Haalt de veldgegevens op via een index. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Retourneert de collectie veldgegevens waarbij de naam gelijk is aan  fieldName . |
|
|  | [iterator()](#iterator--) | Retourneert een iterator over de elementen in deze lijst in de juiste volgorde. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Haalt de sjabloon op die deze documentgegevens heeft geproduceerd.

Wanneer de gegevens werden geproduceerd door een automatische sjabloonverzamelingsselectie (zie
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
dit is het geselecteerde sjabloon.
null
wanneer de gegevens niet werden geproduceerd door een sjabloon.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Haalt het totale aantal veldgegevens op.


**Returns:**
int - Een gehele waarde die het totale aantal veldgegevens vertegenwoordigt.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Haalt de veldgegevens op via een index.

Iteratie over alle velden:

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
van de afstammelingen van de klasse [PageArea](../../com.groupdocs.parser.data/pagearea). Bijvoorbeeld, de methode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extraheert alleen tekstvelden:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De nulgebaseerde index van het veld. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Retourneert de collectie veldgegevens waarbij de naam gelijk is aan  fieldName .

Zoek velden op een veldnaam:

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
een van de afstammelingen van de klasse [PageArea](../../com.groupdocs.parser.data/pagearea). Bijvoorbeeld, de methode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extraheert alleen tekstvelden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fieldName | java.lang.String | De naam van het veld. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Een collectie van [FieldData](../../com.groupdocs.parser.data/fielddata) objecten; lege collectie als er geen veldgegevens worden gevonden.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Retourneert een iterator over de elementen in deze lijst in de juiste volgorde.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - een iterator over de elementen in deze lijst in de juiste volgorde.

