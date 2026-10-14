---
title: "TemplateOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्पलेट कार्यक्षमता द्वारा पार्सिंग के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

टेम्पलेट कार्यक्षमता द्वारा पार्सिंग के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | एक नया उदाहरण प्रारंभ करता है [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार प्राप्त करता है। |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


एक नया उदाहरण प्रारंभ करता है [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangleTolerance | double | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार। इसे टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार प्राप्त करता है। इसे टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है।


**Returns:**
double - 0 (कोई सीमा नहीं) से 1 (पूरे तत्व को अनदेखा करें) तक का डबल मान।

