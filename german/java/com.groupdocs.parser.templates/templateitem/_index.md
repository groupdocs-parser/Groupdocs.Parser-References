---
title: "TemplateItem"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine abstrakte Basisklasse für Vorlagenobjekte bereit."
type: docs
weight: 14
url: /de/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Stellt eine abstrakte Basisklasse für Vorlagenobjekte bereit.

Die Erben der Klasse [TemplateItem](../../com.groupdocs.parser.templates/templateitem) werden in der [Template](../../com.groupdocs.parser.templates/template)-Sammlung verwendet.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Erstellt eine Kopie des aktuellen Elements, wobei alle Koordinaten um den angegebenen Faktor skaliert werden. |
|
|  | [getName()](#getName--) | Gibt den Namen des Vorlagen-Elements zurück. |
|
|  | [getPageIndex()](#getPageIndex--) | Gibt den Seitenindex des Vorlagen-Elements zurück. |
|
|  | [getPageWidth()](#getPageWidth--) | Gibt die Breite der Seite zurück, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Gibt einen Wert zurück, der angibt, ob ein  Name  in GROSSBUCHSTABEN konvertiert wurde. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Erstellt eine Kopie des aktuellen Elements, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Faktor | double | Der Skalierungsfaktor. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Gibt den Namen des Vorlagen-Elements zurück.


**Returns:**
java.lang.String - Ein Großbuchstaben-Stringwert, der den Namen des Vorlagen-Elements darstellt.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Gibt den Seitenindex des Vorlagen-Elements zurück.


**Returns:**
java.lang.Integer - Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagen-Element positioniert ist;  null  wenn das Vorlagen-Element auf einer beliebigen Seite liegt.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Gibt die Breite der Seite zurück, die zur Erstellung des Vorlagen-Elements verwendet wurde.


**Returns:**
java.lang.Double - Die Breite der Seite in Pixeln;  null  wenn die Seitenbreite unbekannt ist.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Gibt einen Wert zurück, der angibt, ob ein  Name  in GROSSBUCHSTABEN konvertiert wurde.


**Returns:**
boolean - Ein boolescher Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN konvertiert wurde.

