---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "method के लिए डेटा प्रदान करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

डेटा प्रदान करता है [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) मेथड के लिए।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | आयताकार क्षेत्र के साथ [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getUri()](#getUri--) | बाहरी संसाधन का URI प्राप्त करता है। |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | बाहरी संसाधन का URI प्राप्त करता है। |
|
|  | [isSkipped()](#isSkipped--) | बाहरी संसाधन के लोडिंग को छोड़ना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | बाहरी संसाधन के लोडिंग को छोड़ना चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
|  | [getData()](#getData--) | उपयोगकर्ता डेटा प्राप्त करता है। |
|
|  | [setData(byte[] data)](#setData-byte---) | उपयोगकर्ता डेटा सेट करता है। |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


आयताकार क्षेत्र के साथ [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | uri | java.lang.String | बाहरी संसाधन का URI। |
|

### getUri() {#getUri--}
```
public String getUri()
```


बाहरी संसाधन का URI प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो बाहरी संसाधन के URI का प्रतिनिधित्व करता है।

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


बाहरी संसाधन का URI प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | uri | java.lang.String | एक स्ट्रिंग मान जो बाहरी संसाधन के नए URI का प्रतिनिधित्व करता है। |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


बाहरी संसाधन के लोडिंग को छोड़ना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean - यदि बाहरी संसाधन का लोडिंग छोड़ना चाहिए तो true; अन्यथा false।

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


बाहरी संसाधन के लोडिंग को छोड़ना चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | छोड़ा गया | boolean | यदि बाहरी संसाधन का लोडिंग छोड़ना चाहिए तो true; अन्यथा false। |
|

### getData() {#getData--}
```
public byte[] getData()
```


उपयोगकर्ता डेटा प्राप्त करता है।


**Returns:**
byte[] - बाहरी संसाधन के उपयोगकर्ता सामग्री के साथ बाइट एरे। यदि सेट नहीं है तो null।

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


उपयोगकर्ता डेटा सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | byte[] | बाइट एरे जिसमें बाहरी संसाधन की उपयोगकर्ता सामग्री है। यदि सेट नहीं है तो null। |
|

