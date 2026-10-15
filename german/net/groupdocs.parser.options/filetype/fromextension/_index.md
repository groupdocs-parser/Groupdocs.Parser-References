---
title: "FromExtension"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Ordnet Dateierweiterungen Dateitypen zu."
type: docs
weight: 930
url: /de/net/groupdocs.parser.options/filetype/fromextension/
---

## FileType.FromExtension method

Ordnet Dateierweiterungen Dateitypen zu.

```csharp
public static FileType FromExtension(string extension)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Erweiterung | String | Dateierweiterung (einschließlich des Punktes "."). |

### Rückgabewert

Wenn der Dateityp unterstützt wird, wird er zurückgegeben, andernfalls wird der Standard‑[`Unknown`](../unknown) Dateityp zurückgegeben.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wird ausgelöst, wenn *extension* null oder ein leerer String ist. |

### Siehe auch

* class [FileType](../../filetype)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
