---
title: "DocumentData"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt Daten des Dokuments dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Stellt Daten des Dokuments dar. Es besteht aus [FieldData](../../com.groupdocs.parser.data/fielddata)-Objekten, die Felddaten aus dem Dokument enthalten. Eine Instanz der Klasse [DocumentData](../../com.groupdocs.parser.data/documentdata) wird als Rückgabewert der Methoden [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) und [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) verwendet. Siehe dort die Anwendungsbeispiele.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Liefert die Vorlage, die diese Dokumentdaten erzeugt hat. |
|
|  | [getCount()](#getCount--) | Liefert die Gesamtzahl der Felddaten. |
|
|  | [get(int index)](#get-int-) | Liefert die Felddaten anhand eines Index. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Gibt die Sammlung von Felddaten zurück, bei denen der Name gleich  fieldName  ist. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator über die Elemente dieser Liste in korrekter Reihenfolge zurück. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Liefert die Vorlage, die diese Dokumentdaten erzeugt hat.

Wenn die Daten durch eine automatische Auswahl von Vorlagen‑Sammlungen erzeugt wurden (siehe
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
dies ist die ausgewählte Vorlage.
null
wenn die Daten nicht durch eine Vorlage erzeugt wurden.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Liefert die Gesamtzahl der Felddaten.


**Returns:**
int - Ein ganzzahliger Wert, der die Gesamtzahl der Felddaten darstellt.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Liefert die Felddaten anhand eines Index.

Iteration über alle Felder:

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
der Erben der Klasse [PageArea](../../com.groupdocs.parser.data/pagearea). Zum Beispiel extrahiert die Methode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) nur Textfelder:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der nullbasierte Index des Feldes. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Gibt die Sammlung von Felddaten zurück, bei denen der Name gleich  fieldName  ist.

Felder nach einem Feldnamen suchen:

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
irgendeiner der Erben der Klasse [PageArea](../../com.groupdocs.parser.data/pagearea). Zum Beispiel extrahiert die Methode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) nur Textfelder.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fieldName | java.lang.String | Der Name des Feldes. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Eine Sammlung von [FieldData](../../com.groupdocs.parser.data/fielddata)-Objekten; leere Sammlung, wenn keine Felddaten gefunden werden.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Gibt einen Iterator über die Elemente dieser Liste in korrekter Reihenfolge zurück.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - Ein Iterator über die Elemente in dieser Liste in korrekter Reihenfolge.

