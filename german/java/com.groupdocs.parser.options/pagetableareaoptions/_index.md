---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion von Tabellenseitenbereichen verwendet werden."
type: docs
weight: 31
url: /de/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Stellt die Optionen bereit, die für die Extraktion von Tabellenseitenbereichen verwendet werden.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Initialisiert eine neue Instanz der [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions)-Klasse. |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions)-Klasse mit einem Suchrechteck und ohne feste Layout. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Liefert das Tabellenlayout, das die Tabelle auf einer Seite definiert. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Initialisiert eine neue Instanz der [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Das Tabellenlayout, das die Tabelle auf einer Seite definiert. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Initialisiert eine neue Instanz der [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions)-Klasse mit einem Suchrechteck und ohne feste Layout.

Nützlich, um automatisch erkannte Tabellen auf einen Bereich der Seite zu beschränken. Spiegelt das C#.

new PageTableAreaOptions(null) { Rectangle = ... }
Muster.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich auf der Seite, in dem Tabellen erkannt werden sollen; übergeben Sie  null , um die gesamte Seite zu durchsuchen. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Liefert das Tabellenlayout, das die Tabelle auf einer Seite definiert.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

