---
title: "QualityMode"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "定义质量级别。"
type: docs
weight: 48
url: /zh/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

定义质量级别。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [High](#High) | 高质量。 |
|
|  | [Normal](#Normal) | 普通质量。 |
|
|  | [Low](#Low) | 低质量。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


高质量。使用快速处理算法。


### Normal {#Normal}
```
public static final QualityMode Normal
```


普通质量。使用默认处理算法。


### Low {#Low}
```
public static final QualityMode Low
```


低质量。使用慢速处理算法。


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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
