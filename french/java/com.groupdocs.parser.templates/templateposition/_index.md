---
title: "TemplatePosition"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit une classe abstraite de base pour les positions de modèle."
type: docs
weight: 18
url: /fr/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Fournit une classe abstraite de base pour les positions de modèle.

## Constructors

| Constructor | Description |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Crée une copie de la position actuelle avec toutes les coordonnées mises à l'échelle par le facteur donné. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Crée une copie de la position actuelle avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | factor | double | Le facteur d'échelle. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

