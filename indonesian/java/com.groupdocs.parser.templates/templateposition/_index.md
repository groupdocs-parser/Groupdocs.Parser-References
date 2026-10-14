---
title: "TemplatePosition"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan kelas abstrak dasar untuk posisi templat."
type: docs
weight: 18
url: /id/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Menyediakan kelas abstrak dasar untuk posisi templat.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Membuat salinan posisi saat ini dengan semua koordinat diskalakan oleh faktor yang diberikan. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Membuat salinan posisi saat ini dengan semua koordinat diskalakan oleh faktor yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | faktor | double | Faktor skala. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

