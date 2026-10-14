---
title: "PreviewOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller alternativ för att ange krav och strömdelegater för förhandsgranskningsgenerering."
type: docs
weight: 34
url: /sv/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Tillhandahåller alternativ för att ange krav och strömdelegater för förhandsgranskningsgenerering.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Initierar en ny instans av klassen [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) som får utdataströmmen att stängas. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Initierar en ny instans av klassen [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) som får utdataströmmen att returneras till klienten för vidare användning. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getWidth()](#getWidth--) | Hämtar sidans förhandsgranskningsbredd. |
|
|  | [setWidth(int width)](#setWidth-int-) | Ställer in sidans förhandsgranskningsbredd. |
|
|  | [getHeight()](#getHeight--) | Hämtar sidans förhandsgranskningshöjd. |
|
|  | [setHeight(int height)](#setHeight-int-) | Ställer in sidans förhandsgranskningshöjd. |
|
|  | [getDpi()](#getDpi--) | Hämtar ett dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Ställer in ett dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Hämtar en array av sidnummer för att generera förhandsgranskningar. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Ställer in en array av sidnummer för att generera förhandsgranskningar. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Hämtar förhandsgranskningsbildformatet. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Ställer in förhandsgranskningsbildformatet. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Hämtar en instans av delegaten för skapande av sidström. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Ställer in en instans av delegaten för skapande av sidström. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Hämtar en instans av delegaten för slutförande av sidförhandsgranskning. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Ställer in en instans av delegaten för slutförande av sidförhandsgranskning. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Hämtar en instans av delegaten för renderingsinformation för sidförhandsgranskning. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Ställer in en instans av delegaten för renderingsinformation för sidförhandsgranskning. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initierar en ny instans av klassen [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) som får utdataströmmen att stängas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Skapar en ström för en specifik sidförhandsgranskning. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initierar en ny instans av klassen [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) som får utdataströmmen att returneras till klienten för vidare användning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Skapar en ström för en specifik sidförhandsgranskning |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Meddelar att sidförhandsgranskningens generering är klar och hämtar utdataströmmen. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Hämtar sidans förhandsgranskningsbredd.


**Returns:**
int - Sidans bredd.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Ställer in sidans förhandsgranskningsbredd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | bredd | int | Sidans bredd. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Hämtar sidans förhandsgranskningshöjd.


**Returns:**
int - Sidans höjd.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Ställer in sidans förhandsgranskningshöjd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | höjd | int | Sidans höjd. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Hämtar ett dpi.


**Returns:**
int - Ett heltal som representerar ett dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Ställer in ett dpi.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dpi | int | Dpi:n. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Hämtar en array av sidnummer för att generera förhandsgranskningar.


**Returns:**
int[] - En samling av sidnummer.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Ställer in en array av sidnummer för att generera förhandsgranskningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageNumbers | int[] | En samling av sidnummer. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Hämtar förhandsgranskningsbildformatet.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Ställer in förhandsgranskningsbildformatet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Förhandsgranskningsformatet. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Hämtar en instans av delegaten för skapande av sidström.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Ställer in en instans av delegaten för skapande av sidström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Delegaten för skapande av sidström. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Hämtar en instans av delegaten för slutförande av sidförhandsgranskning.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Ställer in en instans av delegaten för slutförande av sidförhandsgranskning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Delegaten för slutförande av sidförhandsgranskning. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Hämtar en instans av delegaten för renderingsinformation för sidförhandsgranskning.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Ställer in en instans av delegaten för renderingsinformation för sidförhandsgranskning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Delegaten för renderingsinformation för sidförhandsgranskning. |
|

