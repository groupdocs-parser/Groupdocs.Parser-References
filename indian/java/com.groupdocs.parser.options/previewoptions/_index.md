---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "प्रिव्यू जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट्स सेट करने के विकल्प प्रदान करता है।"
type: docs
weight: 34
url: /hi/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

प्रिव्यू जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट्स सेट करने के विकल्प प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | नया [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) क्लास का एक उदाहरण प्रारंभ करता है जिससे आउटपुट स्ट्रीम बंद हो जाता है। |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | नया [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) क्लास का एक उदाहरण प्रारंभ करता है जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस किया जाता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getWidth()](#getWidth--) | पृष्ठ पूर्वावलोकन की चौड़ाई प्राप्त करता है। |
|
|  | [setWidth(int width)](#setWidth-int-) | पृष्ठ पूर्वावलोकन की चौड़ाई सेट करता है। |
|
|  | [getHeight()](#getHeight--) | पृष्ठ पूर्वावलोकन की ऊँचाई प्राप्त करता है। |
|
|  | [setHeight(int height)](#setHeight-int-) | पृष्ठ पूर्वावलोकन की ऊँचाई सेट करता है। |
|
|  | [getDpi()](#getDpi--) | एक dpi प्राप्त करता है। |
|
|  | [setDpi(int dpi)](#setDpi-int-) | एक dpi सेट करता है। |
|
|  | [getPageNumbers()](#getPageNumbers--) | पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी प्राप्त करता है। |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी सेट करता है। |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | पूर्वावलोकन छवि प्रारूप प्राप्त करता है। |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | पूर्वावलोकन छवि प्रारूप सेट करता है। |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण प्राप्त करता है। |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण सेट करता है। |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण प्राप्त करता है। |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण सेट करता है। |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | पृष्ठ पूर्वावलोकन रेंडर जानकारी प्रतिनिधि का एक उदाहरण प्राप्त करता है। |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | पृष्ठ पूर्वावलोकन रेंडर जानकारी प्रतिनिधि का एक उदाहरण सेट करता है। |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


नया [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) क्लास का एक उदाहरण प्रारंभ करता है जिससे आउटपुट स्ट्रीम बंद हो जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | विशिष्ट पृष्ठ पूर्वावलोकन के लिए एक स्ट्रीम बनाता है। |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


नया [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) क्लास का एक उदाहरण प्रारंभ करता है जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | विशिष्ट पृष्ठ पूर्वावलोकन के लिए एक स्ट्रीम बनाता है |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | सूचित करता है कि पृष्ठ पूर्वावलोकन निर्माण समाप्त हो गया है और आउटपुट स्ट्रीम प्राप्त करता है। |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


पृष्ठ पूर्वावलोकन की चौड़ाई प्राप्त करता है।


**Returns:**
int - पृष्ठ की चौड़ाई।

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


पृष्ठ पूर्वावलोकन की चौड़ाई सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | चौड़ाई | int | पृष्ठ की चौड़ाई। |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


पृष्ठ पूर्वावलोकन की ऊँचाई प्राप्त करता है।


**Returns:**
int - पृष्ठ की ऊँचाई।

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


पृष्ठ पूर्वावलोकन की ऊँचाई सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | ऊँचाई | int | पृष्ठ की ऊँचाई। |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


एक dpi प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो dpi को दर्शाता है।

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


एक dpi सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dpi | int | डॉट्स प्रति इंच। |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी प्राप्त करता है।


**Returns:**
int[] - पृष्ठ संख्याओं का संग्रह।

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageNumbers | int[] | पृष्ठ संख्याओं का संग्रह। |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


पूर्वावलोकन छवि प्रारूप प्राप्त करता है।


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


पूर्वावलोकन छवि प्रारूप सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | पूर्वावलोकन प्रारूप। |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण प्राप्त करता है।


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | पृष्ठ स्ट्रीम निर्माण प्रतिनिधि। |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण प्राप्त करता है।


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि। |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


पृष्ठ पूर्वावलोकन रेंडर जानकारी प्रतिनिधि का एक उदाहरण प्राप्त करता है।


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


पृष्ठ पूर्वावलोकन रेंडर जानकारी प्रतिनिधि का एक उदाहरण सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | पृष्ठ पूर्वावलोकन रेंडर जानकारी प्रतिनिधि। |
|

