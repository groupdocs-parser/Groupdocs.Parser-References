---
title: "ExternalResourceHandler"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit un gestionnaire pour le chargement des ressources externes."
type: docs
weight: 16
url: /fr/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

Fournit un gestionnaire pour le chargement des ressources externes.

## Constructors

| Constructor | Description |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | Appelé avant tout chargement de ressource externe. |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


Appelé avant tout chargement de ressource externe.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | Les données pour contrôler le chargement de la ressource externe. |
|

