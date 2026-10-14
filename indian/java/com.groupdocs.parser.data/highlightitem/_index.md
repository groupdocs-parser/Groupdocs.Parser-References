---
title: "HighlightItem"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "खोज कार्यक्षमता में पाए गए पाठ के संदर्भ को समझाने के लिए आमतौर पर उपयोग किए जाने वाले पाठ के एक भाग को हाइलाइट करने का प्रतिनिधित्व करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

हाइलाइट का प्रतिनिधित्व करता है, जो टेक्स्ट का वह भाग है जिसे आमतौर पर खोज कार्यक्षमता में पाए गए टेक्स्ट के संदर्भ को समझाने के लिए उपयोग किया जाता है।

एक [HighlightItem](../../com.groupdocs.parser.data/highlightitem) वर्ग का उदाहरण [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) मेथड के रिटर्न वैल्यू के रूप में उपयोग किया जाता है,
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) वर्ग का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getPosition()](#getPosition--) | दस्तावेज़ पाठ में स्थिति प्राप्त करता है। |
|
|  | [getText()](#getText--) | हाइलाइट का पाठ प्राप्त करता है। |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


[HighlightItem](../../com.groupdocs.parser.data/highlightitem) वर्ग का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्थिति | int | दस्तावेज़ पाठ में स्थिति। |
|
|  | पाठ | java.lang.String | हाइलाइट का पाठ। |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


दस्तावेज़ पाठ में स्थिति प्राप्त करता है।


**Returns:**
int - हाइलाइट की प्रारंभिक स्थिति का शून्य-आधारित सूचकांक।

### getText() {#getText--}
```
public String getText()
```


हाइलाइट का पाठ प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो हाइलाइट के पाठ का प्रतिनिधित्व करता है।

