---
title: "PreviewOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt opties om vereisten en streamdelegates in te stellen voor het genereren van een voorbeeld."
type: docs
weight: 34
url: /nl/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Biedt opties om vereisten en streamdelegates in te stellen voor het genereren van een voorbeeld.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Initialiseert een nieuw exemplaar van de [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) klasse waardoor de uitvoerstroom wordt gesloten. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Initialiseert een nieuw exemplaar van de [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) klasse waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getWidth()](#getWidth--) | Haalt de breedte van de paginavoorvertoning op. |
|
|  | [setWidth(int width)](#setWidth-int-) | Stelt de breedte van de paginavoorvertoning in. |
|
|  | [getHeight()](#getHeight--) | Haalt de hoogte van het paginavoorbeeld op. |
|
|  | [setHeight(int height)](#setHeight-int-) | Stelt de hoogte van het paginavoorbeeld in. |
|
|  | [getDpi()](#getDpi--) | Haalt een dpi op. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Stelt een dpi in. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Haalt een reeks paginanummers op om voorbeelden te genereren. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Stelt een reeks paginanummers in om voorbeelden te genereren. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Haalt het voorbeeldafbeeldingsformaat op. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Stelt het voorbeeldafbeeldingsformaat in. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Haalt een instantie van de paginastroomcreatie-delegate op. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Stelt een instantie van de paginastroomcreatie-delegate in. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Haalt een instantie van de paginavoorbeeld-voltooiingsdelegate op. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Stelt een instantie van de paginavoorbeeld-voltooiingsdelegate in. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Haalt een instantie van de paginavoorbeeld-renderinfo-delegate op. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Stelt een instantie van de paginavoorbeeld-renderinfo-delegate in. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initialiseert een nieuw exemplaar van de [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) klasse waardoor de uitvoerstroom wordt gesloten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Maakt een stroom voor een specifiek paginavoorbeeld. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initialiseert een nieuw exemplaar van de [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) klasse waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Maakt een stroom voor een specifiek paginavoorbeeld |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Meldt dat de generatie van het paginavoorbeeld is voltooid en haalt de uitvoerstroom op. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Haalt de breedte van de paginavoorvertoning op.


**Returns:**
int - De paginabreedte.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Stelt de breedte van de paginavoorvertoning in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | breedte | int | De paginabreedte. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Haalt de hoogte van het paginavoorbeeld op.


**Returns:**
int - De paginahoogte.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Stelt de hoogte van het paginavoorbeeld in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | hoogte | int | De paginahoogte. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Haalt een dpi op.


**Returns:**
int - Een geheel getal dat een dpi vertegenwoordigt.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Stelt een dpi in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dpi | int | De dpi. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Haalt een reeks paginanummers op om voorbeelden te genereren.


**Returns:**
int[] - Een verzameling paginanummers.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Stelt een reeks paginanummers in om voorbeelden te genereren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageNumbers | int[] | Een verzameling paginanummers. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Haalt het voorbeeldafbeeldingsformaat op.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Stelt het voorbeeldafbeeldingsformaat in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Het preview-formaat. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Haalt een instantie van de paginastroomcreatie-delegate op.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Stelt een instantie van de paginastroomcreatie-delegate in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | De delegate voor het maken van de paginastroom. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Haalt een instantie van de paginavoorbeeld-voltooiingsdelegate op.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Stelt een instantie van de paginavoorbeeld-voltooiingsdelegate in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | De delegate voor het voltooien van de paginapreview. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Haalt een instantie van de paginavoorbeeld-renderinfo-delegate op.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Stelt een instantie van de paginavoorbeeld-renderinfo-delegate in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | De delegate voor renderinformatie van de paginapreview. |
|

