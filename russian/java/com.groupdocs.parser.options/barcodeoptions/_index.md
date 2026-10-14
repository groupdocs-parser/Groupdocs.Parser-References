---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения штрих‑кода."
type: docs
weight: 10
url: /ru/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Предоставляет параметры, используемые для извлечения штрих‑кода.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Инициализирует новый экземпляр класса BarcodeOptions со значениями по умолчанию. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса BarcodeOptions с прямоугольной областью. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Инициализирует новый экземпляр класса BarcodeOptions с настройками качества и типами кодов. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Инициализирует новый экземпляр класса BarcodeOptions. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Возвращает значение, указывающее, разрешены ли некорректные штрихкоды. |
|
|  | [getDimension()](#getDimension--) | Возвращает минимальный размер минимального элемента штрихкода. |
|
|  | [getImageQuality()](#getImageQuality--) | Возвращает качество исходного изображения. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Возвращает качество исходного штрихкода. |
|
|  | [getRectangle()](#getRectangle--) | Получает прямоугольную область, содержащую области страниц. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Возвращает типы штрихкодов для чтения. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Устанавливает значение, указывающее, разрешены ли некорректные штрихкоды. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Устанавливает минимальный размер минимального элемента штрихкода. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Устанавливает качество исходного изображения. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Устанавливает качество исходного штрихкода. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Устанавливает прямоугольную область, содержащую штрихкоды. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Устанавливает типы штрихкодов для чтения. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Инициализирует новый экземпляр класса BarcodeOptions со значениями по умолчанию.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Инициализирует новый экземпляр класса BarcodeOptions с прямоугольной областью.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая штрихкоды. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Инициализирует новый экземпляр класса BarcodeOptions с настройками качества и типами кодов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Качество исходного изображения. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Качество исходного штрихкода. |
|
|  | codeTypes | java.lang.String[] | Типы штрихкодов для чтения. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Инициализирует новый экземпляр класса BarcodeOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая штрихкоды. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Качество исходного изображения. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Качество исходного штрихкода. |
|
|  | dimension | java.lang.Float | Минимальный размер минимального элемента штрихкода. |
|
|  | allowIncorrectBarcodes | boolean | Значение, указывающее, разрешены ли некорректные штрихкоды. |
|
|  | codeTypes | java.lang.String[] | Типы штрихкодов для чтения. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Возвращает значение, указывающее, разрешены ли некорректные штрихкоды.


**Returns:**
boolean -  true  если некорректные штрихкоды разрешены; иначе,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Возвращает минимальный размер минимального элемента штрихкода.


**Returns:**
java.lang.Float - Значение типа float, представляющее минимальный элемент штрихкода;  null  если используется автоматический режим.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Возвращает качество исходного изображения.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Возвращает качество исходного штрихкода.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Получает прямоугольную область, содержащую области страниц.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Возвращает типы штрихкодов для чтения.


**Returns:**
java.util.List<java.lang.String> - Коллекция только для чтения, содержащая типы штрихкодов для чтения; пустая коллекция, если не задана.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Устанавливает значение, указывающее, разрешены ли некорректные штрихкоды.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  если некорректные штрихкоды разрешены. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Устанавливает минимальный размер минимального элемента штрихкода.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dimension | java.lang.Float | Минимальный элемент штрихкода;  null  для автоматического режима. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Устанавливает качество исходного изображения.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Режим качества изображения. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Устанавливает качество исходного штрихкода.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Режим качества штрихкода. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Устанавливает прямоугольную область, содержащую штрихкоды.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область;  null  для сканирования всей страницы. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Устанавливает типы штрихкодов для чтения.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Типы штрихкодов;  null  или пусто для всех типов. |
|

