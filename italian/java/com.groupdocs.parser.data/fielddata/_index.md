---
title: "FieldData"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta i dati del campo come un nome, un indice di pagina, un valore del campo e così via."
type: docs
weight: 13
url: /it/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Rappresenta i dati del campo come un nome, un indice di pagina, un valore del campo e così via. A seconda del campo, il valore può essere un testo, un'immagine, una tabella e così via.

Le istanze della classe [FieldData](../../com.groupdocs.parser.data/fielddata) sono utilizzate nella collezione [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getName()](#getName--) | Restituisce il nome del campo. |
|
|  | [getPageIndex()](#getPageIndex--) | Restituisce l'indice della pagina. |
|
|  | [getPageArea()](#getPageArea--) | Restituisce il valore del campo. |
|
|  | [getLinkedField()](#getLinkedField--) | Restituisce il campo collegato. |
|
|  | [getText()](#getText--) | Restituisce il testo. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Restituisce un valore che indica se un  Name  è stato convertito in MAIUSCOLO. |
|
### getName() {#getName--}
```
public String getName()
```


Restituisce il nome del campo.


**Returns:**
java.lang.String - Un valore stringa in maiuscolo che rappresenta il nome del campo.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Restituisce l'indice della pagina.


**Returns:**
int - Un indice basato su zero della pagina che contiene il campo.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Restituisce il valore del campo.

A seconda del campo, la proprietà PageArea può contenere uno qualsiasi degli eredi della classe [PageArea](../../com.groupdocs.parser.data/pagearea).
Ad esempio, il metodo [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) estrae solo i campi di testo.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Restituisce il campo collegato.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Restituisce il testo.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il valore del testo del campo; null se la proprietà [PageArea](../../com.groupdocs.parser.data/pagearea) non è [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Restituisce un valore che indica se un  Name  è stato convertito in MAIUSCOLO.


**Returns:**
boolean - Un valore booleano che indica se un  Name  è stato convertito in MAIUSCOLO.

