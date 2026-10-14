---
title: "XmlExporter"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "XML 형식으로 데이터를 내보내는 기능을 제공합니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

XML 형식으로 데이터를 내보내는 기능을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | 새로운 [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | 메타데이터 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | 문서 정보를 스트림으로 내보냅니다. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | 텍스트 영역 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | 테이블 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | 바코드 컬렉션을 스트림으로 내보냅니다. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | 문서 데이터를 스트림으로 내보냅니다. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


새로운 [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) 클래스 인스턴스를 초기화합니다.


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


메타데이터 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 메타데이터 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 메타데이터 컬렉션. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


문서 정보를 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 문서 정보. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


텍스트 영역 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 텍스트 영역의 컬렉션. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


테이블 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 테이블 | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | 테이블 컬렉션입니다. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


바코드 컬렉션을 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 바코드 | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | 바코드 컬렉션입니다. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


문서 데이터를 스트림으로 내보냅니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 문서 데이터. |
|
|  | outputStream | java.io.OutputStream | 출력 스트림. |
|

