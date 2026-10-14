---
title: "Template"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce il modello di pagina del documento."
type: docs
weight: 10
url: /it/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Fornisce il modello della pagina del documento. È composto da oggetti [TemplateItem](../../com.groupdocs.parser/templates/templateitem) che rappresentano gli elementi del modello come campi di testo e definizioni di tabelle.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Inizializza una nuova istanza della classe [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Inizializza una nuova istanza della classe [Template](../../com.groupdocs.parser.templates/template). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Restituisce il numero totale di elementi del modello. |
|
|  | [get(int index)](#get-int-) | Restituisce l'elemento del modello per indice. |
|
|  | [getOptions()](#getOptions--) | Restituisce le opzioni del modello. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Carica un modello da un file. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Carica un modello da uno stream. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Salva un modello su un file. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Salva un modello su uno stream. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Inizializza una nuova istanza della classe [Template](../../com.groupdocs.parser.templates/template).

Utilizzo:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | La collezione di oggetti [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Inizializza una nuova istanza della classe [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | La collezione di oggetti [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Le opzioni del modello. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Restituisce il numero totale di elementi del modello.


**Returns:**
int - Un intero che rappresenta il numero totale di elementi del modello.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Restituisce l'elemento del modello per indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice basato su zero dell'elemento del modello. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Restituisce le opzioni del modello.


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


Carica un modello da un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Carica un modello da uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.InputStream | Lo stream di input. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Salva un modello su un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Salva un modello su uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Il flusso di output. |
|

