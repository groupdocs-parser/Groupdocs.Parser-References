---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра."
type: docs
weight: 34
url: /ru/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Предоставляет параметры для установки требований и делегатов потоков при генерации предварительного просмотра.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Инициализирует новый экземпляр класса [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), вызывая закрытие выходного потока. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Инициализирует новый экземпляр класса [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), вызывая возврат выходного потока клиенту для дальнейшего использования. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getWidth()](#getWidth--) | Получает ширину предварительного просмотра страницы. |
|
|  | [setWidth(int width)](#setWidth-int-) | Устанавливает ширину предварительного просмотра страницы. |
|
|  | [getHeight()](#getHeight--) | Получает высоту предварительного просмотра страницы. |
|
|  | [setHeight(int height)](#setHeight-int-) | Устанавливает высоту предварительного просмотра страницы. |
|
|  | [getDpi()](#getDpi--) | Получает dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Устанавливает dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Получает массив номеров страниц для создания предварительных просмотров. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Устанавливает массив номеров страниц для создания предварительных просмотров. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Получает формат изображения предварительного просмотра. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Устанавливает формат изображения предварительного просмотра. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Получает экземпляр делегата создания потока страницы. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Устанавливает экземпляр делегата создания потока страницы. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Получает экземпляр делегата завершения предварительного просмотра страницы. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Устанавливает экземпляр делегата завершения предварительного просмотра страницы. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Получает экземпляр делегата информации о рендеринге предварительного просмотра страницы. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Устанавливает экземпляр делегата информации о рендеринге предварительного просмотра страницы. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Инициализирует новый экземпляр класса [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), вызывая закрытие выходного потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Создаёт поток для конкретного предварительного просмотра страницы. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Инициализирует новый экземпляр класса [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), вызывая возврат выходного потока клиенту для дальнейшего использования.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Создаёт поток для конкретного предварительного просмотра страницы |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Уведомляет, что создание предварительного просмотра страницы завершено, и получает выходной поток. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Получает ширину предварительного просмотра страницы.


**Returns:**
int - Ширина страницы.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Устанавливает ширину предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | width | int | Ширина страницы. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Получает высоту предварительного просмотра страницы.


**Returns:**
int - Высота страницы.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Устанавливает высоту предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | height | int | Высота страницы. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Получает dpi.


**Returns:**
int - Целочисленное значение, представляющее dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Устанавливает dpi.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dpi | int | Разрешение (dpi). |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Получает массив номеров страниц для создания предварительных просмотров.


**Returns:**
int[] — коллекция номеров страниц.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Устанавливает массив номеров страниц для создания предварительных просмотров.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageNumbers | int[] | Коллекция номеров страниц. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Получает формат изображения предварительного просмотра.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Устанавливает формат изображения предварительного просмотра.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Формат предварительного просмотра. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Получает экземпляр делегата создания потока страницы.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Устанавливает экземпляр делегата создания потока страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Делегат создания потока страницы. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Получает экземпляр делегата завершения предварительного просмотра страницы.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Устанавливает экземпляр делегата завершения предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Делегат завершения предварительного просмотра страницы. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Получает экземпляр делегата информации о рендеринге предварительного просмотра страницы.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Устанавливает экземпляр делегата информации о рендеринге предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Делегат информации о рендеринге предварительного просмотра страницы. |
|

