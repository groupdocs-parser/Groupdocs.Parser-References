---
title: "PageTableArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablonla ayrıştırma işlevinde bir tabloyu temsil etmek için kullanılan bir tablo sayfa alanını temsil eder."
type: docs
weight: 22
url: /tr/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Şablonla ayrıştırma işlevinde bir tabloyu temsil etmek için kullanılan bir tablo sayfa alanını temsil eder.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Yeni bir [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCells()](#getCells--) | Hücre koleksiyonunu alır. |
|
|  | [getRowCount()](#getRowCount--) | Tablo satırlarının toplam sayısını alır. |
|
|  | [getColumnCount()](#getColumnCount--) | Tablo sütunlarının toplam sayısını alır. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Satır yüksekliğini döndürür. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Sütun genişliğini döndürür. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Satır ve sütun indekslerine göre tablo hücresini alır. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Yeni bir [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) sınıfının örneğini başlatır.

Not: C# projesi bu yapıcıyı şu şekilde işaretler
internal
(commit 954951f). Java'da "internal-to-the-assembly"
paket-özeline temiz bir şekilde çevrilemez çünkü üreticiler (
WordProcessingParser
,
TableAreaParser
,
vb.) şunlarda bulunur
com.groupdocs.parser
, değil
com.groupdocs.parser.data
. Yapıcı bu nedenle tutulur

public
böylece paketler arası yapılandırma hâlâ çalışır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | satırlar | java.lang.Iterable<java.lang.Double> | Satır yüksekliklerinin koleksiyonu. |
|
|  | sütunlar | java.lang.Iterable<java.lang.Double> | Sütun genişliklerinin koleksiyonu. |
|
|  | hücreler | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | Hücrelerin koleksiyonu. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Tabloyu içeren sayfa. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Tabloyu içeren dikdörtgen alan. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Hücrelerin koleksiyonunu alır. Tablo hücrelerinin basit, yalnızca okunabilir bir koleksiyonu.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Tablo hücrelerinin bir koleksiyonu

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Tablo satırlarının toplam sayısını alır.


**Returns:**
int - Tablo satırlarının toplam sayısını içeren bir tam sayı değeri.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Tablo sütunlarının toplam sayısını alır.


**Returns:**
int - Tablo sütunlarının toplam sayısını içeren bir tam sayı değeri.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Satır yüksekliğini döndürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rowIndex | int | Satırın sıfır tabanlı indeksidir. |
|

**Returns:**
double - Satırın yüksekliğini temsil eden bir çift (double) değeri.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Sütun genişliğini döndürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | columnIndex | int | Sütunun sıfır tabanlı indeksidir. |
|

**Returns:**
double - Sütunun genişliğini temsil eden bir çift (double) değeri.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Satır ve sütun indekslerine göre tablo hücresini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rowIndex | int | Hücre satırının sıfır tabanlı indeksi. |
|
|  | columnIndex | int | Hücre sütununun sıfır tabanlı indeksi. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

