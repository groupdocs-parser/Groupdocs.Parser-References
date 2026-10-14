---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "एक तालिका सेल का प्रतिनिधित्व करता है जो  क्लास में उपयोग किया जाता है।"
type: docs
weight: 23
url: /hi/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

एक तालिका सेल का प्रतिनिधित्व करता है जो [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) क्लास में उपयोग किया जाता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | नए उदाहरण को प्रारंभ करता है [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) क्लास का। |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | नए उदाहरण को प्रारंभ करता है [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | पंक्ति सूचकांक प्राप्त करता है। |
|
|  | [getColumnIndex()](#getColumnIndex--) | स्तंभ सूचकांक प्राप्त करता है। |
|
|  | [getRowSpan()](#getRowSpan--) | टेबल सेल को शामिल करने वाली पंक्तियों की कुल संख्या प्राप्त करता है। |
|
|  | [getColumnSpan()](#getColumnSpan--) | टेबल सेल को शामिल करने वाले स्तंभों की कुल संख्या प्राप्त करता है। |
|
|  | [getPageArea()](#getPageArea--) | टेबल सेल मान प्राप्त करता है। |
|
|  | [getText()](#getText--) | टेबल सेल टेक्स्ट मान प्राप्त करता है। |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


नए उदाहरण को प्रारंभ करता है [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rowIndex | int | पंक्ति का शून्य-आधारित सूचकांक। |
|
|  | columnIndex | int | स्तंभ का शून्य-आधारित सूचकांक। |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | टेबल सेल का मान। |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


नए उदाहरण को प्रारंभ करता है [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rowIndex | int | पंक्ति का शून्य-आधारित सूचकांक। |
|
|  | columnIndex | int | स्तंभ का शून्य-आधारित सूचकांक। |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | टेबल सेल का मान। |
|
|  | rowSpan | int | टेबल सेल को शामिल करने वाली पंक्तियों की कुल संख्या। |
|
|  | columnSpan | int | टेबल सेल को शामिल करने वाले स्तंभों की कुल संख्या। |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


पंक्ति सूचकांक प्राप्त करता है।


**Returns:**
int - टेबल सेल को शामिल करने वाली पहली पंक्ति का शून्य-आधारित सूचकांक।

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


स्तंभ सूचकांक प्राप्त करता है।


**Returns:**
int - टेबल सेल को शामिल करने वाले पहले स्तंभ का शून्य-आधारित सूचकांक।

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


टेबल सेल को शामिल करने वाली पंक्तियों की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक सकारात्मक पूर्णांक मान जो टेबल सेल को शामिल करने वाली पंक्तियों की कुल संख्या दर्शाता है।

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


टेबल सेल को शामिल करने वाले स्तंभों की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक सकारात्मक पूर्णांक मान जो टेबल सेल को शामिल करने वाले स्तंभों की कुल संख्या दर्शाता है।

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


टेबल सेल मान प्राप्त करता है।


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


टेबल सेल टेक्स्ट मान प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जो सेल के टेक्स्ट मान को दर्शाती है; यदि सेल में टेक्स्ट मान नहीं है तो null।

