---
title: "QualityMode"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "품질 수준을 정의합니다."
type: docs
weight: 48
url: /ko/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

품질 수준을 정의합니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [High](#High) | 높은 품질. |
|
|  | [Normal](#Normal) | 보통 품질. |
|
|  | [Low](#Low) | 낮은 품질. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


높은 품질. 빠른 처리 알고리즘이 사용됩니다.


### Normal {#Normal}
```
public static final QualityMode Normal
```


보통 품질. 기본 처리 알고리즘이 사용됩니다.


### Low {#Low}
```
public static final QualityMode Low
```


낮은 품질. 느린 처리 알고리즘이 사용됩니다.


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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
