---
title: "TemplateFixedPosition"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce una posizione del campo del modello definita dall'area rettangolare."
type: docs
weight: 13
url: /it/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Fornisce una posizione del campo del modello definita dall'area rettangolare.

Questo è il modo più semplice per definire la posizione del campo. Richiede di impostare un'area rettangolare sulla pagina che delimita
il valore del campo. Tutto il testo contenuto (anche parzialmente) nell'area rettangolare verrà estratto come valore:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [TemplateFixedPosition](../../com.groupdocs.parser/templates/templatefixedposition). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Ottiene l'area rettangolare che contiene il campo del modello. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Inizializza una nuova istanza della classe [TemplateFixedPosition](../../com.groupdocs.parser/templates/templatefixedposition).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il campo del modello. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Ottiene l'area rettangolare che contiene il campo del modello.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crea una copia della posizione corrente con tutte le coordinate scalate del fattore fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fattore | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
