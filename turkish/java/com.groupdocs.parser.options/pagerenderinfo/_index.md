---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Bir sayfanın nasıl render edildiği bilgisini temsil eder."
type: docs
weight: 30
url: /tr/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Bir sayfanın nasıl render edildiği bilgisini temsil eder.

Bazı belgeler (örneğin elektronik tablolar), bir sayfayı render etmek mümkün değildir
tek bir görüntü olarak. Bu belgeler için bir sayfa bir dizi karo olarak render edilir.
Bu karolar dikdörtgen tablo içinde yer alır.


RowCount
ve
ColumnCount
satır ve sütunların toplam sayısını temsil eder
bu tablonun. Belge sayfası tek bir görüntüye render edilirse bu özellikler 1'e eşittir.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Yeni bir [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Sayfa numarasını alır. |
|
|  | [getRowCount()](#getRowCount--) | Döşeme satırlarının toplam sayısını al. |
|
|  | [getColumnCount()](#getColumnCount--) | Döşeme sütunlarının toplam sayısını al. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | tileIndex ile belirtilen döşemenin yer aldığı sütunun indeksini döndürür. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | tileIndex ile belirtilen döşemenin yer aldığı satırın indeksini döndürür. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Yeni bir [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageNumber | int | Sayfanın numarası (1'den başlar). |
|
|  | rowCount | int | Döşeme satırlarının toplam sayısı. |
|
|  | columnCount | int | Döşeme sütunlarının toplam sayısı. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Sayfa numarasını alır.


**Returns:**
int - Sayfa numarasını temsil eden tam sayı değeri (1'den başlar).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Döşeme satırlarının toplam sayısını al.


**Returns:**
int - Döşeme satırlarının toplam sayısını temsil eden tam sayı değeri.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Döşeme sütunlarının toplam sayısını al.


**Returns:**
int - Döşeme sütunlarının toplam sayısını temsil eden tam sayı değeri.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


tileIndex ile belirtilen döşemenin yer aldığı sütunun indeksini döndürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | tileIndex | int | Döşemenin sıfır tabanlı indeksi. |
|

**Returns:**
int - Sütun indeksini temsil eden sıfır tabanlı tam sayı değeri.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


tileIndex ile belirtilen döşemenin yer aldığı satırın indeksini döndürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | tileIndex | int | Döşemenin sıfır tabanlı indeksi. |
|

**Returns:**
int - Satır indeksini temsil eden sıfır tabanlı tam sayı değeri.

