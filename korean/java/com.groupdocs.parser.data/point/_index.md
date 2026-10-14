---
title: "Point"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "점을 나타냅니다."
type: docs
weight: 25
url: /ko/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

점을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | [Point](../../com.groupdocs.parser.data/point) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getX()](#getX--) | x 좌표를 가져옵니다. |
|
|  | [getY()](#getY--) | y 좌표를 가져옵니다. |
|
|  | [parse(String s)](#parse-java.lang.String-) | 점의 문자열 표현을 해당 클래스 형태로 변환합니다. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


[Point](../../com.groupdocs.parser.data/point) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | x | double | x 좌표. |
|
|  | y | double | y 좌표. |
|

### getX() {#getX--}
```
public double getX()
```


x 좌표를 가져옵니다.


**Returns:**
double - x 좌표를 나타내는 double 값입니다.

### getY() {#getY--}
```
public double getY()
```


y 좌표를 가져옵니다.


**Returns:**
double - y 좌표를 나타내는 double 값입니다.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


점의 문자열 표현을 해당 클래스 형태로 변환합니다. 반환 값은 변환이 성공했는지 실패했는지를 나타냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | s | java.lang.String | 변환할 점을 포함하는 문자열입니다. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
