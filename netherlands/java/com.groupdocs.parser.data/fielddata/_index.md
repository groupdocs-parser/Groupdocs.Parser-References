---
title: "FieldData"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Vertegenwoordigt veldgegevens zoals een naam, een paginanummer, een veldwaarde enzovoort."
type: docs
weight: 13
url: /nl/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Vertegenwoordigt veldgegevens zoals een naam, een paginanummer, een veldwaarde enzovoort. Afhankelijk van het veld kan de waarde een tekst, een afbeelding, een tabel enzovoort zijn.

De instanties van [FieldData](../../com.groupdocs.parser.data/fielddata) klasse worden gebruikt in de [DocumentData](../../com.groupdocs.parser.data/documentdata) collectie.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getName()](#getName--) | Haalt de veldnaam op. |
|
|  | [getPageIndex()](#getPageIndex--) | Haalt het paginanummer op. |
|
|  | [getPageArea()](#getPageArea--) | Haalt de waarde van het veld op. |
|
|  | [getLinkedField()](#getLinkedField--) | Haalt het gekoppelde veld op. |
|
|  | [getText()](#getText--) | Haalt de tekst op. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Haalt een waarde op die aangeeft of een  Name  is omgezet naar HOOFDLETTERS. |
|
### getName() {#getName--}
```
public String getName()
```


Haalt de veldnaam op.


**Returns:**
java.lang.String - Een tekenreekswaarde in hoofdletters die de naam van het veld vertegenwoordigt.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Haalt het paginanummer op.


**Returns:**
int - Een nulgebaseerde index van de pagina die het veld bevat.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Haalt de waarde van het veld op.

Afhankelijk van het veld kan de PageArea-eigenschap elk van de afgeleiden van de [PageArea](../../com.groupdocs.parser.data/pagearea) klasse bevatten.
Bijvoorbeeld, de [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) methode extraheert alleen tekstvelden.

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


Haalt het gekoppelde veld op.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Haalt de tekst op.


**Returns:**
java.lang.String - Een tekenreekswaarde die een waarde van de veldtekst vertegenwoordigt;  null  als de [PageArea](../../com.groupdocs.parser.data/pagearea) eigenschap geen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) is.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Haalt een waarde op die aangeeft of een  Name  is omgezet naar HOOFDLETTERS.


**Returns:**
boolean - Een booleaanse waarde die aangeeft of een  Name  is omgezet naar HOOFDLETTERS.

