---
title: "내보내기"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "메타데이터 컬렉션을 스트림으로 내보냅니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

메타데이터 컬렉션을 스트림으로 내보냅니다.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 메타데이터 | IEnumerable`1 | 메타데이터 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

메타데이터 컬렉션을 파일로 내보냅니다.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 메타데이터 | IEnumerable`1 | 메타데이터 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

문서 정보를 스트림으로 내보냅니다.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 문서 정보입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

문서 정보를 파일로 내보냅니다.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 문서 정보입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

텍스트 영역 컬렉션을 스트림으로 내보냅니다.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | 텍스트 영역의 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

텍스트 영역 컬렉션을 파일로 내보냅니다.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | 텍스트 영역 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

테이블 컬렉션을 스트림으로 내보냅니다.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 테이블 | IEnumerable`1 | 테이블 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

테이블 컬렉션을 파일로 내보냅니다.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 테이블 | IEnumerable`1 | 테이블 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

바코드 컬렉션을 스트림으로 내보냅니다.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 바코드 | IEnumerable`1 | 바코드 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

바코드 컬렉션을 파일로 내보냅니다.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 바코드 | IEnumerable`1 | 바코드 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

문서 데이터를 스트림으로 내보냅니다.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentData | DocumentData | 문서 데이터입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

문서 데이터를 파일로 내보냅니다.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentData | DocumentData | 문서 데이터입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
