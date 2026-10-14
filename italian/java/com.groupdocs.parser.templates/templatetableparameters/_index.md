---
title: "TemplateTableParameters"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce i parametri per gli algoritmi di rilevamento della tabella."
type: docs
weight: 22
url: /it/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Fornisce i parametri per gli algoritmi di rilevamento della tabella.

Ci sono due algoritmi per rilevare una tabella:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

In alcuni casi, quando gli algoritmi non riescono a rilevare una tabella o lo fanno in modo non accurato, viene utilizzata la classe [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Inizializza una nuova istanza della classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Inizializza una nuova istanza della classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Ottiene l'area rettangolare che contiene la tabella. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Ottiene i separatori delle colonne della tabella. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Ottiene il valore che indica se la tabella ha celle unite. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Ottiene il numero minimo di righe della tabella. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Ottiene il numero minimo di colonne della tabella. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Ottiene lo spazio minimo tra le colonne della tabella. |
|
|  | [scale(double factor)](#scale-double-) | Crea una copia di questi parametri con tutte le coordinate scalate del fattore fornito. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Inizializza una nuova istanza della classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene la tabella. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | I separatori delle colonne della tabella. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Inizializza una nuova istanza della classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene la tabella. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | I separatori delle colonne della tabella. |
|
|  | mergedCells | java.lang.Boolean | Il valore che indica se la tabella ha celle unite. |
|
|  | minRowCount | java.lang.Integer | Il numero minimo di righe della tabella. |
|
|  | minColumnCount | java.lang.Integer | Il numero minimo di colonne della tabella. |
|
|  | minVerticalSpace | java.lang.Integer | Lo spazio minimo tra le colonne della tabella. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Ottiene l'area rettangolare che contiene la tabella.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Ottiene i separatori delle colonne della tabella.


**Returns:**
java.util.List<java.lang.Double> - Una collezione di valori double che rappresentano le coordinate x dei separatori delle colonne della tabella;  null  se non è impostato.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Ottiene il valore che indica se la tabella ha celle unite.


**Returns:**
java.lang.Boolean -  true  se la tabella ha celle unite; altrimenti,  false .  null  se non è impostato.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Ottiene il numero minimo di righe della tabella.


**Returns:**
java.lang.Integer - Un valore intero che rappresenta il numero minimo di righe della tabella;  null  se non è impostato.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Ottiene il numero minimo di colonne della tabella.


**Returns:**
java.lang.Integer - Un valore intero che rappresenta il numero minimo di colonne della tabella;  null  se non è impostato.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Ottiene lo spazio minimo tra le colonne della tabella.


**Returns:**
java.lang.Integer - Un valore intero che rappresenta lo spazio minimo tra le colonne della tabella;  null  se non è impostato.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Crea una copia di questi parametri con tutte le coordinate scalate del fattore fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fattore | double | Il fattore di scala. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

