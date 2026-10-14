---
title: "ExternalResourceLoadingArgs"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les données pour la méthode."
type: docs
weight: 17
url: /fr/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Fournit les données pour la méthode [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Constructors

| Constructor | Description |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Initialise une nouvelle instance de la classe [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) avec une zone rectangulaire. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getUri()](#getUri--) | Obtient l'URI de la ressource externe. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Obtient l'URI de la ressource externe. |
|
|  | [isSkipped()](#isSkipped--) | Obtient la valeur qui indique si le chargement de la ressource externe doit être ignoré. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Définit la valeur qui indique si le chargement de la ressource externe doit être ignoré. |
|
|  | [getData()](#getData--) | Obtient les données utilisateur. |
|
|  | [setData(byte[] data)](#setData-byte---) | Définit les données utilisateur. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Initialise une nouvelle instance de la classe [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) avec une zone rectangulaire.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | uri | java.lang.String | URI de la ressource externe. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Obtient l'URI de la ressource externe.


**Returns:**
java.lang.String - Une valeur chaîne qui représente l'URI de la ressource externe.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Obtient l'URI de la ressource externe.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | uri | java.lang.String | Une valeur chaîne qui représente un nouvel URI de la ressource externe. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Obtient la valeur qui indique si le chargement de la ressource externe doit être ignoré.


**Returns:**
boolean - vrai si le chargement de la ressource externe doit être ignoré ; sinon, faux.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Définit la valeur qui indique si le chargement de la ressource externe doit être ignoré.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | ignoré | boolean | true si le chargement de la ressource externe doit être ignoré ; sinon, false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Obtient les données utilisateur.


**Returns:**
byte[] - Le tableau d'octets contenant le contenu utilisateur de la ressource externe. null si n'est pas défini.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Définit les données utilisateur.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | données | byte[] | Le tableau d'octets contenant le contenu utilisateur de la ressource externe. null si n'est pas défini. |
|

