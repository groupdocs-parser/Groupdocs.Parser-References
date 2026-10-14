---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Ορίζει μια λειτουργία εντοπισμού τύπου αρχείου."
type: docs
weight: 44
url: /el/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Ορίζει μια λειτουργία εντοπισμού τύπου αρχείου.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Default](#Default) | Ο τύπος αρχείου ανιχνεύεται με βάση την επέκταση του αρχείου· εάν η επέκταση δεν αναγνωρίζεται, ο τύπος αρχείου ανιχνεύεται με βάση το περιεχόμενο του αρχείου. |
|
|  | [Extension](#Extension) | Ο τύπος αρχείου ανιχνεύεται μόνο με την επέκταση του αρχείου. |
|
|  | [Content](#Content) | Ο τύπος αρχείου ανιχνεύεται μόνο με το περιεχόμενο του αρχείου. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Ο τύπος αρχείου ανιχνεύεται με βάση την επέκταση του αρχείου· εάν η επέκταση δεν αναγνωρίζεται, ο τύπος αρχείου ανιχνεύεται με βάση το περιεχόμενο του αρχείου.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Ο τύπος αρχείου ανιχνεύεται μόνο με την επέκταση του αρχείου.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Ο τύπος αρχείου ανιχνεύεται μόνο με το περιεχόμενο του αρχείου.


### values() {#values--}
```
public static FileTypeDetectionMode[] values()
```




**Returns:**
com.groupdocs.parser.options.FileTypeDetectionMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileTypeDetectionMode valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)
