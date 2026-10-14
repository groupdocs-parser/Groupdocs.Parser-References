---
title: "ImageOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "画像抽出に使用されるオプションを提供します。"
type: docs
weight: 23
url: /ja/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

画像抽出に使用されるオプションを提供します。

パラメーターとして使用される [ImageOptions](../../com.groupdocs.parser.options/imageoptions) クラスのインスタンスです
において [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) と
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

画像抽出のための画像形式を指定するために使用されます。

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | 画像抽出に使用されるオプションを提供します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | 画像抽出の画像形式を取得します。 |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


画像抽出に使用されるオプションを提供します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | 画像の形式。 |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


画像抽出の画像形式を取得します。


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

