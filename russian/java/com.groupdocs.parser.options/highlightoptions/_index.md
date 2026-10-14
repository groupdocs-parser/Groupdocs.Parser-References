---
title: "HighlightOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, которые используются для извлечения выделения блока текста вокруг найденного текста в сценариях поиска."
type: docs
weight: 22
url: /ru/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Предоставляет параметры, используемые для извлечения выделения (блока текста вокруг найденного текста в сценариях поиска).

Экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) используется в качестве параметра в методе [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
Смотрите примеры использования там.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) без установленных ограничений. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), который используется для извлечения выделения фиксированной длины. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), который используется для извлечения выделения с ограничением по строке. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), который используется для извлечения выделения с фиксированным количеством слов. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Возвращает максимальную длину текста. |
|
|  | [getWordCount()](#getWordCount--) | Возвращает максимальное количество слов. |
|
|  | [isLineLimited()](#isLineLimited--) | Возвращает значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Устанавливает максимальную длину текста. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Устанавливает максимальное количество слов. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Устанавливает значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) без установленных ограничений. Установите хотя бы один из #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) перед передачей парсеру.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), который используется для извлечения выделения фиксированной длины.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | maxLength | int | Максимальная длина текста. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), который используется для извлечения выделения с ограничением по строке.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Максимальная длина текста. |
|
|  | isLineLimited | boolean | Значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), который используется для извлечения выделения с фиксированным количеством слов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Максимальная длина текста. |
|
|  | wordCount | int | Максимальное количество слов. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Инициализирует новый экземпляр класса [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Максимальная длина текста. |
|
|  | wordCount | java.lang.Integer | Максимальное количество слов. |
|
|  | isLineLimited | boolean | Значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Возвращает максимальную длину текста.


**Returns:**
java.lang.Integer - Положительное целочисленное значение, представляющее максимальную длину текста;  null  если длина текста не ограничена.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Возвращает максимальное количество слов.


**Returns:**
java.lang.Integer - Положительное целочисленное значение, представляющее максимальное количество слов;  null  если количество слов не ограничено.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Возвращает значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста.


**Returns:**
boolean -  true  если извлечение выделения ограничено началом (или концом) строки текста; иначе  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Устанавливает максимальную длину текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Неотрицательное целое число;  null  для снятия ограничения длины. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Устанавливает максимальное количество слов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Неотрицательное целое число;  null  для снятия ограничения количества слов. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Устанавливает значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lineLimited | boolean | true  для ограничения границами строки. |
|

