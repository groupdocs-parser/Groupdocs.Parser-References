---
title: "OcrEventHandler"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "OCR 이벤트에 대한 핸들러를 제공합니다."
type: docs
weight: 26
url: /ko/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

OCR 이벤트에 대한 핸들러를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | 경고 메시지 목록을 가져옵니다. |
|
|  | [hasWarnings()](#hasWarnings--) | 경고 목록이 비어 있지 않은지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | pageIndex가 있는 페이지에 대한 경고 메시지 목록을 반환합니다. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | 페이지에 대한 경고 메시지를 설정합니다. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 클래스의 새 인스턴스를 초기화합니다.


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


경고 메시지 목록을 가져옵니다.


**Returns:**
java.util.List<java.lang.String> - 모든 페이지에 대한 경고 메시지 목록.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


경고 목록이 비어 있지 않은지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 경고 목록이 비어 있지 않은 경우 true; 그렇지 않으면 false.

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


pageIndex가 있는 페이지에 대한 경고 메시지 목록을 반환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.util.List<java.lang.String> - 페이지에 대한 경고 메시지 목록; 페이지에 경고 메시지가 없으면 빈 목록.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


페이지에 대한 경고 메시지를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | 페이지에 대한 경고 메시지 목록. |
|

