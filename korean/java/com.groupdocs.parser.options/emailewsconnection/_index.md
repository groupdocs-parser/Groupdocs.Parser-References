---
title: "EmailEwsConnection"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "EWS 프로토콜에 대한 이메일 연결 정보를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

EWS 프로토콜에 대한 이메일 연결 정보를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | 새로운 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 클래스 인스턴스를 초기화합니다. |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 새로운 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | 메일함의 URI를 가져옵니다. |
|
|  | [getDomain()](#getDomain--) | 도메인 이름을 가져옵니다. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


새로운 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | 메일함의 URI. |
|
|  | userName | java.lang.String | 사용자 이름. |
|
|  | 비밀번호 | java.lang.String | 비밀번호. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


새로운 [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | 메일함의 URI. |
|
|  | domain | java.lang.String | 도메인 이름. |
|
|  | userName | java.lang.String | 사용자 이름. |
|
|  | 비밀번호 | java.lang.String | 비밀번호. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


메일함의 URI를 가져옵니다.


**Returns:**
java.lang.String - 메일함의 URI를 나타내는 문자열 값.

### getDomain() {#getDomain--}
```
public String getDomain()
```


도메인 이름을 가져옵니다.


**Returns:**
java.lang.String - 도메인 이름을 나타내는 문자열 값.

