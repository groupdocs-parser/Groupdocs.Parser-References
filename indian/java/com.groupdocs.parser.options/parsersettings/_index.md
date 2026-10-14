---
title: "ParserSettings"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "डेटा निष्कर्षण को कस्टमाइज़ करने के लिए उपयोग किए जाने वाले सेटिंग्स प्रदान करता है।"
type: docs
weight: 33
url: /hi/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

डेटा निष्कर्षण को कस्टमाइज़ करने के लिए उपयोग किए जाने वाले सेटिंग्स प्रदान करता है।

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | लॉगर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | OCR कनेक्टर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | बाहरी संसाधन हैंडलर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | लॉगर और OCR कनेक्टर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getLogger()](#getLogger--) | डेटा निष्कर्षण के दौरान घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किया जाने वाला लॉगर प्राप्त करता है। |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR कार्यक्षमता प्रदान करने के लिए उपयोग किया जाने वाला OCR कनेक्टर प्राप्त करता है। |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | बाहरी संसाधनों के लिए हैंडलर प्राप्त करता है। |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


लॉगर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) इंटरफ़ेस को लागू करने वाली क्लास का एक उदाहरण। |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


OCR कनेक्टर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR कार्यक्षमता प्रदान करने के लिए [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) क्लास को विरासत में लेने वाली क्लास का एक उदाहरण। |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


बाहरी संसाधन हैंडलर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | OCR कार्यक्षमता प्रदान करने के लिए [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) क्लास को विरासत में लेने वाली क्लास का एक उदाहरण। |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


लॉगर और OCR कनेक्टर के साथ [ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) इंटरफ़ेस को लागू करने वाली क्लास का एक उदाहरण। |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR कार्यक्षमता प्रदान करने के लिए [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) क्लास को विरासत में लेने वाली क्लास का एक उदाहरण। |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


[ParserSettings](../../com.groupdocs.parser.options/parsersettings) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) इंटरफ़ेस को लागू करने वाली क्लास का एक उदाहरण। |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR कार्यक्षमता प्रदान करने के लिए [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) क्लास को विरासत में लेने वाली क्लास का एक उदाहरण। |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | बाहरी संसाधन लोडिंग को नियंत्रित करने के लिए [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) क्लास को विरासत में लेने वाली क्लास का एक उदाहरण। |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


डेटा निष्कर्षण के दौरान घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किया जाने वाला लॉगर प्राप्त करता है।


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


OCR कार्यक्षमता प्रदान करने के लिए उपयोग किया जाने वाला OCR कनेक्टर प्राप्त करता है।


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


बाहरी संसाधनों के लिए हैंडलर प्राप्त करता है।


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

