---
title: "ExternalResourceHandler"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "बाहरी संसाधनों के लोडिंग के लिए हैंडलर प्रदान करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

बाहरी संसाधनों के लोडिंग के लिए हैंडलर प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | किसी भी बाहरी संसाधन लोड होने से पहले बुलाया जाता है। |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


किसी भी बाहरी संसाधन लोड होने से पहले बुलाया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | बाहरी संसाधन लोडिंग को नियंत्रित करने के लिए डेटा। |
|

