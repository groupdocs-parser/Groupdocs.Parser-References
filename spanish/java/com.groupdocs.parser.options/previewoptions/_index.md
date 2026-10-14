---
title: "PreviewOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas."
type: docs
weight: 34
url: /es/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Inicializa una nueva instancia de la clase [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) que hace que el flujo de salida se cierre. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Inicializa una nueva instancia de la clase [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) que hace que el flujo de salida se devuelva al cliente para su uso posterior. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getWidth()](#getWidth--) | Obtiene el ancho de la vista previa de la página. |
|
|  | [setWidth(int width)](#setWidth-int-) | Establece el ancho de la vista previa de la página. |
|
|  | [getHeight()](#getHeight--) | Obtiene la altura de la vista previa de la página. |
|
|  | [setHeight(int height)](#setHeight-int-) | Establece la altura de la vista previa de la página. |
|
|  | [getDpi()](#getDpi--) | Obtiene un dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Establece un dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Obtiene una matriz de números de página para generar vistas previas. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Establece una matriz de números de página para generar vistas previas. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Obtiene el formato de imagen de la vista previa. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Establece el formato de imagen de la vista previa. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Obtiene una instancia del delegado de creación de flujo de página. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Establece una instancia del delegado de creación de flujo de página. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Obtiene una instancia del delegado de finalización de la vista previa de la página. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Establece una instancia del delegado de finalización de la vista previa de la página. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Obtiene una instancia del delegado de información de renderizado de la vista previa de la página. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Establece una instancia del delegado de información de renderizado de la vista previa de la página. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Inicializa una nueva instancia de la clase [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) que hace que el flujo de salida se cierre.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Crea un flujo para una vista previa de página específica. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Inicializa una nueva instancia de la clase [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) que hace que el flujo de salida se devuelva al cliente para su uso posterior.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Crea un flujo para una vista previa de página específica |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Notifica que la generación de la vista previa de la página ha finalizado y obtiene el flujo de salida. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Obtiene el ancho de la vista previa de la página.


**Returns:**
int - El ancho de la página.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Establece el ancho de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | ancho | int | El ancho de la página. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Obtiene la altura de la vista previa de la página.


**Returns:**
int - La altura de la página.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Establece la altura de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | altura | int | La altura de la página. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Obtiene un dpi.


**Returns:**
int - Un valor entero que representa un dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Establece un dpi.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dpi | int | El dpi. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Obtiene una matriz de números de página para generar vistas previas.


**Returns:**
int[] - Una colección de números de página.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Establece una matriz de números de página para generar vistas previas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pageNumbers | int[] | Una colección de números de página. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Obtiene el formato de imagen de la vista previa.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Establece el formato de imagen de la vista previa.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | El formato de vista previa. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Obtiene una instancia del delegado de creación de flujo de página.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Establece una instancia del delegado de creación de flujo de página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | El delegado de creación del flujo de página. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Obtiene una instancia del delegado de finalización de la vista previa de la página.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Establece una instancia del delegado de finalización de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | El delegado de finalización de la vista previa de la página. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Obtiene una instancia del delegado de información de renderizado de la vista previa de la página.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Establece una instancia del delegado de información de renderizado de la vista previa de la página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | El delegado de información de renderizado de la vista previa de la página. |
|

