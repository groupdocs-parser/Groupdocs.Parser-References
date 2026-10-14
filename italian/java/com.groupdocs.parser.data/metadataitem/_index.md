---
title: "MetadataItem"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un elemento di metadati che è usato negli elementi contenitore e nella funzionalità di estrazione dei metadati."
type: docs
weight: 15
url: /it/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Rappresenta un elemento di metadati che è usato negli elementi contenitore e nella funzionalità di estrazione dei metadati.

Un'istanza della classe [MetadataItem](../../com.groupdocs.parser.data/metadataitem) è utilizzata come valore di ritorno del metodo [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
e come elemento nella collezione [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). Vedi gli esempi d'uso lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getName()](#getName--) | Restituisce il nome dell'elemento di metadati. |
|
|  | [getValue()](#getValue--) | Restituisce il valore dell'elemento di metadati. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Inizializza una nuova istanza della classe [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | name | java.lang.String | Il nome dell'elemento di metadati. |
|
|  | valore | java.lang.String | Il valore dell'elemento di metadati. |
|

### getName() {#getName--}
```
public String getName()
```


Restituisce il nome dell'elemento di metadati.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome dell'elemento di metadati.

### getValue() {#getValue--}
```
public String getValue()
```


Restituisce il valore dell'elemento di metadati.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il valore dell'elemento di metadati.

