---
title: "Mall"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller mall för dokumentsida."
type: docs
weight: 10
url: /sv/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Tillhandahåller dokumentsidans mall. Den består av [TemplateItem](../../com.groupdocs.parser.templates/templateitem)-objekt som representerar mallens element, såsom textfält och tabelldefinitioner.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Initierar en ny instans av klassen [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Initierar en ny instans av klassen [Template](../../com.groupdocs.parser.templates/template). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar det totala antalet mallobjekt. |
|
|  | [get(int index)](#get-int-) | Hämtar mallobjektet efter ett index. |
|
|  | [getOptions()](#getOptions--) | Hämtar mallalternativen. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Läser in en mall från en fil. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Läser in en mall från en ström. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Sparar en mall till en fil. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Sparar en mall till en ström. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Initierar en ny instans av klassen [Template](../../com.groupdocs.parser.templates/template).

Användning:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Samlingen av [TemplateItem](../../com.groupdocs.parser.templates/templateitem)-objekt. |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Initierar en ny instans av klassen [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Samlingen av [TemplateItem](../../com.groupdocs.parser.templates/templateitem)-objekt. |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Mallalternativen. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Hämtar det totala antalet mallobjekt.


**Returns:**
int - Ett heltal som representerar det totala antalet mallobjekt.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Hämtar mallobjektet efter ett index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Det nollbaserade indexet för mallobjektet. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Hämtar mallalternativen.


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


Läser in en mall från en fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Läser in en mall från en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | stream | java.io.InputStream | Inmatningsströmmen. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Sparar en mall till en fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Sparar en mall till en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Utdataströmmen. |
|

