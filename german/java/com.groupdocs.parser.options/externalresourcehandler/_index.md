---
title: "ExternalResourceHandler"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Handler für das Laden externer Ressourcen bereit."
type: docs
weight: 16
url: /de/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

Stellt einen Handler für das Laden externer Ressourcen bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | Wird aufgerufen, bevor irgendeine externe Ressource geladen wird. |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


Wird aufgerufen, bevor irgendeine externe Ressource geladen wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | Die Daten zur Steuerung des Ladens externer Ressourcen. |
|

