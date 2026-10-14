---
title: "ExternalResourceHandler"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет обработчик для загрузки внешних ресурсов."
type: docs
weight: 16
url: /ru/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

Предоставляет обработчик для загрузки внешних ресурсов.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | Вызывается перед любой загрузкой внешнего ресурса. |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


Вызывается перед любой загрузкой внешнего ресурса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | Данные для управления загрузкой внешнего ресурса. |
|

