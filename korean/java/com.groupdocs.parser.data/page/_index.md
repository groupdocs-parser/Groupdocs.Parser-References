---
title: "페이지"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "페이지 인덱스 및 페이지 크기와 같은 문서 페이지 정보를 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

문서 페이지 정보(페이지 인덱스 및 페이지 크기 등)를 나타냅니다. 템플릿 기능을 통한 파싱에서 [PageArea](../../com.groupdocs.parser.data/pagearea) 클래스를 상속하는 페이지를 나타내는 데 사용됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | [Page](../../com.groupdocs.parser.data/page) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getIndex()](#getIndex--) | 페이지 인덱스를 가져옵니다. |
|
|  | [getSize()](#getSize--) | 페이지 크기를 가져옵니다. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


[Page](../../com.groupdocs.parser.data/page) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 페이지 인덱스. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | 페이지 크기. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


페이지 인덱스를 가져옵니다.


**Returns:**
int - 페이지의 0부터 시작하는 인덱스.

### getSize() {#getSize--}
```
public Size getSize()
```


페이지 크기를 가져옵니다.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

