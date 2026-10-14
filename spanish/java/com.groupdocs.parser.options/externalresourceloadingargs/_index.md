---
title: "ExternalResourceLoadingArgs"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona los datos para el método."
type: docs
weight: 17
url: /es/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Proporciona los datos para el método [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Inicializa una nueva instancia de la clase [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) con un área rectangular. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getUri()](#getUri--) | Obtiene el URI del recurso externo. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Obtiene el URI del recurso externo. |
|
|  | [isSkipped()](#isSkipped--) | Obtiene el valor que indica si la carga del recurso externo debe omitirse. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Establece el valor que indica si la carga del recurso externo debe omitirse. |
|
|  | [getData()](#getData--) | Obtiene los datos del usuario. |
|
|  | [setData(byte[] data)](#setData-byte---) | Establece los datos del usuario. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Inicializa una nueva instancia de la clase [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) con un área rectangular.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | uri | java.lang.String | URI del recurso externo. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Obtiene el URI del recurso externo.


**Returns:**
java.lang.String - Un valor de cadena que representa el URI del recurso externo.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Obtiene el URI del recurso externo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | uri | java.lang.String | Un valor de cadena que representa un nuevo URI del recurso externo. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Obtiene el valor que indica si la carga del recurso externo debe omitirse.


**Returns:**
boolean - verdadero si la carga del recurso externo debe omitirse; de lo contrario, falso.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Establece el valor que indica si la carga del recurso externo debe omitirse.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | omitido | boolean | verdadero si la carga del recurso externo debe omitirse; de lo contrario, falso. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Obtiene los datos del usuario.


**Returns:**
byte[] - La matriz de bytes con el contenido del usuario del recurso externo. null si no está establecida.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Establece los datos del usuario.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | byte[] | La matriz de bytes con el contenido del usuario del recurso externo. null si no está configurado. |
|

