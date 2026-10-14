---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Vorlagenfeldposition bereit, die den regulären Ausdruck verwendet."
type: docs
weight: 19
url: /de/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Stellt eine Vorlagenfeldposition bereit, die den regulären Ausdruck verwendet.

Das folgende Beispiel zeigt die Situation, wenn das Dokument \"Invoice Number INV-12345\" enthält.
Dann kann das Vorlagenfeld wie folgt definiert werden:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

In diesem Fall wird als Wert die gesamte Zeichenkette extrahiert. Um nur einen Teil der Zeichenkette zu extrahieren
wird die reguläre Ausdrucksgruppe \"value\" verwendet:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

In diesem Fall wird als Wert die Zeichenkette \"INV-3337\" extrahiert.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Initialisiert eine neue Instanz der [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)-Klasse. |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Initialisiert eine neue Instanz der [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getExpression()](#getExpression--) | Liefert den regulären Ausdruck. |
|
|  | [isMatchCase()](#isMatchCase--) | Liefert den Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Initialisiert eine neue Instanz der [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Initialisiert eine neue Instanz der [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Liefert den regulären Ausdruck.


**Returns:**
java.lang.String - Eine Zeichenkette, die den regulären Ausdruck darstellt.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Liefert den Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird.


**Returns:**
boolean -  true  wenn die Groß-/Kleinschreibung nicht ignoriert wird; andernfalls  false .

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Erstellt eine Kopie der aktuellen Position, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
