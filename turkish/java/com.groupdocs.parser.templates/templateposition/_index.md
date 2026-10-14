---
title: "TemplatePosition"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon konumları için temel soyut sınıfı sağlar."
type: docs
weight: 18
url: /tr/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Şablon konumları için temel soyut sınıfı sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Mevcut konumun bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirilmiş şekilde oluşturur. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Mevcut konumun bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirilmiş şekilde oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | faktör | double | Ölçekleme faktörü. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

