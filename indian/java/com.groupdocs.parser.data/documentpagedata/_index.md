---
title: "DocumentPageData"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "दस्तावेज़ पृष्ठ का डेटा दर्शाता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

दस्तावेज़ पृष्ठ के डेटा का प्रतिनिधित्व करता है। यह [FieldData](../../com.groupdocs.parser.data/fielddata) ऑब्जेक्ट्स से बना है जो दस्तावेज़ पृष्ठ से फ़ील्ड डेटा रखते हैं।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | नए उदाहरण को प्रारंभ करता है [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | पेज इंडेक्स प्राप्त करता है। |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


नए उदाहरण को प्रारंभ करता है [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fields | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | फ़ील्ड डेटा का संग्रह। |
|
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


पेज इंडेक्स प्राप्त करता है।


**Returns:**
int - पृष्ठ का शून्य-आधारित सूचकांक।

