---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een tabelcel voor die wordt gebruikt in de klasse."
type: docs
weight: 23
url: /nl/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Stelt een tabelcel voor die wordt gebruikt in de klasse [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Initialiseert een nieuw exemplaar van de klasse [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Initialiseert een nieuw exemplaar van de klasse [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Haalt de rij‑index op. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Haalt de kolom‑index op. |
|
|  | [getRowSpan()](#getRowSpan--) | Haalt het totale aantal rijen op dat de tabelcel bevat. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Haalt het totale aantal kolommen op dat de tabelcel bevat. |
|
|  | [getPageArea()](#getPageArea--) | Haalt de waarde van de tabelcel op. |
|
|  | [getText()](#getText--) | Haalt de tekstwaarde van de tabelcel op. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Initialiseert een nieuw exemplaar van de klasse [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rowIndex | int | De nulgebaseerde index van de rij. |
|
|  | columnIndex | int | De nulgebaseerde index van de kolom. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | De waarde van de tabelcel. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Initialiseert een nieuw exemplaar van de klasse [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rowIndex | int | De nulgebaseerde index van de rij. |
|
|  | columnIndex | int | De nulgebaseerde index van de kolom. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | De waarde van de tabelcel. |
|
|  | rowSpan | int | Het totale aantal rijen dat de tabelcel bevat. |
|
|  | columnSpan | int | Het totale aantal kolommen dat de tabelcel bevat. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Haalt de rij‑index op.


**Returns:**
int - Een nulgebaseerde index van de eerste rij die de tabelcel bevat.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Haalt de kolom‑index op.


**Returns:**
int - Een nulgebaseerde index van de eerste kolom die de tabelcel bevat.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Haalt het totale aantal rijen op dat de tabelcel bevat.


**Returns:**
int - Een positieve gehele waarde die het totale aantal rijen dat de tabelcel bevat weergeeft.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Haalt het totale aantal kolommen op dat de tabelcel bevat.


**Returns:**
int - Een positieve gehele waarde die het totale aantal kolommen dat de tabelcel bevat weergeeft.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Haalt de waarde van de tabelcel op.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Haalt de tekstwaarde van de tabelcel op.


**Returns:**
java.lang.String - Een string die een tekstwaarde van de cel vertegenwoordigt;  null  als de cel geen tekstwaarde bevat.

