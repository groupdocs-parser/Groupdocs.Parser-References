---
title: "Лицензия"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет лицензию GroupDocs.Parser."
type: docs
weight: 10
url: /ru/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Представляет лицензию GroupDocs.Parser.

Этот пример демонстрирует, как настроить лицензию.

````
 ```

// Инициализировать класс License
License license = new License();
// Установите путь к файлу .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [License()](#License--) | Инициализирует новый экземпляр класса [License](../../com.groupdocs.parser.licensing/license). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Лицензирует компонент. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Лицензирует компонент. |
|
### License() {#License--}
```
public License()
```


Инициализирует новый экземпляр класса [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Лицензирует компонент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Абсолютный путь к файлу лицензии. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Лицензирует компонент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | stream | java.io.InputStream | Поток лицензии. |
|

