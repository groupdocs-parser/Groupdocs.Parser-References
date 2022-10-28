---
title: EmailImapConnection
second_title: GroupDocs.Parser for Java API Reference
description: Represents the email connection information for IMAP protocol.
type: docs
weight: 13
url: /java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Represents the email connection information for IMAP protocol.
## Constructors

| Constructor | Description |
| --- | --- |
| [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initializes a new instance of the [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) class. |
## Methods

| Method | Description |
| --- | --- |
| [getHost()](#getHost--) | Gets the host name. |
| [getPort()](#getPort--) | Gets the port number. |
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Initializes a new instance of the [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) class.

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
