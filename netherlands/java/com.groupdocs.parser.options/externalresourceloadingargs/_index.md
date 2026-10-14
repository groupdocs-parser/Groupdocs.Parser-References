---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Levert de gegevens voor de methode."
type: docs
weight: 17
url: /nl/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Levert de gegevens voor de [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) methode.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Initialiseert een nieuw exemplaar van de [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) klasse met een rechthoekig gebied. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getUri()](#getUri--) | Haalt de URI van de externe bron op. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Haalt de URI van de externe bron op. |
|
|  | [isSkipped()](#isSkipped--) | Haalt de waarde op die aangeeft of het laden van de externe bron moet worden overgeslagen. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Stelt de waarde in die aangeeft of het laden van de externe bron moet worden overgeslagen. |
|
|  | [getData()](#getData--) | Haalt de gebruikersgegevens op. |
|
|  | [setData(byte[] data)](#setData-byte---) | Stelt de gebruikersgegevens in. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Initialiseert een nieuw exemplaar van de [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) klasse met een rechthoekig gebied.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | uri | java.lang.String | URI van de externe bron. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Haalt de URI van de externe bron op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de URI van de externe bron vertegenwoordigt.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Haalt de URI van de externe bron op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | uri | java.lang.String | Een tekenreekswaarde die een nieuwe URI van de externe bron vertegenwoordigt. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Haalt de waarde op die aangeeft of het laden van de externe bron moet worden overgeslagen.


**Returns:**
boolean - true als het laden van de externe bron moet worden overgeslagen; anders false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Stelt de waarde in die aangeeft of het laden van de externe bron moet worden overgeslagen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | overgeslagen | boolean | true als het laden van de externe bron moet worden overgeslagen; anders false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Haalt de gebruikersgegevens op.


**Returns:**
byte[] - De byte-array met de gebruikersinhoud van de externe bron. null als deze niet is ingesteld.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Stelt de gebruikersgegevens in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | byte[] | De byte-array met de gebruikersinhoud van de externe bron. null als deze niet is ingesteld. |
|

