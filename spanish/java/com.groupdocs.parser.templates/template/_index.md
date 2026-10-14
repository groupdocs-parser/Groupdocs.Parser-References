---
title: "Template"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona la plantilla de página del documento."
type: docs
weight: 10
url: /es/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Proporciona la plantilla de la página del documento. Consiste en objetos [TemplateItem](../../com.groupdocs.parser.templates/templateitem) que representan los elementos de la plantilla, como campos de texto y definiciones de tablas.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Inicializa una nueva instancia de la clase [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Inicializa una nueva instancia de la clase [Template](../../com.groupdocs.parser.templates/template). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número total de elementos de plantilla. |
|
|  | [get(int index)](#get-int-) | Obtiene el elemento de plantilla por un índice. |
|
|  | [getOptions()](#getOptions--) | Obtiene las opciones de la plantilla. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Carga una plantilla desde un archivo. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Carga una plantilla desde un flujo. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Guarda una plantilla en un archivo. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Guarda una plantilla en un flujo. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Inicializa una nueva instancia de la clase [Template](../../com.groupdocs.parser.templates/template).

Uso:

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | La colección de objetos [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Inicializa una nueva instancia de la clase [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | La colección de objetos [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Las opciones de la plantilla. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número total de elementos de plantilla.


**Returns:**
int - Un entero que representa el número total de elementos de plantilla.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Obtiene el elemento de plantilla por un índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice basado en cero del elemento de plantilla. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Obtiene las opciones de la plantilla.


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


Carga una plantilla desde un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta al archivo. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Carga una plantilla desde un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.InputStream | El flujo de entrada. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Guarda una plantilla en un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta al archivo. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Guarda una plantilla en un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.OutputStream | El flujo de salida. |
|

