---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller data för  metoden."
type: docs
weight: 17
url: /sv/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Tillhandahåller data för metoden [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Initierar en ny instans av klassen [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) med rektangulärt område. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getUri()](#getUri--) | Hämtar URI:n för den externa resursen. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Hämtar URI:n för den externa resursen. |
|
|  | [isSkipped()](#isSkipped--) | Hämtar värdet som indikerar om inläsning av den externa resursen ska hoppas över. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Ställer in värdet som indikerar om inläsning av den externa resursen ska hoppas över. |
|
|  | [getData()](#getData--) | Hämtar användardata. |
|
|  | [setData(byte[] data)](#setData-byte---) | Ställer in användardata. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Initierar en ny instans av klassen [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) med rektangulärt område.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | uri | java.lang.String | URI för den externa resursen. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Hämtar URI:n för den externa resursen.


**Returns:**
java.lang.String – En strängvärde som representerar URI för den externa resursen.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Hämtar URI:n för den externa resursen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | uri | java.lang.String | Ett strängvärde som representerar en ny URI för den externa resursen. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Hämtar värdet som indikerar om inläsning av den externa resursen ska hoppas över.


**Returns:**
boolean - true om laddningen av den externa resursen måste hoppas över; annars false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Ställer in värdet som indikerar om inläsning av den externa resursen ska hoppas över.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | hoppad över | boolean | true om laddningen av den externa resursen måste hoppas över; annars false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Hämtar användardata.


**Returns:**
byte[] - Bytearrayen med användarens innehåll för den externa resursen. null om den inte är satt.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Ställer in användardata.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | byte[] | Bytearrayen med användarens innehåll för den externa resursen. null om den inte är satt. |
|

