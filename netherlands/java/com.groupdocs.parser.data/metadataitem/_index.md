---
title: "MetadataItem"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een metadata‑item voor dat wordt gebruikt in containeritems en de functionaliteit voor metadata‑extractie."
type: docs
weight: 15
url: /nl/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Stelt een metadata‑item voor dat wordt gebruikt in containeritems en de functionaliteit voor metadata‑extractie.

Een instantie van de [MetadataItem](../../com.groupdocs.parser.data/metadataitem) klasse wordt gebruikt als retourwaarde van de [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) methode.
en als een item in de [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) collectie. Zie daar de gebruiksvoorbeelden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Initialiseert een nieuwe instantie van de [MetadataItem](../../com.groupdocs.parser.data/metadataitem) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getName()](#getName--) | Haalt de naam van het metadata-item op. |
|
|  | [getValue()](#getValue--) | Haalt de waarde van het metadata-item op. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Initialiseert een nieuwe instantie van de [MetadataItem](../../com.groupdocs.parser.data/metadataitem) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | naam | java.lang.String | De naam van het metadata-item. |
|
|  | waarde | java.lang.String | De waarde van het metadata-item. |
|

### getName() {#getName--}
```
public String getName()
```


Haalt de naam van het metadata-item op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de naam van het metadata-item vertegenwoordigt.

### getValue() {#getValue--}
```
public String getValue()
```


Haalt de waarde van het metadata-item op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de waarde van het metadata-item vertegenwoordigt.

