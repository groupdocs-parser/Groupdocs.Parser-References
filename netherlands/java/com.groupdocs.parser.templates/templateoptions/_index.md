---
title: "TemplateOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor het parseren via sjabloonfunctionaliteit."
type: docs
weight: 17
url: /nl/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Biedt de opties die worden gebruikt voor het parseren via sjabloonfunctionaliteit.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Initialiseert een nieuw exemplaar van de klasse [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Haalt de grootte van de rand op die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangleTolerance | double | De grootte van de rand die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Deze wordt gemeten als een fractie van de hoogte van een tekstelement. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Haalt de grootte van de rand op die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Deze wordt gemeten als een fractie van de hoogte van een tekstelement.


**Returns:**
double - De double‑waarde van 0 (geen rand) tot 1 (negeer het hele element).

