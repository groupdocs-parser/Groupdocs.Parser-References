---
title: "DocumentData"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta i dati del documento."
type: docs
weight: 11
url: /it/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Rappresenta i dati del documento. È composto da oggetti [FieldData](../../com.groupdocs.parser.data/fielddata) che contengono i dati dei campi dal documento. Un'istanza della classe [DocumentData](../../com.groupdocs.parser.data/documentdata) viene utilizzata come valore di ritorno dei metodi [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) e [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . Vedi gli esempi d'uso lì.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Ottiene il modello che ha prodotto questi dati del documento. |
|
|  | [getCount()](#getCount--) | Ottiene il numero totale dei dati dei campi. |
|
|  | [get(int index)](#get-int-) | Ottiene i dati del campo per indice. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Restituisce la collezione di dati del campo il cui nome è uguale a  fieldName . |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore sugli elementi di questa lista nella sequenza corretta. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Ottiene il modello che ha prodotto questi dati del documento.

Quando i dati sono stati prodotti da una selezione automatica di raccolta di modelli (vedi
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
questo è il modello selezionato.
null
quando i dati non sono stati prodotti da un modello.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il numero totale dei dati dei campi.


**Returns:**
int - Un valore intero che rappresenta il numero totale dei dati dei campi.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Ottiene i dati del campo per indice.

Iterazione attraverso tutti i campi:

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
degli eredi della classe [PageArea](../../com.groupdocs.parser.data/pagearea). Ad esempio, il metodo [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) estrae solo i campi di testo:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice basato su zero del campo. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Restituisce la collezione di dati del campo il cui nome è uguale a  fieldName .

Trova i campi per nome del campo:

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
qualsiasi degli eredi della classe [PageArea](../../com.groupdocs.parser.data/pagearea). Ad esempio, il metodo [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) estrae solo i campi di testo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fieldName | java.lang.String | Il nome del campo. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Una collezione di oggetti [FieldData](../../com.groupdocs.parser.data/fielddata); collezione vuota se non vengono trovati dati del campo.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Restituisce un iteratore sugli elementi di questa lista nella sequenza corretta.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - un iteratore sugli elementi di questa lista nella sequenza corretta.

