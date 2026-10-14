---
title: "PageTableArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Tabellen‑Seitenbereich dar, der verwendet wird, um eine Tabelle in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren."
type: docs
weight: 22
url: /de/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Stellt einen Tabellen‑Seitenbereich dar, der verwendet wird, um eine Tabelle in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCells()](#getCells--) | Liefert die Sammlung der Zellen. |
|
|  | [getRowCount()](#getRowCount--) | Liefert die Gesamtzahl der Tabellenzeilen. |
|
|  | [getColumnCount()](#getColumnCount--) | Liefert die Gesamtzahl der Tabellenspalten. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Gibt die Zeilenhöhe zurück. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Gibt die Spaltenbreite zurück. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Liefert die Tabellenzelle nach Zeilen- und Spaltenindizes. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Hinweis: Das C#‑Projekt markiert diesen Konstruktor als
internal
(commit 954951f). In Java, "internal-to-the-assembly"
lässt sich nicht sauber in package-private übersetzen, weil die Erzeuger (
WordProcessingParser
,
TableAreaParser
,
usw.) befinden sich in
com.groupdocs.parser
, nicht
com.groupdocs.parser.data
. Der Konstruktor wird daher beibehalten

public
so funktioniert die paketübergreifende Konstruktion weiterhin.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeilen | java.lang.Iterable<java.lang.Double> | Die Sammlung der Zeilenhöhen. |
|
|  | Spalten | java.lang.Iterable<java.lang.Double> | Die Sammlung der Spaltenbreiten. |
|
|  | Zellen | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | Die Sammlung der Zellen. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die die Tabelle enthält. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der die Tabelle enthält. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Ruft die Sammlung der Zellen ab. Eine einfache schreibgeschützte Sammlung von Tabellenzellen.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Eine Sammlung von Tabellenzellen

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Liefert die Gesamtzahl der Tabellenzeilen.


**Returns:**
int - Ein ganzzahliger Wert, der die Gesamtzahl der Tabellenzeilen enthält.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Liefert die Gesamtzahl der Tabellenspalten.


**Returns:**
int - Ein ganzzahliger Wert, der die Gesamtzahl der Tabellenspalten enthält.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Gibt die Zeilenhöhe zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rowIndex | int | Der nullbasierte Index der Zeile. |
|

**Returns:**
double - Ein double-Wert, der die Höhe der Zeile darstellt.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Gibt die Spaltenbreite zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | columnIndex | int | Der nullbasierte Index der Spalte. |
|

**Returns:**
double - Ein double-Wert, der die Breite der Spalte darstellt.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Liefert die Tabellenzelle nach Zeilen- und Spaltenindizes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rowIndex | int | Der nullbasierte Index der Zellenzeile. |
|
|  | columnIndex | int | Der nullbasierte Index der Zellenspalte. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

