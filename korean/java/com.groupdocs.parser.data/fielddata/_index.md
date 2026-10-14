---
title: "FieldData"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "이름, 페이지 인덱스, 필드 값 등과 같은 필드 데이터를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

이름, 페이지 인덱스, 필드 값 등과 같은 필드 데이터를 나타냅니다. 필드에 따라 값은 텍스트, 이미지, 표 등일 수 있습니다.

[FieldData](../../com.groupdocs.parser.data/fielddata) 클래스의 인스턴스는 [DocumentData](../../com.groupdocs.parser.data/documentdata) 컬렉션에서 사용됩니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getName()](#getName--) | 필드 이름을 가져옵니다. |
|
|  | [getPageIndex()](#getPageIndex--) | 페이지 인덱스를 가져옵니다. |
|
|  | [getPageArea()](#getPageArea--) | 필드 값을 가져옵니다. |
|
|  | [getLinkedField()](#getLinkedField--) | 연결된 필드를 가져옵니다. |
|
|  | [getText()](#getText--) | 텍스트를 가져옵니다. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Name이 대문자로 변환되었는지 여부를 나타내는 값을 가져옵니다. |
|
### getName() {#getName--}
```
public String getName()
```


필드 이름을 가져옵니다.


**Returns:**
java.lang.String - 필드 이름을 나타내는 대문자 문자열 값입니다.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


페이지 인덱스를 가져옵니다.


**Returns:**
int - 필드를 포함하는 페이지의 0부터 시작하는 인덱스입니다.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


필드 값을 가져옵니다.

필드에 따라 PageArea 속성은 [PageArea](../../com.groupdocs.parser.data/pagearea) 클래스의 모든 파생 클래스를 포함할 수 있습니다.
예를 들어, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) 메서드는 텍스트 필드만 추출합니다.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


연결된 필드를 가져옵니다.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


텍스트를 가져옵니다.


**Returns:**
java.lang.String - 필드 텍스트의 값을 나타내는 문자열 값; null인 경우 [PageArea](../../com.groupdocs.parser.data/pagearea) 속성이 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 가 아닙니다.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Name이 대문자로 변환되었는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - Name이 대문자로 변환되었는지 여부를 나타내는 부울 값.

