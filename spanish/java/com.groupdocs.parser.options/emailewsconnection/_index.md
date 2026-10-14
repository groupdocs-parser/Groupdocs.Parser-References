---
title: "EmailEwsConnection"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información de conexión del correo electrónico para el protocolo EWS."
type: docs
weight: 13
url: /es/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Representa la información de conexión del correo electrónico para el protocolo EWS.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Obtiene el URI del buzón. |
|
|  | [getDomain()](#getDomain--) | Obtiene el nombre de dominio. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Inicializa una nueva instancia de la clase [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | El URI del buzón. |
|
|  | userName | java.lang.String | El nombre de usuario. |
|
|  | contraseña | java.lang.String | La contraseña. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Inicializa una nueva instancia de la clase [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | El URI del buzón. |
|
|  | domain | java.lang.String | El nombre de dominio. |
|
|  | userName | java.lang.String | El nombre de usuario. |
|
|  | contraseña | java.lang.String | La contraseña. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Obtiene el URI del buzón.


**Returns:**
java.lang.String - Un valor de cadena que representa un URI del buzón.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Obtiene el nombre de dominio.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre de dominio.

