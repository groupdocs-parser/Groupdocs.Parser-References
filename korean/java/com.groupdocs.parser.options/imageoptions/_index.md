---
title: "ImageOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "이미지 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 23
url: /ko/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

이미지 추출에 사용되는 옵션을 제공합니다.

파라미터로 사용되는 [ImageOptions](../../com.groupdocs.parser.options/imageoptions) 클래스의 인스턴스입니다.
다음에서 [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) 및
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

이미지 추출을 위한 이미지 형식을 지정하는 데 사용됩니다.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | 이미지 추출에 사용되는 옵션을 제공합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | 이미지 추출을 위한 이미지 형식을 가져옵니다. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


이미지 추출에 사용되는 옵션을 제공합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | 이미지의 형식입니다. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


이미지 추출을 위한 이미지 형식을 가져옵니다.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

