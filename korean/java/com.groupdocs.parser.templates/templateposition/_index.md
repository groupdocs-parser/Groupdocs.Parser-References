---
title: "TemplatePosition"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 위치를 위한 기본 추상 클래스를 제공합니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

템플릿 위치를 위한 기본 추상 클래스를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | 주어진 factor에 따라 모든 좌표를 스케일링한 현재 위치의 복사본을 생성합니다. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


주어진 factor에 따라 모든 좌표를 스케일링한 현재 위치의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | factor | double | 스케일링 계수. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

