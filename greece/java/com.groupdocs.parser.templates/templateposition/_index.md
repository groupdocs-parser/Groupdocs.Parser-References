---
title: "TemplatePosition"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει μια βασική αφηρημένη κλάση για θέσεις προτύπου."
type: docs
weight: 18
url: /el/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Παρέχει μια βασική αφηρημένη κλάση για θέσεις προτύπου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Δημιουργεί ένα αντίγραφο της τρέχουσας θέσης με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοθέντα παράγοντα. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Δημιουργεί ένα αντίγραφο της τρέχουσας θέσης με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοθέντα παράγοντα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | παράγοντας | double | Ο συντελεστής κλιμάκωσης. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

