---
title: "EmailPopConnection"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información de conexión del correo electrónico para el protocolo POP."
type: docs
weight: 15
url: /es/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

Representa la información de conexión del correo electrónico para el protocolo POP.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getHost()](#getHost--) | Obtiene el nombre del host. |
|
|  | [getPort()](#getPort--) | Obtiene el número de puerto. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


Inicializa una nueva instancia de la clase [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | host | java.lang.String | El nombre del host. |
|
|  | port | int | El número de puerto. |
|
|  | userName | java.lang.String | El nombre de usuario. |
|
|  | contraseña | java.lang.String | La contraseña. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Obtiene el nombre del host.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre de host.

### getPort() {#getPort--}
```
public int getPort()
```


Obtiene el número de puerto.


**Returns:**
int - Un valor entero que representa el número de puerto.

