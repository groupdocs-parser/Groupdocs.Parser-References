---
title: "ExportAsXml"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "메타데이터 컬렉션을 XML 형식으로 스트림에 내보냅니다."
type: docs
weight: 20
url: /ko/net/groupdocs.parser.export/extensions/exportasxml/
---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasxml_4}

메타데이터 컬렉션을 XML 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 메타데이터 | IEnumerable`1 | 메타데이터 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasxml_5}

메타데이터 컬렉션을 XML 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 메타데이터 | IEnumerable`1 | 메타데이터 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, Stream) {#exportasxml_2}

문서 정보를 XML 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 문서 정보입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, string) {#exportasxml_3}

문서 정보를 XML 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 문서 정보입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasxml_10}

텍스트 영역 컬렉션을 XML 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | 텍스트 영역의 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasxml_11}

텍스트 영역 collectiob을 XML 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | 텍스트 영역 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasxml_8}

테이블 컬렉션을 XML 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 테이블 | IEnumerable`1 | 테이블 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasxml_9}

테이블 컬렉션을 XML 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 테이블 | IEnumerable`1 | 테이블 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasxml_6}

바코드 컬렉션을 XML 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 바코드 | IEnumerable`1 | 바코드 컬렉션입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasxml_7}

바코드 컬렉션을 XML 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 바코드 | IEnumerable`1 | 바코드 컬렉션입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, Stream) {#exportasxml}

문서 데이터를 XML 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsXml(this DocumentData documentData, Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentData | DocumentData | 문서 데이터입니다. |
| 스트림 | Stream | 출력 스트림입니다. |

### 참고

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, string) {#exportasxml_1}

문서 데이터를 XML 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsXml(this DocumentData documentData, string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| documentData | DocumentData | 문서 데이터입니다. |
| fileName | 문자열 | 출력 파일에 대한 전체 경로입니다. |

### 참고

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
