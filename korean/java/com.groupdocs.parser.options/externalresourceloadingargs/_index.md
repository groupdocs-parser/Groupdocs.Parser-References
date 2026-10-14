---
title: "ExternalResourceLoadingArgs"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "메서드에 대한 데이터를 제공합니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

메서드 [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-)에 대한 데이터를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | 직사각형 영역을 사용하여 [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getUri()](#getUri--) | 외부 리소스의 URI를 가져옵니다. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | 외부 리소스의 URI를 가져옵니다. |
|
|  | [isSkipped()](#isSkipped--) | 외부 리소스 로드를 건너뛰어야 하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | 외부 리소스 로드를 건너뛰어야 하는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getData()](#getData--) | 사용자 데이터를 가져옵니다. |
|
|  | [setData(byte[] data)](#setData-byte---) | 사용자 데이터를 설정합니다. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


직사각형 영역을 사용하여 [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | uri | java.lang.String | 외부 리소스의 URI. |
|

### getUri() {#getUri--}
```
public String getUri()
```


외부 리소스의 URI를 가져옵니다.


**Returns:**
java.lang.String - 외부 리소스의 URI를 나타내는 문자열 값.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


외부 리소스의 URI를 가져옵니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | uri | java.lang.String | 외부 리소스의 새 URI를 나타내는 문자열 값. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


외부 리소스 로드를 건너뛰어야 하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 외부 리소스 로드를 건너뛰어야 하면 true; 그렇지 않으면 false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


외부 리소스 로드를 건너뛰어야 하는지 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 건너뛰기 | boolean | 외부 리소스 로드를 건너뛰어야 하면 true; 그렇지 않으면 false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


사용자 데이터를 가져옵니다.


**Returns:**
byte[] - 외부 리소스의 사용자 콘텐츠가 포함된 바이트 배열. 설정되지 않은 경우 null.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


사용자 데이터를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 데이터 | byte[] | 외부 리소스의 사용자 콘텐츠가 포함된 바이트 배열. 설정되지 않은 경우 null. |
|

