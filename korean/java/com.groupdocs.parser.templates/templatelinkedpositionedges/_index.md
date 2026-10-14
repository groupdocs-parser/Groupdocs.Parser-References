---
title: "TemplateLinkedPositionEdges"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트 필드가 검색되는 연결된 필드의 가장자리를 제공합니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

연결된 필드에서 텍스트 필드가 검색되는 가장자리 정보를 제공합니다. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) 은 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스에서 사용됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | 인스턴스가 비어 있는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isLeft()](#isLeft--) | 연결된 필드의 왼쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isTop()](#isTop--) | 연결된 필드의 위쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isRight()](#isRight--) | 연결된 필드의 오른쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isBottom()](#isBottom--) | 연결된 필드의 아래쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [parse(String s)](#parse-java.lang.String-) | 가장자리의 문자열 표현을 해당 클래스 형태로 변환합니다. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 왼쪽 | boolean | 연결된 필드의 왼쪽에서 필드를 검색하는지 여부를 나타내는 값. |
|
|  | 위쪽 | boolean | 연결된 필드의 위쪽에서 필드를 검색하는지 여부를 나타내는 값. |
|
|  | 오른쪽 | boolean | 연결된 필드의 오른쪽에서 필드를 검색하는지 여부를 나타내는 값. |
|
|  | 아래쪽 | boolean | 연결된 필드의 아래쪽에서 필드를 검색하는지 여부를 나타내는 값. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


인스턴스가 비어 있는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 인스턴스가 비어 있는 경우 true (모든 필드가 false); 그렇지 않으면 false.

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


연결된 필드의 왼쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 연결된 필드의 왼쪽에서 필드를 검색하는 경우 true; 그렇지 않으면 false.

### isTop() {#isTop--}
```
public boolean isTop()
```


연결된 필드의 위쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 연결된 필드의 위쪽에서 필드를 검색하는 경우 true; 그렇지 않으면 false.

### isRight() {#isRight--}
```
public boolean isRight()
```


연결된 필드의 오른쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 연결된 필드의 오른쪽에서 필드를 검색하는 경우 true; 그렇지 않으면 false.

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


연결된 필드의 아래쪽에서 필드를 검색하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 연결된 필드의 아래쪽에서 필드를 검색하는 경우 true; 그렇지 않으면 false.

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


가장자리의 문자열 표현을 해당 클래스 형태로 변환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | s | java.lang.String | 변환할 가장자리를 포함하는 문자열. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
