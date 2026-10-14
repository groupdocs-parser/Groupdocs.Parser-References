---
title: "TemplateItem"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce una classe astratta base per gli elementi del modello."
type: docs
weight: 14
url: /it/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Fornisce una classe astratta base per gli elementi del modello.

Gli eredi della classe [TemplateItem](../../com.groupdocs.parser.templates/templateitem) sono utilizzati nella collezione [Template](../../com.groupdocs.parser.templates/template).

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Crea una copia dell'elemento corrente con tutte le coordinate scalate del fattore specificato. |
|
|  | [getName()](#getName--) | Restituisce il nome dell'elemento modello. |
|
|  | [getPageIndex()](#getPageIndex--) | Restituisce l'indice della pagina dell'elemento modello. |
|
|  | [getPageWidth()](#getPageWidth--) | Restituisce la larghezza della pagina utilizzata per creare l'elemento modello. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Restituisce un valore che indica se un  Name  è stato convertito in MAIUSCOLO. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Crea una copia dell'elemento corrente con tutte le coordinate scalate del fattore specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fattore | double | Il fattore di scala. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Restituisce il nome dell'elemento modello.


**Returns:**
java.lang.String - Un valore stringa in maiuscolo che rappresenta il nome dell'elemento modello.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Restituisce l'indice della pagina dell'elemento modello.


**Returns:**
java.lang.Integer - Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento modello;  null  se l'elemento modello si trova su qualsiasi pagina.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Restituisce la larghezza della pagina utilizzata per creare l'elemento modello.


**Returns:**
java.lang.Double - La larghezza della pagina in pixel;  null  se la larghezza della pagina è sconosciuta.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Restituisce un valore che indica se un  Name  è stato convertito in MAIUSCOLO.


**Returns:**
boolean - Un valore booleano che indica se un  Name  è stato convertito in MAIUSCOLO.

