---
title: QualityMode
second_title: GroupDocs.Parser for Java API Reference
description: Defines a level of the quality.
type: docs
weight: 48
url: /java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

Defines a level of the quality.
## Fields

| Field | Description |
| --- | --- |
| [High](#High) | Hight quality. |
| [Normal](#Normal) | Normal quality. |
| [Low](#Low) | Low quality. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


Hight quality. Fast processing algorithms are used.

### Normal {#Normal}
```
public static final QualityMode Normal
```


Normal quality. Default processing algorithms are used.

### Low {#Low}
```
public static final QualityMode Low
```


Low quality. Slow processing algorithms are used.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
