---
title: "LoadOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der LoadOptionsgroupdocs.parser.options/loadoptions‑Klasse mit leerem Passwordgroupdocs.parser.options/loadoptions/password, FileFormatgroupdocs.parser.options/loadoptions/fileformat gleich Unknown und Standardkodierungen."
type: docs
weight: 10
url: /de/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit leerem [`Password`](../password), [`FileFormat`](../fileformat) gleich Unknown und Standardkodierungen.

```csharp
public LoadOptions()
```

### Siehe auch

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| timeout | TimeSpan | Der TimeSpan, der die Anzahl der Millisekunden zum Warten darstellt. |

### Siehe auch

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit [`FileFormat`](../fileformat) gleich Unknown und Standardcodierungen.

```csharp
public LoadOptions(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |

### Siehe auch

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit leerem [`Password`](../password) und Standardcodierungen.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileFormat | FileFormat | Das Format der Datei. |

### Siehe auch

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit dem Passwort und Standardcodierungen.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileFormat | FileFormat | Das Format der Datei. |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |

### Siehe auch

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit benutzerdefinierten Codierungen.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileFormat | FileFormat | Das Format der Datei. |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |
| encoding | Encoding | Die Codierung des Dokuments. |
| defaultAnsiEncoding | Encoding | Die standardmäßige ANSI-Codierung, die zur Codierungserkennung verwendet wird. |

### Siehe auch

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Initialisiert eine neue Instanz der vollständig angepassten [`LoadOptions`](../../loadoptions)-Klasse.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileFormat | FileFormat | Das Format der Datei. |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |
| encoding | Encoding | Die Codierung des Dokuments. |
| defaultAnsiEncoding | Encoding | Die standardmäßige ANSI-Codierung, die zur Codierungserkennung verwendet wird. |
| timeout | TimeSpan | Der TimeSpan, der die Anzahl der Millisekunden zum Warten darstellt. |

### Siehe auch

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit leerem [`Password`](../password) und Standardcodierungen.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileType | FileType | Der Typ der Datei. |

### Siehe auch

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit dem Passwort und Standardcodierungen.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileType | FileType | Der Typ der Datei. |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |

### Siehe auch

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Initialisiert eine neue Instanz der [`LoadOptions`](../../loadoptions)-Klasse mit benutzerdefinierten Codierungen.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileType | FileType | Der Typ der Datei. |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |
| encoding | Encoding | Die Codierung des Dokuments. |
| defaultAnsiEncoding | Encoding | Die standardmäßige ANSI-Codierung, die zur Codierungserkennung verwendet wird. |

### Siehe auch

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Initialisiert eine neue Instanz der vollständig angepassten [`LoadOptions`](../../loadoptions)-Klasse.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileType | FileType | Der Typ der Datei. |
| password | String | Das Passwort zum Öffnen der passwortgeschützten Datei. |
| encoding | Encoding | Die Codierung des Dokuments. |
| defaultAnsiEncoding | Encoding | Die standardmäßige ANSI-Codierung, die zur Codierungserkennung verwendet wird. |
| timeout | TimeSpan | Der TimeSpan, der die Anzahl der Millisekunden zum Warten darstellt. |

### Siehe auch

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
