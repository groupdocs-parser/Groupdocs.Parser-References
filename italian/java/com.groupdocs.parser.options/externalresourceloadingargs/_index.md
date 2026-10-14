---
title: "ExternalResourceLoadingArgs"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce i dati per il metodo."
type: docs
weight: 17
url: /it/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Fornisce i dati per il metodo [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Inizializza una nuova istanza della classe [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) con area rettangolare. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getUri()](#getUri--) | Ottiene l'URI della risorsa esterna. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Ottiene l'URI della risorsa esterna. |
|
|  | [isSkipped()](#isSkipped--) | Ottiene il valore che indica se il caricamento della risorsa esterna deve essere saltato. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Imposta il valore che indica se il caricamento della risorsa esterna deve essere saltato. |
|
|  | [getData()](#getData--) | Ottiene i dati dell'utente. |
|
|  | [setData(byte[] data)](#setData-byte---) | Imposta i dati dell'utente. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Inizializza una nuova istanza della classe [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) con area rettangolare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | uri | java.lang.String | URI della risorsa esterna. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Ottiene l'URI della risorsa esterna.


**Returns:**
java.lang.String - Un valore stringa che rappresenta l'URI della risorsa esterna.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Ottiene l'URI della risorsa esterna.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | uri | java.lang.String | Un valore stringa che rappresenta un nuovo URI della risorsa esterna. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Ottiene il valore che indica se il caricamento della risorsa esterna deve essere saltato.


**Returns:**
boolean - true se il caricamento della risorsa esterna deve essere saltato; altrimenti, false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Imposta il valore che indica se il caricamento della risorsa esterna deve essere saltato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | saltato | boolean | true se il caricamento della risorsa esterna deve essere saltato; altrimenti, false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Ottiene i dati dell'utente.


**Returns:**
byte[] - L'array di byte con il contenuto dell'utente della risorsa esterna. null se non è impostato.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Imposta i dati dell'utente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | byte[] | L'array di byte con il contenuto dell'utente della risorsa esterna. null se non è impostato. |
|

