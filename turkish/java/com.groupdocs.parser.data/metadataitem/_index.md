---
title: "MetadataItem"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Konteyner öğelerinde ve meta veri çıkarma işlevinde kullanılan bir meta veri öğesini temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Konteyner öğelerinde ve meta veri çıkarma işlevinde kullanılan bir meta veri öğesini temsil eder.

[MetadataItem](../../com.groupdocs.parser.data/metadataitem) sınıfının bir örneği, [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) yönteminin dönüş değeri olarak kullanılır.
ve [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) koleksiyonunda bir öğe olarak. Oradaki kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | [MetadataItem](../../com.groupdocs.parser.data/metadataitem) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getName()](#getName--) | Meta veri öğesinin adını alır. |
|
|  | [getValue()](#getValue--) | Meta veri öğesinin değerini alır. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


[MetadataItem](../../com.groupdocs.parser.data/metadataitem) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ad | java.lang.String | Meta veri öğesinin adı. |
|
|  | değer | java.lang.String | Meta veri öğesinin değeri. |
|

### getName() {#getName--}
```
public String getName()
```


Meta veri öğesinin adını alır.


**Returns:**
java.lang.String - Meta veri öğesinin adını temsil eden bir dize değeri.

### getValue() {#getValue--}
```
public String getValue()
```


Meta veri öğesinin değerini alır.


**Returns:**
java.lang.String - Meta veri öğesinin değerini temsil eden bir dize değeri.

