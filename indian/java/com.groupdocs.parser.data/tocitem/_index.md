---
title: "TocItem"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेबल ऑफ कंटेंट्स निष्कर्षण कार्यक्षमता में उपयोग किए जाने वाले आइटम का प्रतिनिधित्व करता है।"
type: docs
weight: 31
url: /hi/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

टेबल ऑफ कंटेंट्स निष्कर्षण कार्यक्षमता में उपयोग किए जाने वाले आइटम का प्रतिनिधित्व करता है।

एक उदाहरण [TocItem](../../com.groupdocs.parser.data/tocitem) क्लास का उपयोग [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) मेथड के रिटर्न वैल्यू के रूप में किया जाता है। वहाँ उपयोग उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | TocItem क्लास का नया उदाहरण इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getDepth()](#getDepth--) | गहराई स्तर प्राप्त करता है। |
|
|  | [getText()](#getText--) | टेक्स्ट प्राप्त करता है। |
|
|  | [getPageIndex()](#getPageIndex--) | पेज इंडेक्स प्राप्त करता है। |
|
|  | [extractText()](#extractText--) | दस्तावेज़ से वह पाठ निकालता है जिससे TocItem ऑब्जेक्ट संबंधित है। |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


TocItem क्लास का नया उदाहरण इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | depth | int | आइटम का गहराई स्तर। |
|
|  | पाठ | java.lang.String | आइटम का पाठ। |
|
|  | pageIndex | java.lang.Integer | आइटम द्वारा संदर्भित पृष्ठ का इंडेक्स |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


गहराई स्तर प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो आइटम के गहराई स्तर को दर्शाता है।

### getText() {#getText--}
```
public String getText()
```


टेक्स्ट प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो आइटम के पाठ को दर्शाता है।

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


पेज इंडेक्स प्राप्त करता है।


**Returns:**
java.lang.Integer - एक पूर्णांक मान जो आइटम द्वारा संदर्भित पृष्ठ के इंडेक्स को दर्शाता है; यदि सेट नहीं है तो  null  ।

### extractText() {#extractText--}
```
public TextReader extractText()
```


दस्तावेज़ से वह पाठ निकालता है जिससे TocItem ऑब्जेक्ट संबंधित है।

निम्नलिखित उदाहरण दर्शाता है कि तालिका सामग्री के एक आइटम द्वारा पाठ कैसे निकाला जाए:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

