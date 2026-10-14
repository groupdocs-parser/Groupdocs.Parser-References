---
title: "QualityMode"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Ορίζει ένα επίπεδο ποιότητας."
type: docs
weight: 48
url: /el/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Ορίζει ένα επίπεδο ποιότητας.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [High](#High) | Υψηλή ποιότητα. |
|
|  | [Normal](#Normal) | Κανονική ποιότητα. |
|
|  | [Low](#Low) | Χαμηλή ποιότητα. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Υψηλή ποιότητα. Χρησιμοποιούνται γρήγοροι αλγόριθμοι επεξεργασίας.


### Normal {#Normal}
```
public static final QualityMode Normal
```


Κανονική ποιότητα. Χρησιμοποιούνται προεπιλεγμένοι αλγόριθμοι επεξεργασίας.


### Low {#Low}
```
public static final QualityMode Low
```


Χαμηλή ποιότητα. Χρησιμοποιούνται αργοί αλγόριθμοι επεξεργασίας.


### values() {#values--}
```
public static QualityMode[] values()
```




**Returns:**
com.groupdocs.parser.options.QualityMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static QualityMode valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
