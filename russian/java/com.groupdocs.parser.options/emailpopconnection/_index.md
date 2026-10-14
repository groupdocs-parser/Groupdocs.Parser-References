---
title: "EmailPopConnection"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет информацию о подключении к электронной почте для протокола POP."
type: docs
weight: 15
url: /ru/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

Представляет информацию о подключении к электронной почте для протокола POP.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Создаёт новый экземпляр класса [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getHost()](#getHost--) | Получает имя хоста. |
|
|  | [getPort()](#getPort--) | Получает номер порта. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


Создаёт новый экземпляр класса [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection).


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

