---
title: "ContainerItem"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "Zip 아카이브 엔터티, 이메일 첨부 파일, PDF 포트폴리오 항목 등과 같은 컨테이너 항목을 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Zip 아카이브 엔터티, 이메일 첨부 파일, PDF 포트폴리오 항목 등과 같은 컨테이너 항목을 나타냅니다.

클래스 [ContainerItem](../../com.groupdocs.parser.data/containeritem)의 인스턴스가 [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) 메서드의 반환 값으로 사용됩니다. 해당 사용 예제를 확인하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | [ContainerItem](../../com.groupdocs.parser.data/containeritem)의 새 인스턴스를 항목 이름과 디렉터리로 초기화합니다. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | [ContainerItem](../../com.groupdocs.parser.data/containeritem)의 새 인스턴스를 항목 전체 경로로 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getName()](#getName--) | 항목의 이름을 가져옵니다. |
|
|  | [getDirectory()](#getDirectory--) | 항목의 디렉터리를 가져옵니다. |
|
|  | [getFilePath()](#getFilePath--) | 항목의 전체 경로를 가져옵니다. |
|
|  | [getSize()](#getSize--) | 항목의 크기를 가져옵니다. |
|
|  | [getMetadata()](#getMetadata--) | 메타데이터 항목의 컬렉션을 가져옵니다. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | 메타데이터 값을 가져옵니다. |
|
|  | [openStream()](#openStream--) | 항목 콘텐츠의 스트림을 엽니다. |
|
|  | [openParser()](#openParser--) | 항목 콘텐츠를 위한 [Parser](../../com.groupdocs.parser/parser) 객체를 생성합니다. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | 항목 콘텐츠에 대해 [Parser](../../com.groupdocs.parser/parser) 객체를 [LoadOptions](../../com.groupdocs.parser.options/loadoptions)와 함께 생성합니다. |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 항목 콘텐츠에 대해 [Parser](../../com.groupdocs.parser/parser) 객체를 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 및 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)와 함께 생성합니다. |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | 컨테이너 항목의 파일 유형을 감지합니다. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


[ContainerItem](../../com.groupdocs.parser.data/containeritem)의 새 인스턴스를 항목 이름과 디렉터리로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 이름 | java.lang.String | 항목의 이름입니다. |
|
|  | 디렉터리 | java.lang.String | 항목의 디렉터리입니다. |
|
|  | size | long | 항목의 크기입니다. |
|
|  | 메타데이터 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 메타데이터 항목들의 컬렉션입니다. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


[ContainerItem](../../com.groupdocs.parser.data/containeritem)의 새 인스턴스를 항목 전체 경로로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 항목의 전체 경로입니다. |
|
|  | size | long | 항목의 크기입니다. |
|
|  | 메타데이터 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 메타데이터 항목들의 컬렉션입니다. |
|

### getName() {#getName--}
```
public String getName()
```


항목의 이름을 가져옵니다.


**Returns:**
java.lang.String - 항목의 파일 이름(디렉터리 제외)을 나타내는 문자열 값입니다.

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


항목의 디렉터리를 가져옵니다.


**Returns:**
java.lang.String - 항목의 디렉터리(파일 이름 제외)를 나타내는 문자열 값입니다.

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


항목의 전체 경로를 가져옵니다.


**Returns:**
java.lang.String - 항목의 전체 경로를 나타내는 문자열 값입니다.

### getSize() {#getSize--}
```
public long getSize()
```


항목의 크기를 가져옵니다.


**Returns:**
long - 항목의 크기를 바이트 단위로 나타내는 정수 값입니다.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


메타데이터 항목의 컬렉션을 가져옵니다.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - [MetadataItem](../../com.groupdocs.parser.data/metadataitem) 객체들의 컬렉션; 메타데이터가 설정되지 않은 경우 비어 있습니다.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


메타데이터 값을 가져옵니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 이름 | java.lang.String | 메타데이터의 이름입니다. |
|

**Returns:**
java.lang.String - 메타데이터 항목의 값을 나타내는 문자열 값; 해당 이름의 메타데이터를 찾을 수 없으면  null  입니다.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


항목 콘텐츠의 스트림을 엽니다.


**Returns:**
java.io.InputStream - 항목 콘텐츠를 포함하는 스트림입니다.

### openParser() {#openParser--}
```
public Parser openParser()
```


항목 콘텐츠를 위한 [Parser](../../com.groupdocs.parser/parser) 객체를 생성합니다.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


항목 콘텐츠에 대해 [Parser](../../com.groupdocs.parser/parser) 객체를 [LoadOptions](../../com.groupdocs.parser.options/loadoptions)와 함께 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 항목 콘텐츠를 열기 위한 옵션입니다. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


항목 콘텐츠에 대해 [Parser](../../com.groupdocs.parser/parser) 객체를 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 및 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)와 함께 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 항목 콘텐츠를 열기 위한 옵션입니다. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


컨테이너 항목의 파일 유형을 감지합니다.


detectionMode
parameter는 파일 유형 감지를 제어할 수 있는 기능을 제공합니다:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

다음 예제는 컨테이너 항목의 파일 유형을 감지하는 방법을 보여줍니다:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | 파일 유형 감지 모드를 정의합니다. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

