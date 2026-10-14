---
title: "TemplateLinkedPosition"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "연결된 필드를 사용하는 템플릿 필드 위치를 제공합니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

연결된 필드를 사용하는 템플릿 필드 위치를 제공합니다.

다음 예제는 청구서 번호가 있는 필드가 알려진 상황에 대한 코드를 보여줍니다.
\"Invoice number\" 문자열의 오른쪽에 배치된 경우 다음 코드를 사용합니다:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | 새로운 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | 대문자 이름을 사용하여 새로운 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | 새로운 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | 연결된 필드 이름을 가져옵니다. |
|
|  | [getSearchArea()](#getSearchArea--) | 필드가 검색되는 영역의 크기를 가져옵니다. |
|
|  | [isAutoScale()](#isAutoScale--) | 연결된 필드 크기에 따라 SearchArea가 스케일링되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getEdges()](#getEdges--) | 필드가 검색되는 연결된 필드의 가장자리를 가져옵니다. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


새로운 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | 연결된 필드의 이름입니다. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | 필드가 검색되는 영역의 크기입니다. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | 필드가 검색되는 연결된 필드의 가장자리입니다. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


대문자 이름을 사용하여 새로운 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | 연결된 필드의 이름입니다. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | 필드가 검색되는 영역의 크기입니다. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | 필드가 검색되는 연결된 필드의 가장자리입니다. |
|
|  | autoScale | boolean | 연결된 필드 크기에 따라 searchArea가 스케일링되는지 여부를 나타내는 값입니다. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


새로운 [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | 연결된 필드의 이름입니다. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | 필드가 검색되는 영역의 크기입니다. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | 필드가 검색되는 연결된 필드의 가장자리입니다. |
|
|  | autoScale | boolean | 연결된 필드 크기에 따라 searchArea가 스케일링되는지 여부를 나타내는 값입니다.\\ |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


연결된 필드 이름을 가져옵니다.


**Returns:**
java.lang.String - 연결된 필드 이름을 나타내는 대문자 문자열 값입니다.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


필드가 검색되는 영역의 크기를 가져옵니다.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


연결된 필드 크기에 따라 SearchArea가 스케일링되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
java.lang.Boolean - 연결된 필드 크기에 따라 SearchArea가 스케일링되는 경우 {code true}; 그렇지 않으면 false 입니다.

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


필드가 검색되는 연결된 필드의 가장자리를 가져옵니다.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

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
