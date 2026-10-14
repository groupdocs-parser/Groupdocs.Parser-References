---
title: "TemplateOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'analyse par la fonctionnalité de modèle."
type: docs
weight: 17
url: /fr/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Fournit les options utilisées pour l'analyse par la fonctionnalité de modèle.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Initialise une nouvelle instance de la classe [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Initialise une nouvelle instance de la classe [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangleTolerance | double | La taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte.


**Returns:**
double - La valeur double de 0 (pas de bordure) à 1 (ignorer tout l'élément).

