---
title: "Rectangle"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "직사각형 영역을 나타냅니다."
type: docs
weight: 26
url: /ko/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

직사각형 영역을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | 새로운 [Rectangle](../../com.groupdocs.parser.data/rectangle) 클래스 인스턴스를 초기화합니다. |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | 새로운 [Rectangle](../../com.groupdocs.parser.data/rectangle) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getLeft()](#getLeft--) | 직사각형 영역 왼쪽 가장자리의 x 좌표를 가져옵니다. |
|
|  | [getTop()](#getTop--) | 직사각형 영역 위쪽 가장자리의 y 좌표를 가져옵니다. |
|
|  | [getRight()](#getRight--) | 직사각형 영역 오른쪽 가장자리의 x 좌표를 가져옵니다. |
|
|  | [getBottom()](#getBottom--) | 직사각형 영역 아래쪽 가장자리의 y 좌표를 가져옵니다. |
|
|  | [getPosition()](#getPosition--) | 직사각형 영역 왼쪽 위 모서리의 좌표를 가져옵니다. |
|
|  | [getSize()](#getSize--) | 크기를 가져옵니다. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


새로운 [Rectangle](../../com.groupdocs.parser.data/rectangle) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 왼쪽 | double | 직사각형 영역 왼쪽 가장자리의 x 좌표입니다. |
|
|  | 위쪽 | double | 직사각형 영역 위쪽 가장자리의 y 좌표입니다. |
|
|  | 오른쪽 | double | 직사각형 영역 오른쪽 가장자리의 x 좌표입니다. |
|
|  | 아래쪽 | double | 사각형 영역 하단 가장자리의 y좌표. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


새로운 [Rectangle](../../com.groupdocs.parser.data/rectangle) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | 사각형 영역 좌상단 모서리의 좌표. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | 사각형 영역의 크기. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


직사각형 영역 왼쪽 가장자리의 x 좌표를 가져옵니다.


**Returns:**
double - 사각형 영역 왼쪽 가장자리의 x좌표를 나타내는 double 값.

### getTop() {#getTop--}
```
public double getTop()
```


직사각형 영역 위쪽 가장자리의 y 좌표를 가져옵니다.


**Returns:**
double - 사각형 영역 상단 가장자리의 y좌표를 나타내는 double 값.

### getRight() {#getRight--}
```
public double getRight()
```


직사각형 영역 오른쪽 가장자리의 x 좌표를 가져옵니다.


**Returns:**
double - 사각형 영역 오른쪽 가장자리의 x좌표를 나타내는 double 값.

### getBottom() {#getBottom--}
```
public double getBottom()
```


직사각형 영역 아래쪽 가장자리의 y 좌표를 가져옵니다.


**Returns:**
double - 사각형 영역 하단 가장자리의 y좌표를 나타내는 double 값.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


직사각형 영역 왼쪽 위 모서리의 좌표를 가져옵니다.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


크기를 가져옵니다.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
