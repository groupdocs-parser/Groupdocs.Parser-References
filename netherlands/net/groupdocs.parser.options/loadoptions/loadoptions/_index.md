---
title: "LoadOptions"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Initialiseert een nieuw exemplaar van de LoadOptionsgroupdocs.parser.options/loadoptions‑klasse met een lege Passwordgroupdocs.parser.options/loadoptions/password, FileFormatgroupdocs.parser.options/loadoptions/fileformat gelijk aan Unknown en standaardcoderingen."
type: docs
weight: 10
url: /nl/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met een lege [`Password`](../password), [`FileFormat`](../fileformat) gelijk aan Unknown en standaardcoderingen.

```csharp
public LoadOptions()
```

### Zie ook

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| timeout | TimeSpan | De TimeSpan die het aantal milliseconden dat gewacht moet worden vertegenwoordigt. |

### Zie ook

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met [`FileFormat`](../fileformat) gelijk aan Unknown en standaardcoderingen.

```csharp
public LoadOptions(string password)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |

### Zie ook

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met een lege [`Password`](../password) en standaardcoderingen.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileFormat | FileFormat | Het formaat van het bestand. |

### Zie ook

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met het wachtwoord en standaardcoderingen.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileFormat | FileFormat | Het formaat van het bestand. |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |

### Zie ook

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met aangepaste coderingen.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileFormat | FileFormat | Het formaat van het bestand. |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
| encoding | Encoding | De codering van het document. |
| defaultAnsiEncoding | Encoding | De standaard ANSI‑codering die wordt gebruikt voor coderingsdetectie. |

### Zie ook

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Initialiseert een nieuw exemplaar van de volledig aangepaste [`LoadOptions`](../../loadoptions)‑klasse.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileFormat | FileFormat | Het formaat van het bestand. |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
| encoding | Encoding | De codering van het document. |
| defaultAnsiEncoding | Encoding | De standaard ANSI‑codering die wordt gebruikt voor coderingsdetectie. |
| timeout | TimeSpan | De TimeSpan die het aantal milliseconden dat gewacht moet worden vertegenwoordigt. |

### Zie ook

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met een lege [`Password`](../password) en standaardcoderingen.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileType | FileType | Het type van het bestand. |

### Zie ook

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met het wachtwoord en standaardcoderingen.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileType | FileType | Het type van het bestand. |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |

### Zie ook

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Initialiseert een nieuw exemplaar van de [`LoadOptions`](../../loadoptions)‑klasse met aangepaste coderingen.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileType | FileType | Het type van het bestand. |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
| encoding | Encoding | De codering van het document. |
| defaultAnsiEncoding | Encoding | De standaard ANSI‑codering die wordt gebruikt voor coderingsdetectie. |

### Zie ook

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Initialiseert een nieuw exemplaar van de volledig aangepaste [`LoadOptions`](../../loadoptions)‑klasse.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileType | FileType | Het type van het bestand. |
| password | String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
| encoding | Encoding | De codering van het document. |
| defaultAnsiEncoding | Encoding | De standaard ANSI‑codering die wordt gebruikt voor coderingsdetectie. |
| timeout | TimeSpan | De TimeSpan die het aantal milliseconden dat gewacht moet worden vertegenwoordigt. |

### Zie ook

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
