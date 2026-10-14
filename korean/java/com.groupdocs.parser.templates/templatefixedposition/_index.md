---
title: "TemplateFixedPosition"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "직사각형 영역으로 정의된 템플릿 필드 위치를 제공합니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

직사각형 영역으로 정의된 템플릿 필드 위치를 제공합니다.

필드 위치를 정의하는 가장 간단한 방법입니다. 페이지에 필드 값을 제한하는 직사각형 영역을 설정해야 합니다.
필드 값입니다. 직사각형 영역에 포함된(부분적으로라도) 모든 텍스트가 값으로 추출됩니다:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | 새로운 [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 템플릿 필드를 포함하는 직사각형 영역을 가져옵니다. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


새로운 [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 템플릿 필드를 포함하는 직사각형 영역. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


템플릿 필드를 포함하는 직사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


주어진 factor에 따라 모든 좌표를 스케일링한 현재 위치의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
