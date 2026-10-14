---
title: "PreviewOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus."
type: docs
weight: 34
url: /fr/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Initialise une nouvelle instance de la classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) entraînant la fermeture du flux de sortie. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Initialise une nouvelle instance de la classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) entraînant le retour du flux de sortie au client pour une utilisation ultérieure. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getWidth()](#getWidth--) | Obtient la largeur de l'aperçu de la page. |
|
|  | [setWidth(int width)](#setWidth-int-) | Définit la largeur de l'aperçu de la page. |
|
|  | [getHeight()](#getHeight--) | Obtient la hauteur de l'aperçu de la page. |
|
|  | [setHeight(int height)](#setHeight-int-) | Définit la hauteur de l'aperçu de la page. |
|
|  | [getDpi()](#getDpi--) | Obtient un dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Définit un dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Obtient un tableau de numéros de page pour générer des aperçus. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Définit un tableau de numéros de page pour générer des aperçus. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Obtient le format de l'image d'aperçu. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Définit le format de l'image d'aperçu. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Obtient une instance du délégué de création du flux de page. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Définit une instance du délégué de création du flux de page. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Obtient une instance du délégué de fin d'aperçu de page. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Définit une instance du délégué de fin d'aperçu de page. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Obtient une instance du délégué d'informations de rendu de l'aperçu de page. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Définit une instance du délégué d'informations de rendu de l'aperçu de page. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initialise une nouvelle instance de la classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) entraînant la fermeture du flux de sortie.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Crée un flux pour un aperçu de page spécifique. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initialise une nouvelle instance de la classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) entraînant le retour du flux de sortie au client pour une utilisation ultérieure.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Crée un flux pour un aperçu de page spécifique |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Notifie que la génération de l'aperçu de la page est terminée et récupère le flux de sortie. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Obtient la largeur de l'aperçu de la page.


**Returns:**
int - La largeur de la page.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Définit la largeur de l'aperçu de la page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | largeur | int | La largeur de la page. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Obtient la hauteur de l'aperçu de la page.


**Returns:**
int - La hauteur de la page.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Définit la hauteur de l'aperçu de la page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | hauteur | int | La hauteur de la page. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Obtient un dpi.


**Returns:**
int - Une valeur entière qui représente un dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Définit un dpi.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | dpi | int | Le dpi. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Obtient un tableau de numéros de page pour générer des aperçus.


**Returns:**
int[] - Une collection de numéros de page.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Définit un tableau de numéros de page pour générer des aperçus.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | pageNumbers | int[] | Une collection de numéros de page. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Obtient le format de l'image d'aperçu.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Définit le format de l'image d'aperçu.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Le format d'aperçu. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Obtient une instance du délégué de création du flux de page.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Définit une instance du délégué de création du flux de page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Le délégué de création du flux de page. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Obtient une instance du délégué de fin d'aperçu de page.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Définit une instance du délégué de fin d'aperçu de page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Le délégué d'achèvement de l'aperçu de la page. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Obtient une instance du délégué d'informations de rendu de l'aperçu de page.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Définit une instance du délégué d'informations de rendu de l'aperçu de page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Le délégué d'informations de rendu de l'aperçu de la page. |
|

