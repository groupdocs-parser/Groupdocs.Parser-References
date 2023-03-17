---
title: OcrEventHandler
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Stellt einen Handler für OCREreignisse bereit.
type: docs
weight: 490
url: /de/net/groupdocs.parser.options/ocreventhandler/
---
## OcrEventHandler class

Stellt einen Handler für OCR-Ereignisse bereit.

```csharp
public class OcrEventHandler
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [OcrEventHandler](ocreventhandler)() | Initialisiert eine neue Instanz von[`OcrEventHandler`](../ocreventhandler) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [HasWarnings](../../groupdocs.parser.options/ocreventhandler/haswarnings) { get; } | Ruft den Wert ab, der angibt, ob die Liste der Warnungen nicht leer ist. |
| [Warnings](../../groupdocs.parser.options/ocreventhandler/warnings) { get; } | Ruft eine Liste mit Warnmeldungen ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetWarnings](../../groupdocs.parser.options/ocreventhandler/getwarnings)(int) | Gibt eine Liste mit Warnmeldungen für die Seite mit zurück*pageIndex* . |
| virtual [OnWarnings](../../groupdocs.parser.options/ocreventhandler/onwarnings)(int, IList&lt;string&gt;) | Legt Warnmeldungen für die Seite fest. |

### Siehe auch

* namensraum [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* Montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->