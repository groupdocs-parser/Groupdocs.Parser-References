---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о подключении к электронной почте для протокола IMAP."
type: docs
weight: 14
url: /ru/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Представляет информацию о подключении к электронной почте для протокола IMAP.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getHost()](#getHost--) | Получает имя хоста. |
|
|  | [getPort()](#getPort--) | Получает номер порта. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Инициализирует новый экземпляр класса [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | host | java.lang.String | Имя хоста. |
|
|  | port | int | Номер порта. |
|
|  | userName | java.lang.String | Имя пользователя. |
|
|  | пароль | java.lang.String | Пароль. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Получает имя хоста.


**Returns:**
java.lang.String - Строковое значение, представляющее имя хоста.

### getPort() {#getPort--}
```
public int getPort()
```


Получает номер порта.


**Returns:**
int - Целочисленное значение, представляющее номер порта.

