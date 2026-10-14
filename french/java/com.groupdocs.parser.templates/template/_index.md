---
title: "Modèle"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit le modèle de page de document."
type: docs
weight: 10
url: /fr/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Fournit le modèle de page de document. Il se compose d'objets [TemplateItem](../../com.groupdocs.parser.templates/templateitem) qui représentent les éléments du modèle tels que les champs de texte et les définitions de tableau.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Initialise une nouvelle instance de la classe [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Initialise une nouvelle instance de la classe [Template](../../com.groupdocs.parser.templates/template). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre total d'éléments du modèle. |
|
|  | [get(int index)](#get-int-) | Obtient l'élément du modèle par un index. |
|
|  | [getOptions()](#getOptions--) | Obtient les options du modèle. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Charge un modèle depuis un fichier. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Charge un modèle depuis un flux. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Enregistre un modèle dans un fichier. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Enregistre un modèle dans un flux. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Initialise une nouvelle instance de la classe [Template](../../com.groupdocs.parser.templates/template).

Utilisation :

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | La collection d'objets [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Initialise une nouvelle instance de la classe [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | La collection d'objets [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Les options du modèle. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre total d'éléments du modèle.


**Returns:**
int - Un entier qui représente le nombre total d'éléments du modèle.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Obtient l'élément du modèle par un index.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | indice | int | L'index basé sur zéro de l'élément du modèle. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Obtient les options du modèle.


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


Charge un modèle depuis un fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Charge un modèle depuis un flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | Le flux d'entrée. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Enregistre un modèle dans un fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Enregistre un modèle dans un flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Le flux de sortie. |
|

