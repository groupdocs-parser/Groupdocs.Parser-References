---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "पेज कैसे रेंडर किया जाता है, इसकी जानकारी को दर्शाता है।"
type: docs
weight: 30
url: /hi/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

पेज कैसे रेंडर किया जाता है, इसकी जानकारी को दर्शाता है।

कुछ दस्तावेज़ (स्प्रेडशीट, उदाहरण के लिए) पृष्ठ को रेंडर करने में असमर्थ होते हैं
एकल छवि के रूप में। उन दस्तावेज़ों के लिए पृष्ठ को टाइलों के सेट के रूप में रेंडर किया जाता है।
इन टाइलों को आयताकार तालिका में रखा जाता है।


RowCount
और
ColumnCount
पंक्तियों और स्तंभों की कुल संख्या को दर्शाते हैं
इस तालिका की। यदि दस्तावेज़ पृष्ठ को एकल छवि में रेंडर किया जाता है तो ये गुण 1 के बराबर होते हैं।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | नए उदाहरण को प्रारंभ करता है [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | पृष्ठ संख्या प्राप्त करता है। |
|
|  | [getRowCount()](#getRowCount--) | टाइल पंक्तियों की कुल संख्या प्राप्त करें। |
|
|  | [getColumnCount()](#getColumnCount--) | टाइल स्तंभों की कुल संख्या प्राप्त करें। |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | उस स्तंभ का सूचकांक लौटाता है जहाँ टाइल के साथ  tileIndex  रखा गया है। |
|
|  | [getRow(int tileIndex)](#getRow-int-) | उस पंक्ति का सूचकांक लौटाता है जहाँ टाइल के साथ  tileIndex  रखा गया है। |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


नए उदाहरण को प्रारंभ करता है [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageNumber | int | पृष्ठ की संख्या (1 से शुरू)। |
|
|  | rowCount | int | टाइल पंक्तियों की कुल संख्या। |
|
|  | columnCount | int | टाइल स्तंभों की कुल संख्या। |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


पृष्ठ संख्या प्राप्त करता है।


**Returns:**
int - वह पूर्णांक मान जो पृष्ठ संख्या को दर्शाता है (1 से शुरू)।

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


टाइल पंक्तियों की कुल संख्या प्राप्त करें।


**Returns:**
int - वह पूर्णांक मान जो टाइल पंक्तियों की कुल संख्या को दर्शाता है।

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


टाइल स्तंभों की कुल संख्या प्राप्त करें।


**Returns:**
int - वह पूर्णांक मान जो टाइल स्तंभों की कुल संख्या को दर्शाता है।

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


उस स्तंभ का सूचकांक लौटाता है जहाँ टाइल के साथ  tileIndex  रखा गया है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | tileIndex | int | टाइल का शून्य-आधारित सूचकांक। |
|

**Returns:**
int - वह शून्य-आधारित पूर्णांक मान जो स्तंभ सूचकांक को दर्शाता है।

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


उस पंक्ति का सूचकांक लौटाता है जहाँ टाइल के साथ  tileIndex  रखा गया है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | tileIndex | int | टाइल का शून्य-आधारित सूचकांक। |
|

**Returns:**
int - वह शून्य-आधारित पूर्णांक मान जो पंक्ति सूचकांक को दर्शाता है।

