---
title: "ExportAsJson"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "메타데이터 컬렉션을 JSON 형식으로 스트림에 내보냅니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.export/extensions/exportasjson/
---

## ExportAsJson(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasjson_4}

메타데이터 컬렉션을 JSON 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<MetadataItem> metadata, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasjson_5}

메타데이터 컬렉션을 JSON 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<MetadataItem> metadata, string fileName)
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

## ExportAsJson(this IDocumentInfo, Stream) {#exportasjson_2}

문서 정보를 JSON 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsJson(this IDocumentInfo documentInfo, Stream stream)
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

## ExportAsJson(this IDocumentInfo, string) {#exportasjson_3}

문서 정보를 JSON 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsJson(this IDocumentInfo documentInfo, string fileName)
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

## ExportAsJson(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasjson_10}

텍스트 영역 컬렉션을 JSON 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<PageTextArea> textAreas, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasjson_11}

텍스트 영역 collectiob을 JSON 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<PageTextArea> textAreas, string fileName)
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

## ExportAsJson(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasjson_8}

테이블 컬렉션을 JSON 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<PageTableArea> tables, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasjson_9}

테이블 컬렉션을 JSON 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<PageTableArea> tables, string fileName)
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

## ExportAsJson(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasjson_6}

바코드 컬렉션을 JSON 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasjson_7}

바코드 컬렉션을 JSON 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsJson(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
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

## ExportAsJson(this DocumentData, Stream) {#exportasjson}

문서 데이터를 JSON 형식으로 스트림에 내보냅니다.

```csharp
public static void ExportAsJson(this DocumentData documentData, Stream stream)
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

## ExportAsJson(this DocumentData, string) {#exportasjson_1}

문서 데이터를 JSON 형식으로 파일에 내보냅니다.

```csharp
public static void ExportAsJson(this DocumentData documentData, string fileName)
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
