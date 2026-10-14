---
title: "Template"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de sjabloon voor de documentpagina."
type: docs
weight: 10
url: /nl/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Biedt de sjabloon voor de documentpagina. Het bestaat uit [TemplateItem](../../com.groupdocs.parser/templates/templateitem) objecten die de items van het sjabloon vertegenwoordigen, zoals tekstvelden en tabeldefinities.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Initialiseert een nieuw exemplaar van de [Template](../../com.groupdocs.parser.templates/template) klasse. |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Initialiseert een nieuw exemplaar van de [Template](../../com.groupdocs.parser.templates/template) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het totale aantal sjabloonitems op. |
|
|  | [get(int index)](#get-int-) | Haalt het sjabloonitem op via een index. |
|
|  | [getOptions()](#getOptions--) | Haalt de sjabloonopties op. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Laadt een sjabloon vanuit een bestand. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Laadt een sjabloon vanuit een stream. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Slaat een sjabloon op in een bestand. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Slaat een sjabloon op in een stream. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Initialiseert een nieuw exemplaar van de [Template](../../com.groupdocs.parser.templates/template) klasse.

Gebruik:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | De collectie van [TemplateItem](../../com.groupdocs.parser.templates/templateitem) objecten. |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Initialiseert een nieuw exemplaar van de [Template](../../com.groupdocs.parser.templates/template) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | De collectie van [TemplateItem](../../com.groupdocs.parser.templates/templateitem) objecten. |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | De sjabloonopties. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Haalt het totale aantal sjabloonitems op.


**Returns:**
int - Een geheel getal dat het totale aantal sjabloonitems weergeeft.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Haalt het sjabloonitem op via een index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De nulgebaseerde index van het sjabloonitem. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Haalt de sjabloonopties op.


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


Laadt een sjabloon vanuit een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Laadt een sjabloon vanuit een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.InputStream | De invoerstream. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Slaat een sjabloon op in een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Slaat een sjabloon op in een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.OutputStream | De uitvoerstream. |
|

