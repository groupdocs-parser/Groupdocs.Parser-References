---
title: "QualityMode"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "गुणवत्ता के स्तर को परिभाषित करता है।"
type: docs
weight: 48
url: /hi/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

गुणवत्ता के स्तर को परिभाषित करता है।

## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [High](#High) | उच्च गुणवत्ता। |
|
|  | [Normal](#Normal) | सामान्य गुणवत्ता। |
|
|  | [Low](#Low) | निम्न गुणवत्ता। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


उच्च गुणवत्ता। तेज़ प्रसंस्करण एल्गोरिदम का उपयोग किया जाता है।


### Normal {#Normal}
```
public static final QualityMode Normal
```


सामान्य गुणवत्ता। डिफ़ॉल्ट प्रसंस्करण एल्गोरिदम का उपयोग किया जाता है।


### Low {#Low}
```
public static final QualityMode Low
```


निम्न गुणवत्ता। धीमी प्रसंस्करण एल्गोरिदम का उपयोग किया जाता है।


### values() {#values--}
```
public static QualityMode[] values()
```




**Returns:**
com.groupdocs.parser.options.QualityMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static QualityMode valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
