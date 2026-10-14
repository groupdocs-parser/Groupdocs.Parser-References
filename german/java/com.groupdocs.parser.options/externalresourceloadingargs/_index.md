---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Daten für die Methode bereit."
type: docs
weight: 17
url: /de/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Stellt die Daten für die Methode [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) mit rechteckigem Bereich. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getUri()](#getUri--) | Gibt die URI der externen Ressource zurück. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Gibt die URI der externen Ressource zurück. |
|
|  | [isSkipped()](#isSkipped--) | Ermittelt den Wert, der angibt, ob das Laden der externen Ressource übersprungen werden muss. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Legt den Wert fest, der angibt, ob das Laden der externen Ressource übersprungen werden muss. |
|
|  | [getData()](#getData--) | Ermittelt die Benutzerdaten. |
|
|  | [setData(byte[] data)](#setData-byte---) | Legt die Benutzerdaten fest. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Initialisiert eine neue Instanz der Klasse [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) mit rechteckigem Bereich.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | URI | java.lang.String | URI der externen Ressource. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Gibt die URI der externen Ressource zurück.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der die URI der externen Ressource darstellt.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Gibt die URI der externen Ressource zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | URI | java.lang.String | Ein Zeichenkettenwert, der eine neue URI der externen Ressource darstellt. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Ermittelt den Wert, der angibt, ob das Laden der externen Ressource übersprungen werden muss.


**Returns:**
boolean - true, wenn das Laden der externen Ressource übersprungen werden muss; andernfalls false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Legt den Wert fest, der angibt, ob das Laden der externen Ressource übersprungen werden muss.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | übersprungen | boolean | true, wenn das Laden der externen Ressource übersprungen werden muss; andernfalls false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Ermittelt die Benutzerdaten.


**Returns:**
byte[] - Das Byte-Array mit dem Benutzerinhalt der externen Ressource. null, wenn nicht gesetzt.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Legt die Benutzerdaten fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | byte[] | Das Byte-Array mit dem Benutzerinhalt der externen Ressource. null, wenn nicht gesetzt. |
|

