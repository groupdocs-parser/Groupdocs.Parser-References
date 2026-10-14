---
title: "EmailPopConnection"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "POP 프로토콜에 대한 이메일 연결 정보를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

POP 프로토콜에 대한 이메일 연결 정보를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | 새로운 [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) 클래스의 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getHost()](#getHost--) | 호스트 이름을 가져옵니다. |
|
|  | [getPort()](#getPort--) | 포트 번호를 가져옵니다. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


새로운 [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | host | java.lang.String | 호스트 이름. |
|
|  | port | int | 포트 번호. |
|
|  | userName | java.lang.String | 사용자 이름. |
|
|  | 비밀번호 | java.lang.String | 비밀번호. |
|

### getHost() {#getHost--}
```
public String getHost()
```


호스트 이름을 가져옵니다.


**Returns:**
java.lang.String - 호스트 이름을 나타내는 문자열 값.

### getPort() {#getPort--}
```
public int getPort()
```


포트 번호를 가져옵니다.


**Returns:**
int - 포트 번호를 나타내는 정수 값.

