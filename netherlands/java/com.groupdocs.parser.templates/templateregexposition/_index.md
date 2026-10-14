---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt een sjabloon-veldpositie die de reguliere expressie gebruikt."
type: docs
weight: 19
url: /nl/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Biedt een sjabloon-veldpositie die de reguliere expressie gebruikt.

Het volgende voorbeeld toont de situatie als het document "Invoice Number INV-12345" bevat
dan kan het sjabloonveld op de volgende manier worden gedefinieerd:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

In dit geval wordt de volledige tekenreeks als waarde geëxtraheerd. Om alleen een deel van de tekenreeks te extraheren
de reguliere-expressiegroep "value" wordt gebruikt:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

In dit geval wordt de tekenreeks "INV-3337" als waarde geëxtraheerd.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Initialiseert een nieuw exemplaar van de klasse [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getExpression()](#getExpression--) | Haalt de reguliere expressie op. |
|
|  | [isMatchCase()](#isMatchCase--) | Haalt de waarde op die aangeeft of hoofdlettergebruik van tekst niet wordt genegeerd. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Haalt de reguliere expressie op.


**Returns:**
java.lang.String - Een string die de reguliere expressie vertegenwoordigt.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Haalt de waarde op die aangeeft of hoofdlettergebruik van tekst niet wordt genegeerd.


**Returns:**
boolean -  true  als een tekstcase niet wordt genegeerd; anders,  false .

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Maakt een kopie van de huidige positie waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
