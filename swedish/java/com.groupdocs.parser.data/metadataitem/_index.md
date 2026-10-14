---
title: "MetadataItem"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett metadataobjekt som används i containerobjekt och metadataextraktionsfunktionalitet."
type: docs
weight: 15
url: /sv/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Representerar ett metadataobjekt som används i containerobjekt och metadataextraktionsfunktionalitet.

En instans av klassen [MetadataItem](../../com.groupdocs.parser.data/metadataitem) används som returvärde för metoden [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
och som ett objekt i samlingen [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) . Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getName()](#getName--) | Hämtar namnet på metadataobjektet. |
|
|  | [getValue()](#getValue--) | Hämtar värdet på metadataobjektet. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Initierar en ny instans av klassen [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | namn | java.lang.String | Namnet på metadataobjektet. |
|
|  | värde | java.lang.String | Värdet på metadataobjektet. |
|

### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på metadataobjektet.


**Returns:**
java.lang.String - Ett strängvärde som representerar namnet på metadataobjektet.

### getValue() {#getValue--}
```
public String getValue()
```


Hämtar värdet på metadataobjektet.


**Returns:**
java.lang.String - Ett strängvärde som representerar värdet på metadataobjektet.

