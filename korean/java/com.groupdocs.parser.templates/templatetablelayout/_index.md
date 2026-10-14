---
title: "TemplateTableLayout"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 테이블 레이아웃을 제공하며, 이는 class가 테이블 위치를 정의하는 데 사용됩니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

템플릿 테이블 레이아웃을 제공하며, 이는 [TemplateTable](../../com.groupdocs.parser.templates/templatetable) 클래스가 테이블 위치를 정의하는 데 사용됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 테이블을 포함하는 직사각형 영역을 가져옵니다. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | 테이블 열 구분자를 가져옵니다. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | 테이블 행 구분자를 가져옵니다. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | 같은 크기, 구분자 및 위치를 가진 새로운 레이아웃을 포인트 단위로 생성합니다. |
|
|  | [scale(double factor)](#scale-double-) | 주어진 계수로 모든 좌표를 스케일링한 이 레이아웃의 복사본을 생성합니다. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | 테이블 열 구분자. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | 테이블 행 구분자. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


테이블을 포함하는 직사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


테이블 열 구분자를 가져옵니다.


**Returns:**
java.util.List<java.lang.Double> - 테이블 열 구분자의 x좌표를 나타내는 double 값들의 컬렉션입니다.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


테이블 행 구분자를 가져옵니다.


**Returns:**
java.util.List<java.lang.Double> - 테이블 행 구분자의 y좌표를 나타내는 double 값들의 컬렉션입니다.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


같은 크기, 구분자 및 위치를 가진 새로운 레이아웃을 포인트 단위로 생성합니다.

이 기능을 사용하면 Table Layout을 이동할 수 있습니다.

예를 들어, 문서의 각 페이지에 테이블이 있거나(또는 페이지에 테이블이 있는 문서 집합) 있습니다.
이러한 테이블은 위치와 내용은 다르지만 동일한 열과 행을 가집니다. 이 경우 사용자는
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 객체를 (0, 0) 위치에 한 번 정의한 다음, 해당 테이블의 위치로 이동시킬 수 있습니다.

테이블 위치가 페이지의 다른 객체에 의존하는 경우, 사용자는 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 객체를 정의할 수 있습니다
템플릿 문서를 기반으로 하고, 앵커 객체에 따라 이동시킵니다. 예를 들어, 이것이 요약 테이블인 경우
그리고 상세 테이블이 뒤따르며(행 수가 다를 수 있음). 이 경우 사용자는 정의할 수 있습니다
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
메서드는 현재 객체의 복사본을 반환합니다. 사용자는 임의의 좌표를 전달할 수 있습니다
(음수일 경우에도 - 레이아웃이 왼쪽/위쪽으로 이동합니다).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | 새 레이아웃의 위치. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


주어진 계수로 모든 좌표를 스케일링한 이 레이아웃의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | factor | double | 스케일링 계수. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

