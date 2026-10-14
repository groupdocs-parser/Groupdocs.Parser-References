---
title: "TemplateItem"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt een abstracte basisklasse voor sjabloonitems."
type: docs
weight: 14
url: /nl/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Biedt een abstracte basisklasse voor sjabloonitems.

De afstammelingen van de klasse [TemplateItem](../../com.groupdocs.parser.templates/templateitem) worden gebruikt in de collectie [Template](../../com.groupdocs.parser.templates/template).

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Maakt een kopie van het huidige item waarbij alle coördinaten worden geschaald met de opgegeven factor. |
|
|  | [getName()](#getName--) | Haalt de naam van het sjabloonitem op. |
|
|  | [getPageIndex()](#getPageIndex--) | Haalt het paginanummer van het sjabloonitem op. |
|
|  | [getPageWidth()](#getPageWidth--) | Haalt de breedte van de pagina op die werd gebruikt om het sjabloonitem te maken. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Haalt een waarde op die aangeeft of een  Name  is omgezet naar HOOFDLETTERS. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Maakt een kopie van het huidige item waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | factor | double | De schaalfactor. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Haalt de naam van het sjabloonitem op.


**Returns:**
java.lang.String - Een hoofdlettertekenreeks die de naam van het sjabloonitem vertegenwoordigt.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Haalt het paginanummer van het sjabloonitem op.


**Returns:**
java.lang.Integer - Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt;  null  als het sjabloonitem zich op een willekeurige pagina bevindt.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Haalt de breedte van de pagina op die werd gebruikt om het sjabloonitem te maken.


**Returns:**
java.lang.Double - De breedte van de pagina in pixels;  null  als de paginabreedte onbekend is.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Haalt een waarde op die aangeeft of een  Name  is omgezet naar HOOFDLETTERS.


**Returns:**
boolean - Een booleaanse waarde die aangeeft of een  Name  is omgezet naar HOOFDLETTERS.

