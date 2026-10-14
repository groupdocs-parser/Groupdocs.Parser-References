---
title: "TemplateTableLayout"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce il layout della tabella modello che è utilizzato dalla classe per definire la posizione della tabella."
type: docs
weight: 21
url: /it/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Fornisce il layout della tabella modello che è utilizzato dalla classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) per definire la posizione della tabella.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Inizializza una nuova istanza della classe [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Ottiene l'area rettangolare che contiene la tabella. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Ottiene i separatori delle colonne della tabella. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Ottiene i separatori delle righe della tabella. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Crea un nuovo layout con le stesse dimensioni, separatori e posizione nel punto. |
|
|  | [scale(double factor)](#scale-double-) | Crea una copia di questo layout con tutte le coordinate scalate del fattore fornito. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Inizializza una nuova istanza della classe [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | I separatori delle colonne della tabella. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | I separatori delle righe della tabella. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Ottiene l'area rettangolare che contiene la tabella.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Ottiene i separatori delle colonne della tabella.


**Returns:**
java.util.List<java.lang.Double> - Una collezione di valori double che rappresentano le coordinate x dei separatori delle colonne della tabella.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Ottiene i separatori delle righe della tabella.


**Returns:**
java.util.List<java.lang.Double> - Una collezione di valori double che rappresentano le coordinate y dei separatori delle righe della tabella.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Crea un nuovo layout con le stesse dimensioni, separatori e posizione nel punto.

Questa funzionalità consente di spostare il Layout della Tabella.

Ad esempio, un documento ha tabelle su ogni pagina (o un insieme di documenti con una tabella nella pagina).
Queste tabelle differiscono per posizione e contenuto, ma hanno le stesse colonne e righe. In questo caso un utente
può definire l'oggetto [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) a (0, 0) una volta e poi spostarlo nella posizione della tabella specifica.

Se la posizione della tabella dipende da un altro oggetto della pagina, un utente può definire l'oggetto [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)
basato sul documento modello e poi spostarlo secondo un oggetto di ancoraggio. Ad esempio, se questa è una tabella riepilogativa
e viene seguita da una tabella di dettagli (che può contenere un numero diverso di righe). In questo caso un utente può definire
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
il metodo restituisce una copia dell'oggetto corrente. Un utente può passare qualsiasi coordinata
(anche negative - allora il layout verrà spostato a sinistra/alto).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | La posizione del nuovo layout. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Crea una copia di questo layout con tutte le coordinate scalate del fattore fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fattore | double | Il fattore di scala. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

