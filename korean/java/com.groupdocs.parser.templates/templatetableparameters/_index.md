---
title: "TemplateTableParameters"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "테이블 감지 알고리즘에 대한 매개변수를 제공합니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

테이블 감지 알고리즘에 대한 매개변수를 제공합니다.

표를 감지하기 위한 두 가지 알고리즘이 있습니다:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

알고리즘이 표를 감지하지 못하거나 정확하지 않게 감지하는 경우에는 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) 클래스를 사용합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 테이블을 포함하는 직사각형 영역을 가져옵니다. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | 테이블 열 구분자를 가져옵니다. |
|
|  | [hasMergedCells()](#hasMergedCells--) | 표에 병합된 셀이 있는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getMinRowCount()](#getMinRowCount--) | 표 행의 최소 개수를 가져옵니다. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | 표 열의 최소 개수를 가져옵니다. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | 표 열 사이의 최소 간격을 가져옵니다. |
|
|  | [scale(double factor)](#scale-double-) | 주어진 계수에 따라 모든 좌표가 스케일된 이 매개변수들의 복사본을 생성합니다. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 표를 포함하는 직사각형 영역입니다. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | 테이블 열 구분자. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 표를 포함하는 직사각형 영역입니다. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | 테이블 열 구분자. |
|
|  | mergedCells | java.lang.Boolean | 표에 병합된 셀이 있는지 여부를 나타내는 값입니다. |
|
|  | minRowCount | java.lang.Integer | 표 행의 최소 개수입니다. |
|
|  | minColumnCount | java.lang.Integer | 표 열의 최소 개수입니다. |
|
|  | minVerticalSpace | java.lang.Integer | 표 열 사이의 최소 간격입니다. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


테이블을 포함하는 직사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


테이블 열 구분자를 가져옵니다.


**Returns:**
java.util.List<java.lang.Double> - 표 열 구분선의 x 좌표를 나타내는 double 값들의 컬렉션; 설정되지 않은 경우  null  입니다.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


표에 병합된 셀이 있는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
java.lang.Boolean - 표에 병합된 셀이 있는 경우  true ; 그렇지 않으면  false . 설정되지 않은 경우  null .

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


표 행의 최소 개수를 가져옵니다.


**Returns:**
java.lang.Integer - 표 행의 최소 개수를 나타내는 정수값; 설정되지 않은 경우  null .

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


표 열의 최소 개수를 가져옵니다.


**Returns:**
java.lang.Integer - 표 열의 최소 개수를 나타내는 정수값; 설정되지 않은 경우  null .

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


표 열 사이의 최소 간격을 가져옵니다.


**Returns:**
java.lang.Integer - 표 열 사이의 최소 간격을 나타내는 정수값; 설정되지 않은 경우  null .

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


주어진 계수에 따라 모든 좌표가 스케일된 이 매개변수들의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | factor | double | 스케일링 계수. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

