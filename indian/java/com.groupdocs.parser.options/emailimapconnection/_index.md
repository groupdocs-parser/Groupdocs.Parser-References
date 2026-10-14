---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "IMAP प्रोटोकॉल के लिए ईमेल कनेक्शन जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

IMAP प्रोटोकॉल के लिए ईमेल कनेक्शन जानकारी का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | नए [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) क्लास का एक नया उदाहरण आरंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getHost()](#getHost--) | होस्ट नाम प्राप्त करता है। |
|
|  | [getPort()](#getPort--) | पोर्ट संख्या प्राप्त करता है। |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


नए [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) क्लास का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | host | java.lang.String | होस्ट नाम। |
|
|  | port | int | पोर्ट संख्या। |
|
|  | userName | java.lang.String | उपयोगकर्ता नाम। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड। |
|

### getHost() {#getHost--}
```
public String getHost()
```


होस्ट नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो होस्ट नाम का प्रतिनिधित्व करता है।

### getPort() {#getPort--}
```
public int getPort()
```


पोर्ट संख्या प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो पोर्ट नंबर का प्रतिनिधित्व करता है।

