---
title: "PageTableArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में तालिका को दर्शाने के लिए उपयोग किए जाने वाले तालिका पृष्ठ क्षेत्र का प्रतिनिधित्व करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में तालिका को दर्शाने के लिए उपयोग किए जाने वाले तालिका पृष्ठ क्षेत्र का प्रतिनिधित्व करता है।

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | एक नई इंस्टेंस को प्रारंभ करता है [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) क्लास की। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getCells()](#getCells--) | सेलों का संग्रह प्राप्त करता है। |
|
|  | [getRowCount()](#getRowCount--) | टेबल पंक्तियों की कुल संख्या प्राप्त करता है। |
|
|  | [getColumnCount()](#getColumnCount--) | टेबल कॉलमों की कुल संख्या प्राप्त करता है। |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | पंक्ति की ऊँचाई लौटाता है। |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | कॉलम की चौड़ाई लौटाता है। |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | पंक्ति और कॉलम सूचकांकों द्वारा टेबल सेल प्राप्त करता है। |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


एक नई इंस्टेंस को प्रारंभ करता है [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) क्लास की।

नोट: C# प्रोजेक्ट इस कंस्ट्रक्टर को इस रूप में चिह्नित करता है
आंतरिक
(commit 954951f). जावा में, \"internal-to-the-assembly\"
पैकेज-प्राइवेट में साफ़ तौर पर अनुवाद नहीं होता क्योंकि उत्पादक (
WordProcessingParser
,
TableAreaParser
,
इत्यादि) में स्थित हैं
com.groupdocs.parser
, नहीं
com.groupdocs.parser.data
. इसलिए कंस्ट्रक्टर को रखा गया है

सार्वजनिक
इसलिए क्रॉस-पैकेज निर्माण अभी भी काम करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पंक्तियाँ | java.lang.Iterable<java.lang.Double> | पंक्तियों की ऊँचाइयों का संग्रह। |
|
|  | स्तंभ | java.lang.Iterable<java.lang.Double> | स्तंभों की चौड़ाइयों का संग्रह। |
|
|  | सेल्स | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | सेल्स का संग्रह। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | वह पृष्ठ जिसमें तालिका सम्मिलित है। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | आयताकार क्षेत्र जो टेबल को समाहित करता है। |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


सेल्स का संग्रह प्राप्त करता है। तालिका सेल्स का एक साधारण केवल-पढ़ने योग्य संग्रह।


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - तालिका सेल्स का संग्रह

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


टेबल पंक्तियों की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो तालिका की पंक्तियों की कुल संख्या रखता है।

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


टेबल कॉलमों की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो तालिका के स्तंभों की कुल संख्या रखता है।

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


पंक्ति की ऊँचाई लौटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rowIndex | int | पंक्ति का शून्य-आधारित सूचकांक। |
|

**Returns:**
double - एक डबल मान जो पंक्ति की ऊँचाई दर्शाता है।

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


कॉलम की चौड़ाई लौटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | columnIndex | int | स्तंभ का शून्य-आधारित सूचकांक। |
|

**Returns:**
double - कॉलम की चौड़ाई का प्रतिनिधित्व करने वाला एक double मान।

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


पंक्ति और कॉलम सूचकांकों द्वारा टेबल सेल प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rowIndex | int | सेल पंक्ति का शून्य-आधारित सूचकांक। |
|
|  | columnIndex | int | सेल कॉलम का शून्य-आधारित सूचकांक। |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

