---
title: "TextStyle"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트의 스타일을 나타내며, 예를 들어 글꼴 이름, 글꼴 크기 등을 포함합니다."
type: docs
weight: 30
url: /ko/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

글꼴 이름, 글꼴 크기 등과 같은 텍스트 스타일을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | 새로운 [TextStyle](../../com.groupdocs.parser.data/textstyle) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getName()](#getName--) | 스타일 이름을 가져옵니다. |
|
|  | [getFontName()](#getFontName--) | 글꼴 이름을 가져옵니다. |
|
|  | [getFontSize()](#getFontSize--) | 글꼴 크기를 가져옵니다. |
|
|  | [isBold()](#isBold--) | 글꼴이 굵게 표시되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isItalic()](#isItalic--) | 글꼴이 기울임꼴인지 여부를 나타내는 값을 가져옵니다. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


새로운 [TextStyle](../../com.groupdocs.parser.data/textstyle) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 이름 | java.lang.String | 스타일의 이름입니다. |
|
|  | fontName | java.lang.String | 글꼴의 이름입니다. |
|
|  | fontSize | double | 글꼴의 크기입니다. |
|
|  | bold | boolean | 글꼴이 굵게 표시되는지 여부를 나타내는 값. |
|
|  | italic | boolean | 글꼴이 기울임꼴인지 여부를 나타내는 값. |
|

### getName() {#getName--}
```
public String getName()
```


스타일 이름을 가져옵니다.


**Returns:**
java.lang.String - 스타일 이름을 나타내는 문자열 값입니다.

### getFontName() {#getFontName--}
```
public String getFontName()
```


글꼴 이름을 가져옵니다.


**Returns:**
java.lang.String - 글꼴 이름을 나타내는 문자열 값입니다.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


글꼴 크기를 가져옵니다.


**Returns:**
double - 글꼴 크기를 나타내는 double 값입니다.

### isBold() {#isBold--}
```
public boolean isBold()
```


글꼴이 굵게 표시되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  글꼴이 굵게 설정된 경우; 그렇지 않으면  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


글꼴이 기울임꼴인지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  글꼴이 기울임꼴인 경우; 그렇지 않으면  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
