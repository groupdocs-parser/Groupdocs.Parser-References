---
title: "MetadataItem"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un elemento de metadatos que se utiliza en elementos contenedores y en la funcionalidad de extracción de metadatos."
type: docs
weight: 15
url: /es/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Representa un elemento de metadatos que se utiliza en elementos contenedores y en la funcionalidad de extracción de metadatos.

Una instancia de la clase [MetadataItem](../../com.groupdocs.parser.data/metadataitem) se utiliza como valor de retorno del método [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
y como un elemento en la colección [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). Consulte los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la clase [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getName()](#getName--) | Obtiene el nombre del elemento de metadatos. |
|
|  | [getValue()](#getValue--) | Obtiene el valor del elemento de metadatos. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Inicializa una nueva instancia de la clase [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | nombre | java.lang.String | El nombre del elemento de metadatos. |
|
|  | valor | java.lang.String | El valor del elemento de metadatos. |
|

### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del elemento de metadatos.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre del elemento de metadatos.

### getValue() {#getValue--}
```
public String getValue()
```


Obtiene el valor del elemento de metadatos.


**Returns:**
java.lang.String - Un valor de cadena que representa el valor del elemento de metadatos.

