---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о подключении к электронной почте для протокола EWS."
type: docs
weight: 13
url: /ru/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Представляет информацию о подключении к электронной почте для протокола EWS.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Получает URI почтового ящика. |
|
|  | [getDomain()](#getDomain--) | Получает имя домена. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Инициализирует новый экземпляр класса [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI почтового ящика. |
|
|  | userName | java.lang.String | Имя пользователя. |
|
|  | пароль | java.lang.String | Пароль. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Инициализирует новый экземпляр класса [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI почтового ящика. |
|
|  | домен | java.lang.String | Имя домена. |
|
|  | userName | java.lang.String | Имя пользователя. |
|
|  | пароль | java.lang.String | Пароль. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Получает URI почтового ящика.


**Returns:**
java.lang.String - Строковое значение, которое представляет URI почтового ящика.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Получает имя домена.


**Returns:**
java.lang.String - Строковое значение, которое представляет имя домена.

