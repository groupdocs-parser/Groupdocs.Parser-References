---
title: "PageImageArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート解析機能でページ上の画像を表すために使用されるページ画像領域、またはメールや Zip アーカイブから抽出された画像が画像添付ファイルの場合に使用されます。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

テンプレート解析機能でページ上の画像を表すために使用されるページ画像領域、またはメールや Zip アーカイブから抽出された画像が画像添付ファイルの場合に使用されます。

以下のメソッドの戻り値として、[PageImageArea](../../com.groupdocs.parser.data/pageimagearea) クラスのインスタンスが使用されます：

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

そこにある使用例をご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 画像のフォーマットを取得します。 |
|
|  | [getRotation()](#getRotation--) | 画像の回転角度を取得します。 |
|
|  | [getImageStream()](#getImageStream--) | 画像ストリームを返します。 |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | 画像ストリームを別のフォーマットで返します。 |
|
|  | [save(String filePath)](#save-java.lang.String-) | 画像をファイルに保存します。 |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | 画像を別の形式でファイルに保存します。 |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


[PageImageArea](../../com.groupdocs.parser.data/pageimagearea) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 画像のストリームです。 |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 画像の形式。 |
|
|  | 回転 | double | 画像の回転角度です。 |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


[PageImageArea](../../com.groupdocs.parser.data/pageimagearea) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 画像のストリームです。 |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 画像の形式。 |
|
|  | 回転 | double | 画像の回転角度です。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 画像を含むページです。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 画像を含む矩形領域です。 |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


画像のフォーマットを取得します。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


画像の回転角度を取得します。


**Returns:**
double - 画像の回転角度を表す double 値です。

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


画像ストリームを返します。

次の例は画像をファイルに保存する方法を示しています：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }
     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images) {
         // Open the image stream
         try (InputStream imageStream = image.getImageStream()) {
             // Create the file to save image
             try (OutputStream destStream = new FileOutputStream(imageNumber + image.getFileType().getExtension())) {
                 byte[] buffer = new byte[4096];
                 int readed = 0;
                 do {
                     // Read data from the image stream
                     readed = imageStream.read(buffer, 0, buffer.length);
                     if (readed > 0) {
                         // Write data to the file stream
                         destStream.write(buffer, 0, readed);
                     }
                 }
                 while (readed > 0);
             }
             imageNumber++;
         }
     }
 }
 
````



**Returns:**
java.io.InputStream - 画像を含むストリームです。

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


画像ストリームを別のフォーマットで返します。

次の例は PNG 形式で画像を保存する方法を示しています：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }

     // Create the options to save images in PNG format
     ImageOptions options = new ImageOptions(ImageFormat.Png);

     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images) {
         // Open the image stream
         try (InputStream imageStream = image.getImageStream(options)) {
             // Create the file to save image
             try (OutputStream destStream = new FileOutputStream(imageNumber + ".png")) {
                 byte[] buffer = new byte[4096];
                 int readed = 0;
                 do {
                     // Read data from the image stream
                     readed = imageStream.read(buffer, 0, buffer.length);
                     if (readed > 0) {
                         // Write data to the file stream
                         destStream.write(buffer, 0, readed);
                     }
                 }
                 while (readed > 0);
             }
             imageNumber++;
         }
     }
 }
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | 画像を抽出するために使用されるオプションです。 |
|

**Returns:**
java.io.InputStream - 画像を含むストリームです

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


画像をファイルに保存します。

次の例は画像をファイルに保存する方法を示しています：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();

     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }

     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images)
     {
         // Save the image to the file
         image.save(Constants.getOutputFilePath(String.format("%d", imageNumber) + image.getFileType().getExtension()));

         imageNumber++;
     }
 }
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


画像を別の形式でファイルに保存します。

次の例は PNG 形式で画像をファイルに保存する方法を示しています：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();

     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }

     // Create the options to save images in PNG format
     ImageOptions options = new ImageOptions(ImageFormat.Png);

     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images)
     {
         // Save the image to the png file
         image.save(Constants.getOutputFilePath(String.format("%d.png", imageNumber)), options);

         imageNumber++;
     }
 }
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | 画像を保存するために使用されるオプションです。 |
|

