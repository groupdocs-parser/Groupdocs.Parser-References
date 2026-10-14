---
title: "ExporterBase"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "데이터 내보내기 기능을 위한 기본 클래스를 제공합니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

데이터 내보내기 기능을 위한 기본 클래스를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | 메타데이터 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | 메타데이터 컬렉션을 파일로 내보냅니다. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | 문서 정보를 스트림으로 내보냅니다. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | 문서 정보를 파일로 내보냅니다. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | 텍스트 영역 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | 텍스트 영역 컬렉션을 파일로 내보냅니다. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | 테이블 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | 테이블 컬렉션을 파일로 내보냅니다. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | 바코드 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | 바코드 컬렉션을 파일로 내보냅니다. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | 문서 데이터를 스트림으로 내보냅니다. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | 문서 데이터를 파일로 내보냅니다. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


메타데이터 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 메타데이터 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 메타데이터 컬렉션. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


메타데이터 컬렉션을 파일로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 메타데이터 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 메타데이터 컬렉션. |
|
|  | fileName | java.lang.String | 출력 파일에 대한 전체 경로. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


문서 정보를 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 문서 정보. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


문서 정보를 파일로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 문서 정보. |
|
|  | fileName | java.lang.String | 출력 파일에 대한 전체 경로. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


텍스트 영역 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 텍스트 영역의 컬렉션. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


텍스트 영역 컬렉션을 파일로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 텍스트 영역 컬렉션. |
|
|  | fileName | java.lang.String | 출력 파일에 대한 전체 경로. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


테이블 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 테이블 | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | 테이블 컬렉션입니다. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


테이블 컬렉션을 파일로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 테이블 | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | 테이블 컬렉션입니다. |
|
|  | fileName | java.lang.String | 출력 파일에 대한 전체 경로. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


바코드 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 바코드 | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | 바코드 컬렉션입니다. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


바코드 컬렉션을 파일로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 바코드 | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | 바코드 컬렉션입니다. |
|
|  | fileName | java.lang.String | 출력 파일에 대한 전체 경로. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


문서 데이터를 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 문서 데이터. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


문서 데이터를 파일로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 문서 데이터. |
|
|  | fileName | java.lang.String | 출력 파일에 대한 전체 경로. |
|

