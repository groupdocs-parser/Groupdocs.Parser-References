---
title: "लाइसेंस"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "GroupDocs.Parser लाइसेंस का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

GroupDocs.Parser लाइसेंस का प्रतिनिधित्व करता है।

यह उदाहरण लाइसेंस सेटअप करने का तरीका दर्शाता है।

````
 ```

// लाइसेंस क्लास को प्रारंभ करें
License license = new License();
// .lic फ़ाइल का पथ सेट करें
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [License()](#License--) | नए उदाहरण को प्रारंभ करता है [License](../../com.groupdocs.parser.licensing/license) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | घटक को लाइसेंस देता है। |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | घटक को लाइसेंस देता है। |
|
### License() {#License--}
```
public License()
```


नए उदाहरण को प्रारंभ करता है [License](../../com.groupdocs.parser.licensing/license) क्लास का।


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


घटक को लाइसेंस देता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | लाइसेंस फ़ाइल का पूर्ण पथ। |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


घटक को लाइसेंस देता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | stream | java.io.InputStream | लाइसेंस स्ट्रीम। |
|

