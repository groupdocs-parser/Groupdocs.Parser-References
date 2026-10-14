---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen."
type: docs
weight: 34
url: /de/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Initialisiert eine neue Instanz der Klasse [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), wodurch der Ausgabestream geschlossen wird. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Initialisiert eine neue Instanz der Klasse [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), wodurch der Ausgabestream dem Client zur weiteren Verwendung zurückgegeben wird. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getWidth()](#getWidth--) | Liefert die Breite der Seitenvorschau. |
|
|  | [setWidth(int width)](#setWidth-int-) | Setzt die Breite der Seitenvorschau. |
|
|  | [getHeight()](#getHeight--) | Ermittelt die Höhe der Seitenvorschau. |
|
|  | [setHeight(int height)](#setHeight-int-) | Legt die Höhe der Seitenvorschau fest. |
|
|  | [getDpi()](#getDpi--) | Ermittelt einen dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Legt einen dpi fest. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Ermittelt ein Array von Seitenzahlen, um Vorschauen zu erzeugen. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Legt ein Array von Seitenzahlen fest, um Vorschauen zu erzeugen. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Ermittelt das Vorschaubildformat. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Legt das Vorschaubildformat fest. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Ermittelt eine Instanz des Delegaten zur Erstellung des Seitenstroms. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Legt eine Instanz des Delegaten zur Erstellung des Seitenstroms fest. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Ermittelt eine Instanz des Delegaten für den Abschluss der Seitenvorschau. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Legt eine Instanz des Delegaten für den Abschluss der Seitenvorschau fest. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Ermittelt eine Instanz des Delegaten für Renderinformationen der Seitenvorschau. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Legt eine Instanz des Delegaten für Renderinformationen der Seitenvorschau fest. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initialisiert eine neue Instanz der Klasse [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), wodurch der Ausgabestream geschlossen wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Erstellt einen Stream für eine bestimmte Seitenvorschau. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initialisiert eine neue Instanz der Klasse [PreviewOptions](../../com.groupdocs.parser.options/previewoptions), wodurch der Ausgabestream dem Client zur weiteren Verwendung zurückgegeben wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Erstellt einen Stream für eine bestimmte Seitenvorschau |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Benachrichtigt, dass die Erzeugung der Seitenvorschau abgeschlossen ist, und ermittelt den Ausgabestream. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Liefert die Breite der Seitenvorschau.


**Returns:**
int - Die Seitenbreite.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Setzt die Breite der Seitenvorschau.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Breite | int | Die Seitenbreite. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Ermittelt die Höhe der Seitenvorschau.


**Returns:**
int - Die Seitenhöhe.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Legt die Höhe der Seitenvorschau fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Höhe | int | Die Seitenhöhe. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Ermittelt einen dpi.


**Returns:**
int - Ein ganzzahliger Wert, der einen dpi darstellt.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Legt einen dpi fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dpi | int | Die DPI. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Ermittelt ein Array von Seitenzahlen, um Vorschauen zu erzeugen.


**Returns:**
int[] - Eine Sammlung von Seitenzahlen.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Legt ein Array von Seitenzahlen fest, um Vorschauen zu erzeugen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageNumbers | int[] | Eine Sammlung von Seitenzahlen. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Ermittelt das Vorschaubildformat.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Legt das Vorschaubildformat fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Das Vorschaformat. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Ermittelt eine Instanz des Delegaten zur Erstellung des Seitenstroms.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Legt eine Instanz des Delegaten zur Erstellung des Seitenstroms fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Der Delegat zur Erstellung des Seitenstroms. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Ermittelt eine Instanz des Delegaten für den Abschluss der Seitenvorschau.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Legt eine Instanz des Delegaten für den Abschluss der Seitenvorschau fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Der Delegat für den Abschluss der Seitenvorschau. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Ermittelt eine Instanz des Delegaten für Renderinformationen der Seitenvorschau.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Legt eine Instanz des Delegaten für Renderinformationen der Seitenvorschau fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Der Delegat für Renderinformationen der Seitenvorschau. |
|

