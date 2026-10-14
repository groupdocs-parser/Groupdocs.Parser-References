---
title: "TextReader"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "연속적인 문자 시퀀스를 읽을 수 있는 리더를 나타냅니다."
type: docs
weight: 29
url: /ko/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

연속적인 문자 시퀀스를 읽을 수 있는 리더를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | 텍스트 리더에서 문자 한 줄을 읽고 데이터를 문자열로 반환합니다. |
|
|  | [readToEnd()](#readToEnd--) | 현재 위치부터 텍스트 리더의 끝까지 모든 문자를 읽고 하나의 문자열로 반환합니다. |
|
|  | [dispose()](#dispose--) | 텍스트 리더([TextReader](../../com.groupdocs.parser.data/textreader)) 객체가 사용한 모든 리소스를 해제합니다. |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


텍스트 리더에서 문자 한 줄을 읽고 데이터를 문자열로 반환합니다.


**Returns:**
java.lang.String - 리더에서 다음 줄, 또는 모든 문자를 읽은 경우  null  .

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


현재 위치부터 텍스트 리더의 끝까지 모든 문자를 읽고 하나의 문자열로 반환합니다.


**Returns:**
java.lang.String - 현재 위치부터 텍스트 리더의 끝까지 모든 문자를 포함하는 문자열.

### dispose() {#dispose--}
```
public void dispose()
```


텍스트 리더([TextReader](../../com.groupdocs.parser.data/textreader)) 객체가 사용한 모든 리소스를 해제합니다.


