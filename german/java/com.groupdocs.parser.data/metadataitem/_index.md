---
title: "MetadataItem"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt ein Metadaten‑Element dar, das in Containerelementen und der Metadaten‑Extraktionsfunktion verwendet wird."
type: docs
weight: 15
url: /de/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Stellt ein Metadaten‑Element dar, das in Containerelementen und der Metadaten‑Extraktionsfunktion verwendet wird.

Eine Instanz der Klasse [MetadataItem](../../com.groupdocs.parser.data/metadataitem) wird als Rückgabewert der Methode [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) verwendet.
und als Element in der Sammlung von [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getName()](#getName--) | Liefert den Namen des Metadaten‑Elements. |
|
|  | [getValue()](#getValue--) | Liefert den Wert des Metadaten‑Elements. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Initialisiert eine neue Instanz der Klasse [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Name | java.lang.String | Der Name des Metadaten‑Elements. |
|
|  | Wert | java.lang.String | Der Wert des Metadaten‑Elements. |
|

### getName() {#getName--}
```
public String getName()
```


Liefert den Namen des Metadaten‑Elements.


**Returns:**
java.lang.String - Ein String‑Wert, der den Namen des Metadaten‑Elements darstellt.

### getValue() {#getValue--}
```
public String getValue()
```


Liefert den Wert des Metadaten‑Elements.


**Returns:**
java.lang.String - Ein String‑Wert, der den Wert des Metadaten‑Elements darstellt.

