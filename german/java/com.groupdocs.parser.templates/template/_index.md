---
title: "Template"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Dokumentenseitenvorlage bereit."
type: docs
weight: 10
url: /de/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Stellt die Dokumentenseitenvorlage bereit. Sie besteht aus [TemplateItem](../../com.groupdocs.parser.templates/templateitem)-Objekten, die die Elemente der Vorlage wie Textfelder und Tabellendefinitionen repräsentieren.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Initialisiert eine neue Instanz der Klasse [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Initialisiert eine neue Instanz der Klasse [Template](../../com.groupdocs.parser.templates/template). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Liefert die Gesamtzahl der Vorlagenelemente. |
|
|  | [get(int index)](#get-int-) | Liefert das Vorlagenelement anhand eines Index. |
|
|  | [getOptions()](#getOptions--) | Liefert die Vorlagenoptionen. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Lädt eine Vorlage aus einer Datei. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Lädt eine Vorlage aus einem Stream. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Speichert eine Vorlage in einer Datei. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Speichert eine Vorlage in einen Stream. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Initialisiert eine neue Instanz der Klasse [Template](../../com.groupdocs.parser.templates/template).

Verwendung:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Die Sammlung von [TemplateItem](../../com.groupdocs.parser.templates/templateitem)-Objekten. |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Initialisiert eine neue Instanz der Klasse [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Die Sammlung von [TemplateItem](../../com.groupdocs.parser.templates/templateitem)-Objekten. |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Die Vorlagenoptionen. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Liefert die Gesamtzahl der Vorlagenelemente.


**Returns:**
int - Eine Ganzzahl, die die Gesamtzahl der Vorlagenobjekte darstellt.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Liefert das Vorlagenelement anhand eines Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der nullbasierte Index des Vorlagenobjekts. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Liefert die Vorlagenoptionen.


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


Lädt eine Vorlage aus einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Lädt eine Vorlage aus einem Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.InputStream | Der Eingabestream. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Speichert eine Vorlage in einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Speichert eine Vorlage in einen Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Der Ausgabestream. |
|

