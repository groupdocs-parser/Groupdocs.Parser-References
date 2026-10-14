---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "EWS प्रोटोकॉल के लिए ईमेल कनेक्शन जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

EWS प्रोटोकॉल के लिए ईमेल कनेक्शन जानकारी का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | नए [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | नए [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | मेलबॉक्स का URI प्राप्त करता है। |
|
|  | [getDomain()](#getDomain--) | डोमेन नाम प्राप्त करता है। |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


नए [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | मेलबॉक्स का URI। |
|
|  | userName | java.lang.String | उपयोगकर्ता नाम। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड। |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


नए [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | मेलबॉक्स का URI। |
|
|  | domain | java.lang.String | डोमेन नाम। |
|
|  | userName | java.lang.String | उपयोगकर्ता नाम। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड। |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


मेलबॉक्स का URI प्राप्त करता है।


**Returns:**
java.lang.String - स्ट्रिंग मान जो मेलबॉक्स के URI को दर्शाता है।

### getDomain() {#getDomain--}
```
public String getDomain()
```


डोमेन नाम प्राप्त करता है।


**Returns:**
java.lang.String - स्ट्रिंग मान जो डोमेन नाम को दर्शाता है।

