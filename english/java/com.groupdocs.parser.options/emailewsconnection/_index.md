---
title: EmailEwsConnection
second_title: GroupDocs.Parser for Java API Reference
description: Represents the email connection information for EWS protocol.
type: docs
weight: 13
url: /java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Represents the email connection information for EWS protocol.
## Constructors

| Constructor | Description |
| --- | --- |
| [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Initializes a new instance of the [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) class. |
| [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Initializes a new instance of the [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) class. |
## Methods

| Method | Description |
| --- | --- |
| [getMailboxUri()](#getMailboxUri--) | Gets the URI of the mailbox. |
| [getDomain()](#getDomain--) | Gets the domain name. |
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Initializes a new instance of the [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mailboxUri | java.lang.String | The URI of mailbox. |
| userName | java.lang.String | The user name. |
| password | java.lang.String | The password. |

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Initializes a new instance of the [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mailboxUri | java.lang.String | The URI of mailbox. |
| domain | java.lang.String | The domain name. |
| userName | java.lang.String | The user name. |
| password | java.lang.String | The password. |

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Gets the URI of the mailbox.

**Returns:**
java.lang.String - A string value that represents a URI of the mailbox.
### getDomain() {#getDomain--}
```
public String getDomain()
```


Gets the domain name.

**Returns:**
java.lang.String - A string value that represents the domain name.
