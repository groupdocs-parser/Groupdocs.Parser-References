---
title: MetadataItem
second_title: GroupDocs.Parser for Java API Reference
description: Represents a metadata item which is used in container items and metadata extraction functionality.
type: docs
weight: 15
url: /java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Represents a metadata item which is used in container items and metadata extraction functionality.

An instance of [MetadataItem](../../com.groupdocs.parser.data/metadataitem) class is used as return value of [Parser.getMetadata()](../../com.groupdocs.parser/parser\#getMetadata--) method and as a item in [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem\#getMetadata--) collection. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Initializes a new instance of the [MetadataItem](../../com.groupdocs.parser.data/metadataitem) class. |
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--) | Gets the name of the metadata item. |
| [getValue()](#getValue--) | Gets the value of the metadata item. |
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Initializes a new instance of the [MetadataItem](../../com.groupdocs.parser.data/metadataitem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the metadata item. |
| value | java.lang.String | The value of the metadata item. |

### getName() {#getName--}
```
public String getName()
```


Gets the name of the metadata item.

**Returns:**
java.lang.String - A string value that represents the name of the metadata item.
### getValue() {#getValue--}
```
public String getValue()
```


Gets the value of the metadata item.

**Returns:**
java.lang.String - A string value that represents the value of the metadata item.
