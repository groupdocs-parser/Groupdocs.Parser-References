---
title: "ExternalResourceHandler"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει έναν χειριστή για τη φόρτωση εξωτερικών πόρων."
type: docs
weight: 16
url: /el/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

Παρέχει έναν χειριστή για τη φόρτωση εξωτερικών πόρων.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | Καλείται πριν από οποιαδήποτε φόρτωση εξωτερικού πόρου. |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


Καλείται πριν από οποιαδήποτε φόρτωση εξωτερικού πόρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | Τα δεδομένα για τον έλεγχο της φόρτωσης εξωτερικού πόρου. |
|

