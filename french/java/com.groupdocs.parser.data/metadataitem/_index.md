---
title: "MetadataItem"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente un élément de métadonnées utilisé dans les éléments de conteneur et la fonctionnalité d'extraction de métadonnées."
type: docs
weight: 15
url: /fr/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Représente un élément de métadonnées utilisé dans les éléments de conteneur et la fonctionnalité d'extraction de métadonnées.

Une instance de la classe [MetadataItem](../../com.groupdocs.parser.data/metadataitem) est utilisée comme valeur de retour de la méthode [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
et comme élément dans la collection [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). Voir les exemples d'utilisation là-bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getName()](#getName--) | Obtient le nom de l'élément de métadonnées. |
|
|  | [getValue()](#getValue--) | Obtient la valeur de l'élément de métadonnées. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Initialise une nouvelle instance de la classe [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | nom | java.lang.String | Le nom de l'élément de métadonnées. |
|
|  | valeur | java.lang.String | La valeur de l'élément de métadonnées. |
|

### getName() {#getName--}
```
public String getName()
```


Obtient le nom de l'élément de métadonnées.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le nom de l'élément de métadonnées.

### getValue() {#getValue--}
```
public String getValue()
```


Obtient la valeur de l'élément de métadonnées.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente la valeur de l'élément de métadonnées.

