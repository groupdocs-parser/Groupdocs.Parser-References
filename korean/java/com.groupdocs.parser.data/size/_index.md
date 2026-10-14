---
title: "Size"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "크기를 나타냅니다."
type: docs
weight: 28
url: /ko/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

크기를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | [Size](../../com.groupdocs.parser.data/size) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 너비를 가져옵니다. |
|
|  | [getHeight()](#getHeight--) | 높이를 가져옵니다. |
|
|  | [isEmpty()](#isEmpty--) | 크기가 비어 있는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [parse(String s)](#parse-java.lang.String-) | 크기의 문자열 표현을 해당 클래스 형태로 변환합니다. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


[Size](../../com.groupdocs.parser.data/size) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 너비 | double | 픽셀 단위의 너비입니다. |
|
|  | 높이 | double | 픽셀 단위의 높이입니다. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


너비를 가져옵니다.


**Returns:**
double - 픽셀 단위의 너비를 나타내는 double 값입니다.

### getHeight() {#getHeight--}
```
public double getHeight()
```


높이를 가져옵니다.


**Returns:**
double - 픽셀 단위의 높이를 나타내는 double 값입니다.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


크기가 비어 있는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 너비와 높이가 0이면 true, 그렇지 않으면 false.

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


크기의 문자열 표현을 해당 클래스 형태로 변환합니다. 반환값은 변환이 성공했는지 실패했는지를 나타냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | s | java.lang.String | 변환할 크기를 포함하는 문자열입니다. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
