---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sınıfta kullanılan bir tablo hücresini temsil eder."
type: docs
weight: 23
url: /tr/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Sınıfta kullanılan bir tablo hücresini temsil eder. [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) sınıfı.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Yeni bir [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) sınıfı örneği başlatır. |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Yeni bir [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Satır indeksini alır. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Sütun indeksini alır. |
|
|  | [getRowSpan()](#getRowSpan--) | Tablo hücresini içeren toplam satır sayısını alır. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Tablo hücresini içeren toplam sütun sayısını alır. |
|
|  | [getPageArea()](#getPageArea--) | Tablo hücresi değerini alır. |
|
|  | [getText()](#getText--) | Tablo hücresi metin değerini alır. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Yeni bir [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rowIndex | int | Satırın sıfır tabanlı indeksidir. |
|
|  | columnIndex | int | Sütunun sıfır tabanlı indeksidir. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Tablo hücresinin değeridir. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Yeni bir [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rowIndex | int | Satırın sıfır tabanlı indeksidir. |
|
|  | columnIndex | int | Sütunun sıfır tabanlı indeksidir. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Tablo hücresinin değeridir. |
|
|  | rowSpan | int | Tablo hücresini içeren toplam satır sayısıdır. |
|
|  | columnSpan | int | Tablo hücresini içeren toplam sütun sayısı. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Satır indeksini alır.


**Returns:**
int - Tablo hücresini içeren ilk satırın sıfır tabanlı indeksi.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Sütun indeksini alır.


**Returns:**
int - Tablo hücresini içeren ilk sütunun sıfır tabanlı indeksi.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Tablo hücresini içeren toplam satır sayısını alır.


**Returns:**
int - Tablo hücresini içeren toplam satır sayısını temsil eden pozitif tam sayı değeri.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Tablo hücresini içeren toplam sütun sayısını alır.


**Returns:**
int - Tablo hücresini içeren toplam sütun sayısını temsil eden pozitif tam sayı değeri.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Tablo hücresi değerini alır.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Tablo hücresi metin değerini alır.


**Returns:**
java.lang.String - Hücrenin metin değerini temsil eden bir dize; hücre metin değeri içermiyorsa  null  .

