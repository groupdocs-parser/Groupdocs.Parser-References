---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Tabellenzelle dar, die in der Klasse verwendet wird."
type: docs
weight: 23
url: /de/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Stellt eine Tabellenzelle dar, die in der [PageTableArea](../../com.groupdocs.parser.data/pagetablearea)-Klasse verwendet wird.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Initialisiert eine neue Instanz der [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell)-Klasse. |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Initialisiert eine neue Instanz der [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Liefert den Zeilenindex. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Liefert den Spaltenindex. |
|
|  | [getRowSpan()](#getRowSpan--) | Liefert die Gesamtzahl der Zeilen, die die Tabellenzelle enthalten. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Liefert die Gesamtzahl der Spalten, die die Tabellenzelle enthalten. |
|
|  | [getPageArea()](#getPageArea--) | Liefert den Wert der Tabellenzelle. |
|
|  | [getText()](#getText--) | Liefert den Textwert der Tabellenzelle. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Initialisiert eine neue Instanz der [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rowIndex | int | Der nullbasierte Index der Zeile. |
|
|  | columnIndex | int | Der nullbasierte Index der Spalte. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Der Wert der Tabellenzelle. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Initialisiert eine neue Instanz der [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rowIndex | int | Der nullbasierte Index der Zeile. |
|
|  | columnIndex | int | Der nullbasierte Index der Spalte. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Der Wert der Tabellenzelle. |
|
|  | rowSpan | int | Die Gesamtzahl der Zeilen, die die Tabellenzelle enthalten. |
|
|  | columnSpan | int | Die Gesamtzahl der Spalten, die die Tabellenzelle enthalten. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Liefert den Zeilenindex.


**Returns:**
int – Ein nullbasierter Index der ersten Zeile, die die Tabellenzelle enthält.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Liefert den Spaltenindex.


**Returns:**
int – Ein nullbasierter Index der ersten Spalte, die die Tabellenzelle enthält.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Liefert die Gesamtzahl der Zeilen, die die Tabellenzelle enthalten.


**Returns:**
int – Ein positiver ganzzahliger Wert, der die Gesamtzahl der Zeilen darstellt, die die Tabellenzelle enthalten.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Liefert die Gesamtzahl der Spalten, die die Tabellenzelle enthalten.


**Returns:**
int – Ein positiver ganzzahliger Wert, der die Gesamtzahl der Spalten darstellt, die die Tabellenzelle enthalten.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Liefert den Wert der Tabellenzelle.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Liefert den Textwert der Tabellenzelle.


**Returns:**
java.lang.String – Ein String, der den Textwert der Zelle darstellt;  null  falls die Zelle keinen Textwert enthält.

