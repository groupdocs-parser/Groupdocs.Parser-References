---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller en mallfältposition som använder reguljära uttrycket."
type: docs
weight: 19
url: /sv/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Tillhandahåller en mallfältposition som använder reguljära uttrycket.

Följande exempel visar situationen om dokumentet innehåller "Invoice Number INV-12345"
då kan mallfältet definieras på följande sätt:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

I det här fallet extraheras hela strängen som värde. För att extrahera endast en del av strängen
regular expression‑gruppen "value" används:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

I det här fallet extraheras strängen "INV-3337" som värde.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Initierar en ny instans av klassen [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Initierar en ny instans av klassen [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getExpression()](#getExpression--) | Hämtar det reguljära uttrycket. |
|
|  | [isMatchCase()](#isMatchCase--) | Hämtar värdet som indikerar om ett textfall inte ignoreras. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Initierar en ny instans av klassen [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Initierar en ny instans av klassen [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Hämtar det reguljära uttrycket.


**Returns:**
java.lang.String - En sträng som representerar det reguljära uttrycket.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Hämtar värdet som indikerar om ett textfall inte ignoreras.


**Returns:**
boolean -  true  om skiftläge i texten inte ignoreras; annars,  false .

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Skapar en kopia av den aktuella positionen med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
