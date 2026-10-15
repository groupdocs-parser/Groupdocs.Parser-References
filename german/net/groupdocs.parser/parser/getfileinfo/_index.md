---
title: "GetFileInfo"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Gibt die allgemeinen Informationen zu einer Datei zurück."
type: docs
weight: 260
url: /de/net/groupdocs.parser/parser/getfileinfo/
---

## GetFileInfo(string) {#getfileinfo_2}

Gibt die allgemeinen Informationen zu einer Datei zurück.

```csharp
public static FileInfo GetFileInfo(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |

### Rückgabewert

Eine Instanz der [`FileInfo`](../../../groupdocs.parser.options/fileinfo)-Klasse.

### Beispiele

Der folgende Code zeigt, wie geprüft wird, ob eine Datei passwortgeschützt ist:

```csharp
// Dateiinformation abrufen
Options.FileInfo info = Parser.GetFileInfo(filePath);
// Überprüfen Sie die Eigenschaft IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### Siehe auch

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(string, LoadOptions) {#getfileinfo_3}

Gibt die allgemeinen Informationen zu einer Datei zurück.

```csharp
public static FileInfo GetFileInfo(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Pfad zur Datei. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Rückgabewert

Eine Instanz der [`FileInfo`](../../../groupdocs.parser.options/fileinfo)-Klasse.

### Beispiele

Der folgende Code zeigt, wie der Dateityp des passwortgeschützten Dokuments überprüft wird:

```csharp
// Dateiinformation abrufen
Options.FileInfo info = Parser.GetFileInfo(filePath, new LoadOptions("password"));
// Überprüfen Sie die Eigenschaft IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Den Dateityp ausgeben
Console.WriteLine(info.FileType.ToString());
```

### Siehe auch

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream) {#getfileinfo}

Gibt die allgemeinen Informationen zu einer Datei zurück.

```csharp
public static FileInfo GetFileInfo(Stream document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Der Quell-Eingabestream. |

### Rückgabewert

Eine Instanz der [`FileInfo`](../../../groupdocs.parser.options/fileinfo)-Klasse.

### Beispiele

Der folgende Code zeigt, wie geprüft wird, ob eine Datei passwortgeschützt ist:

```csharp
// Dateiinformation abrufen
Options.FileInfo info = Parser.GetFileInfo(document);
// Überprüfen Sie die Eigenschaft IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### Siehe auch

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream, LoadOptions) {#getfileinfo_1}

Gibt die allgemeinen Informationen zu einer Datei zurück.

```csharp
public static FileInfo GetFileInfo(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Der Quell-Eingabestream. |
| loadOptions | LoadOptions | Die Optionen zum Öffnen der Datei. |

### Rückgabewert

Eine Instanz der [`FileInfo`](../../../groupdocs.parser.options/fileinfo)-Klasse.

### Beispiele

Der folgende Code zeigt, wie der Dateityp des passwortgeschützten Dokuments überprüft wird:

```csharp
// Dateiinformation abrufen
Options.FileInfo info = Parser.GetFileInfo(document);
// Überprüfen Sie die Eigenschaft IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Den Dateityp ausgeben
Console.WriteLine(info.FileType.ToString());
```

### Siehe auch

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
