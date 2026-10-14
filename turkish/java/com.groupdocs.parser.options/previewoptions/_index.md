---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlamak üzere seçenekler sağlar."
type: docs
weight: 34
url: /tr/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlamak üzere seçenekler sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Yeni bir [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) sınıfı örneği başlatır ve çıktı akışının kapatılmasına neden olur. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Yeni bir [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) sınıfı örneği başlatır ve çıktı akışının istemciye daha sonraki kullanım için geri gönderilmesine neden olur. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getWidth()](#getWidth--) | Sayfa önizleme genişliğini alır. |
|
|  | [setWidth(int width)](#setWidth-int-) | Sayfa önizleme genişliğini ayarlar. |
|
|  | [getHeight()](#getHeight--) | Sayfa önizleme yüksekliğini alır. |
|
|  | [setHeight(int height)](#setHeight-int-) | Sayfa önizleme yüksekliğini ayarlar. |
|
|  | [getDpi()](#getDpi--) | dpi değerini alır. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | dpi değerini ayarlar. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Önizlemeler oluşturmak için sayfa numaralarının bir dizisini alır. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Önizlemeler oluşturmak için sayfa numaralarının bir dizisini ayarlar. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Önizleme görüntü formatını alır. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Önizleme görüntü formatını ayarlar. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Sayfa akışı oluşturma temsilcisinin bir örneğini alır. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Sayfa akışı oluşturma temsilcisinin bir örneğini ayarlar. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Sayfa önizleme tamamlama temsilcisinin bir örneğini alır. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Sayfa önizleme tamamlama temsilcisinin bir örneğini ayarlar. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Sayfa önizleme render bilgi temsilcisinin bir örneğini alır. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Sayfa önizleme render bilgi temsilcisinin bir örneğini ayarlar. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Yeni bir [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) sınıfı örneği başlatır ve çıktı akışının kapatılmasına neden olur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Belirli bir sayfa önizlemesi için bir akış oluşturur. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Yeni bir [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) sınıfı örneği başlatır ve çıktı akışının istemciye daha sonraki kullanım için geri gönderilmesine neden olur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Belirli bir sayfa önizlemesi için bir akış oluşturur. |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Sayfa önizleme oluşturulmasının tamamlandığını bildirir ve çıktı akışını alır. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Sayfa önizleme genişliğini alır.


**Returns:**
int - Sayfa genişliği.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Sayfa önizleme genişliğini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | genişlik | int | Sayfa genişliği. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Sayfa önizleme yüksekliğini alır.


**Returns:**
int - Sayfa yüksekliği.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Sayfa önizleme yüksekliğini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yükseklik | int | Sayfa yüksekliği. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


dpi değerini alır.


**Returns:**
int - DPI'yi temsil eden bir tam sayı değeri.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


dpi değerini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dpi | int | DPI. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Önizlemeler oluşturmak için sayfa numaralarının bir dizisini alır.


**Returns:**
int[] - Sayfa numaralarının bir koleksiyonu.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Önizlemeler oluşturmak için sayfa numaralarının bir dizisini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageNumbers | int[] | Sayfa numaralarının bir koleksiyonu. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Önizleme görüntü formatını alır.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Önizleme görüntü formatını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Önizleme formatı. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Sayfa akışı oluşturma temsilcisinin bir örneğini alır.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Sayfa akışı oluşturma temsilcisinin bir örneğini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Sayfa akışı oluşturma temsilcisi. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Sayfa önizleme tamamlama temsilcisinin bir örneğini alır.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Sayfa önizleme tamamlama temsilcisinin bir örneğini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Sayfa önizleme tamamlama temsilcisi. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Sayfa önizleme render bilgi temsilcisinin bir örneğini alır.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Sayfa önizleme render bilgi temsilcisinin bir örneğini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Sayfa önizleme render bilgi temsilcisi. |
|

