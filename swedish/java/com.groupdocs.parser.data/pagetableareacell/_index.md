---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en tabellcell som används i  klass."
type: docs
weight: 23
url: /sv/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Representerar en tabellcell som används i [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) klass.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Initierar en ny instans av [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) klass. |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Initierar en ny instans av [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) klass. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Hämtar radindexet. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Hämtar kolumnindexet. |
|
|  | [getRowSpan()](#getRowSpan--) | Hämtar det totala antalet rader som innehåller tabellcellen. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Hämtar det totala antalet kolumner som innehåller tabellcellen. |
|
|  | [getPageArea()](#getPageArea--) | Hämtar tabellcellens värde. |
|
|  | [getText()](#getText--) | Hämtar tabellcellens textvärde. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Initierar en ny instans av [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) klass.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rowIndex | int | Det nollbaserade indexet för raden. |
|
|  | columnIndex | int | Det nollbaserade indexet för kolumnen. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Värdet på tabellcellen. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Initierar en ny instans av [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) klass.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rowIndex | int | Det nollbaserade indexet för raden. |
|
|  | columnIndex | int | Det nollbaserade indexet för kolumnen. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Värdet på tabellcellen. |
|
|  | rowSpan | int | Det totala antalet rader som innehåller tabellcellen. |
|
|  | columnSpan | int | Det totala antalet kolumner som innehåller tabellcellen. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Hämtar radindexet.


**Returns:**
int - Ett nollbaserat index för den första raden som innehåller tabellcellen.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Hämtar kolumnindexet.


**Returns:**
int - Ett nollbaserat index för den första kolumnen som innehåller tabellcellen.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Hämtar det totala antalet rader som innehåller tabellcellen.


**Returns:**
int - Ett positivt heltal som representerar det totala antalet rader som innehåller tabellcellen.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Hämtar det totala antalet kolumner som innehåller tabellcellen.


**Returns:**
int - Ett positivt heltal som representerar det totala antalet kolumner som innehåller tabellcellen.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Hämtar tabellcellens värde.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Hämtar tabellcellens textvärde.


**Returns:**
java.lang.String - En sträng som representerar ett textvärde för cellen;  null  om cellen inte innehåller ett textvärde.

