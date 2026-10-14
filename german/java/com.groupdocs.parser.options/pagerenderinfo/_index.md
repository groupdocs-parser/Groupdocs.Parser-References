---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Informationen darüber dar, wie eine Seite gerendert wird."
type: docs
weight: 30
url: /de/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Stellt die Informationen darüber dar, wie eine Seite gerendert wird.

Einige Dokumente (Tabellenkalkulationen, zum Beispiel) können nicht als einzelne Seite gerendert werden
als ein einzelnes Bild. Für diese Dokumente wird eine Seite als Menge von Kacheln gerendert.
Diese Kacheln werden in der rechteckigen Tabelle platziert.


RowCount
und
ColumnCount
repräsentieren die Gesamtzahl der Zeilen und Spalten
dieser Tabelle. Wenn die Dokumentenseite als einzelnes Bild gerendert wird, sind diese Eigenschaften gleich 1.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Initialisiert eine neue Instanz der [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Liefert die Seitennummer. |
|
|  | [getRowCount()](#getRowCount--) | Gibt die Gesamtzahl der Kachelzeilen zurück. |
|
|  | [getColumnCount()](#getColumnCount--) | Gibt die Gesamtzahl der Kachelspalten zurück. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Gibt den Index der Spalte zurück, in der die Kachel mit  tileIndex  platziert ist. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Gibt den Index der Zeile zurück, in der die Kachel mit  tileIndex  platziert ist. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Initialisiert eine neue Instanz der [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageNumber | int | Die Nummer der Seite (beginnt bei 1). |
|
|  | rowCount | int | Die Gesamtzahl der Kachelzeilen. |
|
|  | columnCount | int | Die Gesamtzahl der Kachelspalten. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Liefert die Seitennummer.


**Returns:**
int - Der ganzzahlige Wert, der die Seitennummer darstellt (beginnt bei 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Gibt die Gesamtzahl der Kachelzeilen zurück.


**Returns:**
int - Der ganzzahlige Wert, der die Gesamtzahl der Kachelzeilen darstellt.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Gibt die Gesamtzahl der Kachelspalten zurück.


**Returns:**
int - Der ganzzahlige Wert, der die Gesamtzahl der Kachelspalten darstellt.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Gibt den Index der Spalte zurück, in der die Kachel mit  tileIndex  platziert ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | tileIndex | int | Der nullbasierte Index der Kachel. |
|

**Returns:**
int - Der nullbasierte ganzzahlige Wert, der den Spaltenindex darstellt.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Gibt den Index der Zeile zurück, in der die Kachel mit  tileIndex  platziert ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | tileIndex | int | Der nullbasierte Index der Kachel. |
|

**Returns:**
int - Der nullbasierte ganzzahlige Wert, der den Zeilenindex darstellt.

