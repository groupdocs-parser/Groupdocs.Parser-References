---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет данные для метода ."
type: docs
weight: 17
url: /ru/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Предоставляет данные для метода [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Инициализирует новый экземпляр класса [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) с прямоугольной областью. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getUri()](#getUri--) | Получает URI внешнего ресурса. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Получает URI внешнего ресурса. |
|
|  | [isSkipped()](#isSkipped--) | Получает значение, указывающее, следует ли пропустить загрузку внешнего ресурса. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Устанавливает значение, указывающее, следует ли пропустить загрузку внешнего ресурса. |
|
|  | [getData()](#getData--) | Получает пользовательские данные. |
|
|  | [setData(byte[] data)](#setData-byte---) | Устанавливает пользовательские данные. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Инициализирует новый экземпляр класса [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) с прямоугольной областью.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | uri | java.lang.String | URI внешнего ресурса. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Получает URI внешнего ресурса.


**Returns:**
java.lang.String - Строковое значение, представляющее URI внешнего ресурса.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Получает URI внешнего ресурса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | uri | java.lang.String | Строковое значение, представляющее новый URI внешнего ресурса. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Получает значение, указывающее, следует ли пропустить загрузку внешнего ресурса.


**Returns:**
boolean - true, если загрузку внешнего ресурса следует пропустить; иначе false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Устанавливает значение, указывающее, следует ли пропустить загрузку внешнего ресурса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пропущено | boolean | true, если загрузку внешнего ресурса следует пропустить; иначе false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Получает пользовательские данные.


**Returns:**
byte[] - Массив байтов с пользовательским содержимым внешнего ресурса. null, если не установлен.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Устанавливает пользовательские данные.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | byte[] | Массив байтов с пользовательским содержимым внешнего ресурса. null, если не установлен. |
|

