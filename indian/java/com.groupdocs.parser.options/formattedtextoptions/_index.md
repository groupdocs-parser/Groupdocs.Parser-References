---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "फ़ॉर्मेटेड टेक्स्ट निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

फ़ॉर्मेटेड टेक्स्ट निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

एक उदाहरण [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) क्लास का पैरामीटर के रूप में [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-) में उपयोग किया जाता है।
और [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) मेथड्स। वहाँ उपयोग के उदाहरण देखें।

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | कोई मोड सेट किए बिना [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | नए [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getMode()](#getMode--) | फ़ॉर्मेटेड टेक्स्ट निष्कर्षण मोड प्राप्त करता है। |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | फ़ॉर्मेटेड टेक्स्ट निष्कर्षण मोड सेट करता है। |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


कोई मोड सेट किए बिना [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) क्लास का नया उदाहरण प्रारंभ करता है।


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


नए [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | फ़ॉर्मेटेड टेक्स्ट निष्कर्षण का मोड। |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


फ़ॉर्मेटेड टेक्स्ट निष्कर्षण मोड प्राप्त करता है।


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


फ़ॉर्मेटेड टेक्स्ट निष्कर्षण मोड सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) एनीमरेशन जिसमें फ़ॉर्मेटेड टेक्स्ट निष्कर्षण मोड शामिल है। |
|

