---
title: EmailPopConnection
second_title: GroupDocs.Parser for Java API Reference
description: Represents the email connection information for POP protocol.
type: docs
weight: 15
url: /java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

Represents the email connection information for POP protocol.
## Constructors

| Constructor | Description |
| --- | --- |
| [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initializes a new instance of the [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) class. |
## Methods

| Method | Description |
| --- | --- |
| [getHost()](#getHost--) | Gets the host name. |
| [getPort()](#getPort--) | Gets the port number. |
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


Initializes a new instance of the [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| host | java.lang.String | The host name. |
| port | int | The port number. |
| userName | java.lang.String | The user name. |
| password | java.lang.String | The password. |

### getHost() {#getHost--}
```
public String getHost()
```


Gets the host name.

**Returns:**
java.lang.String - A string value that represents the host name.
### getPort() {#getPort--}
```
public int getPort()
```


Gets the port number.

**Returns:**
int - An integer value that represents the port number.
